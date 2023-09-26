Sat Sep  9 11:00:30 UTC 2023
STRATEGY: pending
MAX-DEPTH: 500
TIMEOUT: 86400
# Analysis results for contracts/VaultProxy.sol

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

```
vaultImplementation.delegatecall(_input)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x1, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: blockHashAddendsInexpansible(uint256), txdata: 0x00000000, value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: VaultProxy
- Function name: `fallback`
- PC address: 528
- Estimated Gas Usage: 4234 - 76512

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/VaultProxy.sol:45

### Code

```
vaultImplementation.delegatecall(_input)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: blockHashAddendsInexpansible(uint256), txdata: 0x00000000, value: 0x0


Sat Sep  9 11:05:49 UTC 2023
