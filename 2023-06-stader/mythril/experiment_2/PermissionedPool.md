Wed Aug  2 20:47:36 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for contracts/PermissionedPool.sol

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PermissionedPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 6977
- Estimated Gas Usage: 3515 - 73345

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PermissionedPool.sol:193

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getTotalActiveValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getTotalActiveValidatorCount(), txdata: 0x77c359e1, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 7012
- Estimated Gas Usage: 3515 - 73345

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionedPool.sol:193

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getTotalActiveValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getTotalActiveValidatorCount(), txdata: 0x77c359e1, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 7019
- Estimated Gas Usage: 3515 - 73345

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionedPool.sol:193

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getTotalActiveValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getTotalActiveValidatorCount(), txdata: 0x77c359e1, value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PermissionedPool
- Function name: `getTotalQueuedValidatorCount()`
- PC address: 7239
- Estimated Gas Usage: 3450 - 73280

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PermissionedPool.sol:186

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getTotalQueuedValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getTotalQueuedValidatorCount(), txdata: 0x7bd977d9, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getTotalQueuedValidatorCount()`
- PC address: 7274
- Estimated Gas Usage: 3450 - 73280

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionedPool.sol:186

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getTotalQueuedValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getTotalQueuedValidatorCount(), txdata: 0x7bd977d9, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getTotalQueuedValidatorCount()`
- PC address: 7281
- Estimated Gas Usage: 3450 - 73280

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionedPool.sol:186

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getTotalQueuedValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getTotalQueuedValidatorCount(), txdata: 0x7bd977d9, value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PermissionedPool
- Function name: `getCollateralETH()`
- PC address: 9646
- Estimated Gas Usage: 3471 - 73301

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PermissionedPool.sol:218

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getCollateralETH()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getCollateralETH(), txdata: 0xb01db078, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getCollateralETH()`
- PC address: 9681
- Estimated Gas Usage: 3471 - 73301

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionedPool.sol:218

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getCollateralETH()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getCollateralETH(), txdata: 0xb01db078, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getCollateralETH()`
- PC address: 9688
- Estimated Gas Usage: 3471 - 73301

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionedPool.sol:218

### Code

```
INodeRegistry(staderConfig.getPermissionedNodeRegistry()).getCollateralETH()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getCollateralETH(), txdata: 0xb01db078, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 18294
- Estimated Gas Usage: 3515 - 73345

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:586

### Code

```
sub(dataEnd, headStart)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: getTotalActiveValidatorCount(), txdata: 0x77c359e1, value: 0x0


Wed Aug  2 21:49:57 UTC 2023
