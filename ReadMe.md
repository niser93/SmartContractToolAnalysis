DLTs are an emerging reality opening the way to new application design paradigms like smart contracts-based distributed applications. 
If on one side DLTs are creating new markets and opportunities, on the other they are also exposing users to new security issues deriving 
from the smart contracts usage and in particular from the scarce maturity in terms of security practices in their design and development. 
This paper raises a warning on the efficacy of a state-of-the-art software testing tool, namely Mythril, by challenging it with real 
smart contracts extracted from the Code4arena competitions and comparing its performance with security audits released during the contests. 
The paper highlights possible root causes of inefficiency, opening the way toward a more scalable and efficient smart contract testing tools.


# Asymmetry
**contest**: [2023-03-Asymmetry](https://code4rena.com/contests/2023-03-asymmetry-contest)\
**Analysis report**: [https://code4rena.com/reports/2023-03-asymmetry](https://code4rena.com/reports/2023-03-asymmetry)\
**Bot report**: [https://gist.github.com/muratkurtulus/c7a89b0ef411b5b96dd8af23ccd95dc4](https://gist.github.com/muratkurtulus/c7a89b0ef411b5b96dd8af23ccd95dc4)\
**Files in scope**: 4 (including 4 contracts)\
**SLOC**:460\
**Our comparison and description**: [2023-03-asymmetry/report.md](2023-03-asymmetry/report.md)


* **Analysis report**:\
High in analysis report: 8\
Medium in analysis report: 12


* **Bot report**:\
High in bot report: 0\
Medium in bot report: 0


* **Mythril report**:\
High in Mythril report: 0\
Medium in Mythril report: 0\
Low in Mythril report: 3\
Valid finds in Mythril report: 0


* **Comparison Analysis report/mythril finds**:\
High in analysis report found also by Mythril: 0 (out of 8)\
Medium in analysis report found also by Mythril: 1 (out of 12)


* **Comparison bot report/mythril finds**:\
High in bot report found also by Mythril: 0 (out of 0)\
Medium in bot report found also by Mythril: 0 (out of 0)



# Juicebox
**contest**: [2023-05-Juicebox](https://code4rena.com/contests/2023-05-juicebox-buyback-delegate)\
**Analysis report**: [https://code4rena.com/reports/2023-05-juicebox](https://code4rena.com/reports/2023-05-juicebox)\
**Bot report**: [https://gist.github.com/itsmetechjay/2efc963de59bcad62e69de48171d10ca](https://gist.github.com/itsmetechjay/2efc963de59bcad62e69de48171d10ca)\
**Files in scope**: 1 (including 1 contract)\
**SLOC**:160\
**Our comparison and description**: [2023-05-juicebox/report.md](2023-05-juicebox/report.md)


* **Analysis report**:\
High in analysis report: 0\
Medium in analysis report: 3


* **Bot report**:\
High in bot report: 0\
Medium in bot report: 3


* **Mythril report**:\
High in Mythril report: 0\
Medium in Mythril report: 0
Low in Mythril report: 0\
Valid finds in Mythril report: 0


* **Comparison Analysis report/mythril finds**:\
High in analysis report found also by Mythril: 0 (out of 0)\
Medium in analysis report found also by Mythril: 0 (out of 3)


* **Comparison bot report/mythril finds**:\
High in bot report found also by Mythril: 0 (out of 0)\
Medium in bot report found also by Mythril: 0 (out of 3)



# Llama
**contest**: [2023-06-Llama](https://code4rena.com/contests/2023-06-llama)\
**Analysis report**: [https://code4rena.com/reports/2023-06-llama](https://code4rena.com/reports/2023-06-llama)\
**Bot report**: [https://gist.github.com/itsmetechjay/610f1b31f419156f06898ee10c89402d](https://gist.github.com/itsmetechjay/610f1b31f419156f06898ee10c89402d)\
**Files in scope**: 23 (including 11 contracts)\
**SLOC**:2096\
**Our comparison and description**: [2023-06-llama/report.md](2023-06-llama/report.md)


* **Analysis report**:\
High in analysis report: 2\
Medium in analysis report: 3


* **Bot report**:\
High in bot report: 0\
Medium in bot report: 2


* **Mythril report**:\
High in Mythril report: 11 (11 IAB)\
Medium in Mythril report: 2
Low in Mythril report: 13\
Valid finds in Mythril report: 0


* **Comparison Analysis report/mythril finds**:\
High in analysis report found also by Mythril: 0\
Medium in analysis report found also by Mythril: 0


* **Comparison bot report/mythril finds**:\
High in bot report found also by Mythril: 0\
Medium in bot report found also by Mythril: 0




# Stader
**contest**: [2023-06-Stader](https://code4rena.com/contests/2023-06-stader-labs)\
**Analysis report**: [https://code4rena.com/reports/2023-06-stader](https://code4rena.com/reports/2023-06-stader)\
**Bot report**: [https://gist.github.com/CloudEllie/9a06bd326750de18279979886ed93ffd](https://gist.github.com/CloudEllie/9a06bd326750de18279979886ed93ffd)\
**Files in scope**: 23 (including 23 contracts)\
**SLOC**:4343\
**Our comparison and description**: [2023-06-stader/report.md](2023-06-stader/report.md)


* **Analysis report**:\
High in analysis report: 1\
Medium in analysis report: 14


* **Bot report**:\
High in bot report: 0\
Medium in bot report: 1


* **Mythril report**:\
High in Mythril report: 28 (26 IAB)\
Medium in Mythril report: 1
Low in Mythril report: 25\
Valid finds in Mythril report: 2


* **Comparison Analysis report/mythril finds**:\
High in analysis report found also by Mythril: 1 (out of 1)\
Medium in analysis report found also by Mythril: 1 (out of 14)


* **Comparison bot report/mythril finds**:\
High in bot report found also by Mythril: 0 (out of 0)\
Medium in bot report found also by Mythril: 0 (out of 1)



# Analysis of Mythril high finds

In 4 contests, Mythril found 2 high vulnerabilities not IAB, both in STADER contest:

## SWC ID 105 - Unprotected Ether Withdrawal in StaderInsuranceFund.sol (not valid)

### Contract
StaderInsuranceFund.sol (1 instance)

### Mythril description
Any sender can withdraw Ether from the contract account.
Arbitrary senders other than the contract creator can profitably extract Ether from the contract account. Verify the business logic carefully and make sure that appropriate security controls are in place to prevent unexpected loss of funds.
In file: contracts/StaderInsuranceFund.sol:48

### Analysis of vulnerability validity 

[StaderInsuranceFund.sol#L40-L53](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/StaderInsuranceFund.sol#L40-L53)
```

40  // `MANAGER` can withdraw access fund
41  function withdrawFund(uint256 _amount) external override nonReentrant {
42      UtilLib.onlyManagerRole(msg.sender, staderConfig);
43      if (address(this).balance < _amount || _amount == 0) {
44          revert InvalidAmountProvided();
45      }
46  
47      //slither-disable-next-line arbitrary-send-eth
48      (bool success, ) = payable(msg.sender).call{value: _amount}('');
49      if (!success) {
50          revert TransferFailed();
51      }
52      emit FundWithdrawn(_amount);
53  }
```
This find is valid, because anyone could withdraw Ether using line 48:

```
(bool success, ) = payable(msg.sender).call{value: _amount}('');
```
However, line 42 protect this function from malicious attacker.

Only who has ```Manager Role``` can call ```withdrawFund(uint256 _amount)``` without revert

We can check ```UtilLib.onlyManagerRole(msg.sender, staderConfig)``` function:

[UtilLib.sol#L25-L30](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/library/UtilLib.sol#L25-L30)
```
//checks for Manager role in staderConfig
function onlyManagerRole(address _addr, IStaderConfig _staderConfig) internal view {
    if (!_staderConfig.onlyManagerRole(_addr)) {
        revert CallerNotManager();
    }
}
```

_staderConfig parameter is setted by external caller, when StaderInsuranceFund is initialized:

[StaderInsuranceFund.sol#L26-L33](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/StaderInsuranceFund.sol#L26-L33)
```
function initialize(address _admin, address _staderConfig) public initializer {
    UtilLib.checkNonZeroAddress(_admin);
    UtilLib.checkNonZeroAddress(_staderConfig);
    __AccessControl_init_unchained();
    __ReentrancyGuard_init();
    staderConfig = IStaderConfig(_staderConfig);
    _grantRole(DEFAULT_ADMIN_ROLE, _admin);
}
```
This function can be called once when contract is created (see [Writing Upgradeable Contracts](https://docs.openzeppelin.com/upgrades-plugins/1.x/writing-upgradeable)

Furthermore, _staderConfig can only been updated by address with DEFAULT_ADMIN_ROLE, also defined into initialize(address _admin, address _staderConfig):

[StaderInsuranceFund.sol#L68-L73](https://github.com/code-423n4/2023-06-stader/blob/7566b5a35f32ebd55d3578b8bd05c038feb7d9cc/contracts/StaderInsuranceFund.sol#L68-L73)
```
68  //update the address of staderConfig
69  function updateStaderConfig(address _staderConfig) external onlyRole(DEFAULT_ADMIN_ROLE) {
70      UtilLib.checkNonZeroAddress(_staderConfig);
71      staderConfig = IStaderConfig(_staderConfig);
72      emit UpdatedStaderConfig(_staderConfig);
73  }
```

Therefore, it seems that nobody can exploit vulnerability reported by Mythril.


## SWC-ID 112 Delegatecall to user-supplied address (valid)

### Contract
VaultProxy.sol (1 instance)

### Mythril description
The contract delegates execution to another contract with a user-supplied address.
The smart contract delegates execution to a user-supplied address.This could allow an attacker to execute arbitrary code in the context of this contract account and manipulate the state of the contract account or execute actions on its behalf.
In file: contracts/VaultProxy.sol:45

### Analysis of vulnerability validity 
This vulnerability is valid and is also inside Analysis report by warden.\
We describe it into [Stader H-01 VaultProxy implementation can be initialized by anyone and self-destructed](2023-06-stader/report.md#h-01-vaultproxy-implementation-can-be-initialized-by-anyone-and-self-destructed)


# Analysis of Mythril medium finds

## SWC-ID 104 Unchecked return value from external call. (not valid)

### Contract
LlamaExecutor.sol (2 instances)

[LlamaExecutor.sol#L34](https://github.com/code-423n4/2023-06-llama/blob/main/src/LlamaExecutor.sol#L34)

[LlamaExecutor.sol#L34](https://github.com/code-423n4/2023-06-llama/blob/main/src/LlamaExecutor.sol#L34)


### Mythril description
The return value of a message call is not checked.
External calls return a boolean value. If the callee halts with an exception, 'false' is returned and execution continues in the caller. The caller should check whether an exception happened and react accordingly to avoid unexpected behavior. For example it is often desirable to wrap external calls in require() so the transaction is reverted if the call fails.
In file: src/LlamaExecutor.sol:34

### Analysis of vulnerability validity

[LlamaExecutor.sol#L19-L35](https://github.com/code-423n4/2023-06-llama/blob/9d422c264b57657098c2784aa951852cad32e01c/src/LlamaExecutor.sol#L19-L35)
```
19  /// @notice Called by `executeAction` in the core contract to make the call described by the action.
20  /// @dev Using a separate executor contract ensures `target` being delegatecalled cannot write to `LlamaCore`'s
21  /// storage. By using a sole executor for calls and delegatecalls,
22  /// a Llama instance is represented by one contract address.
23  /// @param target The contract called when the action is executed.
24  /// @param value The value in wei to be sent when the action is executed.
25  /// @param isScript A boolean that determines if the target is a script and should be delegatecalled.
26  /// @param data Data to be called on the `target` when the action is executed.
27  /// @return success A boolean that indicates if the call succeeded.
28  /// @return result The data returned by the function being called.
29  function execute(address target, uint256 value, bool isScript, bytes calldata data)
30      external
31      returns (bool success, bytes memory result)
32  {
33      if (msg.sender != LLAMA_CORE) revert OnlyLlamaCore();
34      (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);
35  }
```

Mythril report that return of ```target.call{value: value}(data)``` is not checked.
This is true, but it is returned by ```execute(address target, uint256 value, bool isScript, bytes calldata data)```
The result of call is stored into a variable and returned, so we don't consider this find valid.

## SWC-ID 107 State access after external call (not valid)

### Contract
StaderInsuranceFund.sol (1 instance)

[StaderInsuranceFund.sol#L11](https://github.com/code-423n4/2023-06-stader/blob/main/contracts/StaderInsuranceFund.sol#L11)

### Mythril description
Write to persistent state following external call\
The contract account state is accessed after an external call to a user defined address. To prevent reentrancy issues, consider accessing the state only before the call, especially if the callee is untrusted. Alternatively, a reentrancy lock can be used to prevent untrusted callees from re-entering the contract in an intermediate state.\
In file: node_modules/@openzeppelin/contracts-upgradeable/security/ReentrancyGuardUpgradeable.sol:72

### Analysis of vulnerability validity
This vulnerability is not explicity inside the contract.
It is due to import of ```ReentrancyGuardUpgradeable.sol```, a contract from openzeppelin.

[ReentrancyGuardUpgradeable.sol#L66-L74](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/contracts/security/ReentrancyGuardUpgradeable.sol#L66-L74)
```
66  function _nonReentrantBefore() private {
67      // On the first call to nonReentrant, _status will be _NOT_ENTERED
68      if (_status == _ENTERED) {
69          revert ReentrancyGuardReentrantCall();
70      }
71
72
73      // Any calls to nonReentrant after this point will fail
74      _status = _ENTERED;
75  }
```

This module aims to avoid reentrancy. In order to do so, it permit only one call at a time.
So, vulnerability reported by Mythril can't be exploited, because _status variable avoids reentrancy.


