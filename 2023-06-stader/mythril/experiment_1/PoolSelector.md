Sun Jul 30 06:53:35 UTC 2023
# Analysis results for #utility.yul

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1127
- Estimated Gas Usage: 9119 - 148783

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PoolSelector.sol:57

### Code

```
poolUtils.getTotalActiveValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000800000000000000000000000000000000000000000000000000000000000000000, decoded_data: (128, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1162
- Estimated Gas Usage: 9119 - 148783

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PoolSelector.sol:57

### Code

```
poolUtils.getTotalActiveValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1169
- Estimated Gas Usage: 9119 - 148783

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PoolSelector.sol:57

### Code

```
poolUtils.getTotalActiveValidatorCount()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000000, decoded_data: (32, 0), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1269
- Estimated Gas Usage: 9109 - 148773

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PoolSelector.sol:59

### Code

```
poolUtils.getQueuedValidatorCountByPool(_poolId)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d0000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc1000000000000000000000000000000000000000000000000000000000000003c3133772efff9d72bf1bf9f03ebbfb7fffffff38066002a9af6044130c9000980, decoded_data: (60, 22254261355813978198819641766908115050796629257895712439698802455156073957760), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1304
- Estimated Gas Usage: 9119 - 148783

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PoolSelector.sol:59

### Code

```
poolUtils.getQueuedValidatorCountByPool(_poolId)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000, decoded_data: (16, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1311
- Estimated Gas Usage: 9119 - 148783

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PoolSelector.sol:59

### Code

```
poolUtils.getQueuedValidatorCountByPool(_poolId)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000, decoded_data: (16, 0), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1395
- Estimated Gas Usage: 9109 - 148773

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/PoolSelector.sol:60

### Code

```
poolUtils.getActiveValidatorCountByPool(_poolId)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000073bf5fbffffdf76e24c5fffe7d4dc4320020050703009c77c8117ef00eaa3b0, decoded_data: (0, 3272131638666260921439196821414867525280522185616155654834232623735040025520), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1430
- Estimated Gas Usage: 9119 - 148783

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PoolSelector.sol:60

### Code

```
poolUtils.getActiveValidatorCountByPool(_poolId)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000, decoded_data: (2, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1437
- Estimated Gas Usage: 9109 - 148773

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/PoolSelector.sol:60

### Code

```
poolUtils.getActiveValidatorCountByPool(_poolId)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc1000000000000000000000000000000000000000000000000000000000000004083ffeffeabfeffa331dec141227766f7bfcb823faca0000008020ca7777ba568, decoded_data: (64, 59705185549243023490261767203982570052230316948511065339618772250622928069992), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 8958
- Estimated Gas Usage: 9119 - 148783

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:461

### Code

```
sub(dataEnd, headStart)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


Sun Jul 30 07:31:40 UTC 2023
