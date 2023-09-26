Mon Aug 28 10:45:38 UTC 2023
STRATEGY: naive-random
MAX-DEPTH: 250
TIMEOUT: 86400
# Analysis results for contracts/PoolSelector.sol

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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1162
- Estimated Gas Usage: 9109 - 148773

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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000088800f8f4e0400c04004003e98151ac8ceb64ffffff17c5000000c04fd0000501, decoded_data: (8, 61516265642261520378392498116374007973833347252187361417791757052906336945409), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000280000000000000000000000000000000000000000000000000000000000000000, decoded_data: (40, 0), value: 0x0


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
Caller: [CREATOR], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d0000000000000000000000000000000000000000000000000000000000000020, decoded_data: (32,), value: 0x0
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000008304008400000001c000000000000000100100000000000000000000010004000, decoded_data: (8, 21824151883549964436922985656739454680703533109342000447978543429557556363264), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1304
- Estimated Gas Usage: 9109 - 148773

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
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000002074a51bfffffd5fffbf8ffb5eefc7eecd1bbff3fdfb95832fd73fea9d37fdfe, decoded_data: (0, 14680104957204539915202338548612467011021767705436262966890414070454589849086), value: 0x0


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
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000440000000000000000000000000000000000000000000000000000000000000000, decoded_data: (68, 0), value: 0x0


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
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc1000000000000000000000000000000000000000000000000000000000000000822e088dfa038d5c005e80b4e1d82806023938008142840510201800444014420, decoded_data: (8, 15775355260786032799710877597968897627551864541549813922971182030701857948704), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000, decoded_data: (2, 0), value: 0x0


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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


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


Mon Aug 28 11:33:35 UTC 2023
