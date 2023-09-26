Fri Sep  8 13:44:01 UTC 2023
STRATEGY: pending
MAX-DEPTH: 500
TIMEOUT: 86400
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
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000800000000000000000000000000000000000000000000000000000000000000000, decoded_data: (128, 0), value: 0x0


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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


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
Caller: [SOMEGUY], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d0000000000000000000000000000000000000000000000000000000000000140, decoded_data: (320,), value: 0x0
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000c18a3eadf0696f7f9dcbfadbf646af0ae283320a8142d7c71b4a5043c08d914, decoded_data: (0, 5471289829323276755738560575350695832856551249722628964282460931148585949460), value: 0x0


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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000, decoded_data: (2, 0), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000040000000000000000000000000000000000000000000000000000000000000000, decoded_data: (4, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1437
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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000800000000000000000000000000000000000000000000000000000000000000000, decoded_data: (128, 0), value: 0x0


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


Fri Sep  8 14:17:33 UTC 2023
