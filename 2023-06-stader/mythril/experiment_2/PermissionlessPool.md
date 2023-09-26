Thu Aug  3 07:32:05 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for #utility.yul

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PermissionlessPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 4320
- Estimated Gas Usage: 3493 - 73323

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PermissionlessPool.sol:172

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getTotalActiveValidatorCount()
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
- Contract: PermissionlessPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 4355
- Estimated Gas Usage: 3493 - 73323

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionlessPool.sol:172

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getTotalActiveValidatorCount()
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
- Contract: PermissionlessPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 4362
- Estimated Gas Usage: 3493 - 73323

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionlessPool.sol:172

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getTotalActiveValidatorCount()
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
- Contract: PermissionlessPool
- Function name: `getTotalQueuedValidatorCount()`
- PC address: 4582
- Estimated Gas Usage: 3515 - 73345

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PermissionlessPool.sol:165

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getTotalQueuedValidatorCount()
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
- Contract: PermissionlessPool
- Function name: `getTotalQueuedValidatorCount()`
- PC address: 4617
- Estimated Gas Usage: 3515 - 73345

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionlessPool.sol:165

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getTotalQueuedValidatorCount()
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
- Contract: PermissionlessPool
- Function name: `getTotalQueuedValidatorCount()`
- PC address: 4624
- Estimated Gas Usage: 3515 - 73345

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionlessPool.sol:165

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getTotalQueuedValidatorCount()
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
- Contract: PermissionlessPool
- Function name: `getCollateralETH()`
- PC address: 7032
- Estimated Gas Usage: 3449 - 73279

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PermissionlessPool.sol:192

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getCollateralETH()
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
- Contract: PermissionlessPool
- Function name: `getCollateralETH()`
- PC address: 7067
- Estimated Gas Usage: 3449 - 73279

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionlessPool.sol:192

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getCollateralETH()
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
- Contract: PermissionlessPool
- Function name: `getCollateralETH()`
- PC address: 7074
- Estimated Gas Usage: 3449 - 73279

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PermissionlessPool.sol:192

### Code

```
INodeRegistry(staderConfig.getPermissionlessNodeRegistry()).getCollateralETH()
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
- Contract: PermissionlessPool
- Function name: `getTotalActiveValidatorCount()`
- PC address: 16538
- Estimated Gas Usage: 3493 - 73323

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:715

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


Thu Aug  3 08:34:14 UTC 2023
