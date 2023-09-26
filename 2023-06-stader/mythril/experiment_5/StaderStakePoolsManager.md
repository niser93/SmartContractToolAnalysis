Thu Aug 31 04:36:46 UTC 2023
STRATEGY: weighted-random
MAX-DEPTH: 1000
TIMEOUT: 86400
# Analysis results for contracts/StaderStakePoolsManager.sol

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: StaderStakePoolsManager
- Function name: `totalAssets()`
- PC address: 2167
- Estimated Gas Usage: 4141 - 74723

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/StaderStakePoolsManager.sol:136

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getExchangeRate()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: totalAssets(), txdata: 0x01e1d114, value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: StaderStakePoolsManager
- Function name: `depositETHOverTargetWeight()`
- PC address: 6296
- Estimated Gas Usage: 7865 - 27960

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/StaderStakePoolsManager.sol:216

### Code

```
if (block.number < lastExcessETHDepositBlock + excessETHDepositCoolDown) {
            revert CooldownNotComplete();
        }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: depositETHOverTargetWeight(), txdata: 0xbf040ea1, value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: StaderStakePoolsManager
- Function name: `convertToAssets(uint256)`
- PC address: 8988
- Estimated Gas Usage: 4583 - 75165

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/StaderStakePoolsManager.sol:295

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getExchangeRate()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: convertToAssets(uint256), txdata: 0x07a2d13a0101020401011001020101010101010101010101010101010101010101010101, decoded_data: (454093607086274407575874887200925900438757199406164155400716758027279073537,), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: StaderStakePoolsManager
- Function name: `previewWithdraw(uint256)`
- PC address: 8988
- Estimated Gas Usage: 4605 - 75187

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/StaderStakePoolsManager.sol:295

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getExchangeRate()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: previewWithdraw(uint256), txdata: 0x0a28a4770104010102010101010101010101010101010101010101010101010101010101, decoded_data: (459387165759710956122291334136177794420446941521837889684551514202946208001,), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: StaderStakePoolsManager
- Function name: `convertToShares(uint256)`
- PC address: 10957
- Estimated Gas Usage: 4598 - 75180

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/StaderStakePoolsManager.sol:272

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getExchangeRate()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: convertToShares(uint256), txdata: 0xc6e6f5920000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: StaderStakePoolsManager
- Function name: `previewDeposit(uint256)`
- PC address: 10957
- Estimated Gas Usage: 4608 - 75190

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/StaderStakePoolsManager.sol:272

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getExchangeRate()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: previewDeposit(uint256), txdata: 0xef8b30f70101010101010101010101010101010140010101010101010101010401010101, decoded_data: (454086624460063511464984254936031011273035421246765637402577429155303981313,), value: 0x0


Thu Aug 31 11:25:20 UTC 2023
