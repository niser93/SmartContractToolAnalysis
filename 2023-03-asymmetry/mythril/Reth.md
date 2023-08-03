Mon Jul 31 18:55:09 UTC 2023
# Analysis results for SafEth/derivatives/Reth.sol

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: Reth
- Function name: `balance()`
- PC address: 1671
- Estimated Gas Usage: 3509 - 73858

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: SafEth/derivatives/Reth.sol:222

### Code

```
IERC20(rethAddress()).balanceOf(address(this))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: balance(), txdata: 0xb69ef8a8, value: 0x0


Mon Jul 31 18:56:58 UTC 2023
