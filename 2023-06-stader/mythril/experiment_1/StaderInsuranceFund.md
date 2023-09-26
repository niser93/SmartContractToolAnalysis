Sun Jul 30 10:26:14 UTC 2023
# Analysis results for contracts/StaderInsuranceFund.sol

## External Call To User-Supplied Address
- SWC ID: 107
- Severity: Low
- Contract: StaderInsuranceFund
- Function name: `withdrawFund(uint256)`
- PC address: 1566
- Estimated Gas Usage: 15603 - 125691

### Description

A call to a user-supplied address is executed.
An external message call to an address specified by the caller is executed. Note that the callee account might contain arbitrary code and could re-enter any function within this contract. Reentering the contract in an intermediate state may lead to unexpected behaviour. Make sure that no state modifications are executed after this call and/or reentrancy guards are in place.
In file: contracts/StaderInsuranceFund.sol:48

### Code

```
payable(msg.sender).call{value: _amount}('')
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x10000000000000000, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: depositFund(), txdata: 0x8d0d8cb6, value: 0x1
Caller: [ATTACKER], function: withdrawFund(uint256), txdata: 0x0cee17250000000000000000000000000000000000000000000000000000000000000001, decoded_data: (1,), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: StaderInsuranceFund
- Function name: `withdrawFund(uint256)`
- PC address: 1566
- Estimated Gas Usage: 15603 - 125691

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/StaderInsuranceFund.sol:48

### Code

```
payable(msg.sender).call{value: _amount}('')
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: depositFund(), txdata: 0x8d0d8cb6, value: 0x1
Caller: [ATTACKER], function: withdrawFund(uint256), txdata: 0x0cee17250000000000000000000000000000000000000000000000000000000000000001, decoded_data: (1,), value: 0x0


## Unprotected Ether Withdrawal
- SWC ID: 105
- Severity: High
- Contract: StaderInsuranceFund
- Function name: `withdrawFund(uint256)`
- PC address: 1566
- Estimated Gas Usage: 15603 - 125691

### Description

Any sender can withdraw Ether from the contract account.
Arbitrary senders other than the contract creator can profitably extract Ether from the contract account. Verify the business logic carefully and make sure that appropriate security controls are in place to prevent unexpected loss of funds.
In file: contracts/StaderInsuranceFund.sol:48

### Code

```
payable(msg.sender).call{value: _amount}('')
```

### Initial State:

Account: [CREATOR], balance: 0x40020000000000000, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x1fffffffffffffff, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: depositFund(), txdata: 0x8d0d8cb6, value: 0x1
Caller: [ATTACKER], function: withdrawFund(uint256), txdata: 0x0cee17250000000000000000000000000000000000000000000000000000000000000001, decoded_data: (1,), value: 0x0


## State access after external call
- SWC ID: 107
- Severity: Medium
- Contract: StaderInsuranceFund
- Function name: `withdrawFund(uint256)`
- PC address: 3128
- Estimated Gas Usage: 15603 - 125691

### Description

Write to persistent state following external call
The contract account state is accessed after an external call to a user defined address. To prevent reentrancy issues, consider accessing the state only before the call, especially if the callee is untrusted. Alternatively, a reentrancy lock can be used to prevent untrusted callees from re-entering the contract in an intermediate state.
In file: node_modules/@openzeppelin/contracts-upgradeable/security/ReentrancyGuardUpgradeable.sol:72

### Code

```
_status = _NOT_ENTERED
```

### Initial State:

Account: [CREATOR], balance: 0x40000440000000000, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: depositFund(), txdata: 0x8d0d8cb6, value: 0x1
Caller: [ATTACKER], function: withdrawFund(uint256), txdata: 0x0cee17250000000000000000000000000000000000000000000000000000000000000001, decoded_data: (1,), value: 0x0


Sun Jul 30 10:28:57 UTC 2023
