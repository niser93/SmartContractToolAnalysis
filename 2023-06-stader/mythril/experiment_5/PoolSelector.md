Wed Aug 30 15:04:20 UTC 2023
STRATEGY: weighted-random
MAX-DEPTH: 1000
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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000, decoded_data: (16, 0), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000280000000000000000000000000000000000000000000000000000000000000000, decoded_data: (40, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1169
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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000883c961effffffffffffffff1413028f7ffef5e7bbcfffefa713606ef85e7fff, decoded_data: (0, 61621594328921297144785032482619937524725179010283685982823645834692249157631), value: 0x0


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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000883ba5fedffffffffffffffffffffffffffffffffffffffffffffffffffffffe, decoded_data: (0, 61619937043709780727261744738882029252811523279784803973301029207859703840766), value: 0x0


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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000807639423eff1f17ff029081801e095540d00000000000003fea007e4700000021, decoded_data: (128, 53474083629160808871488300027451264967887563733754679009418585334542426439713), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1311
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
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000243c0a1e5b7e4c542880000000000310fbf3edfe0000efbddf7f00fb00bfc66f, decoded_data: (0, 16389343208781535552327024350522031180781568029093300366561941410938246645359), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1430
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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000010ff2640400d2344e6228000340c1b12000000000000000000000004400000001, decoded_data: (1, 7212960000986303600398707448839523322500375288258516515441337132192844742657), value: 0x0


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
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 8958
- Estimated Gas Usage: 9109 - 148773

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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc1000000000000000000000000000000000000000000000000000000000000000106414717fffffffffffffffffffffffffffffffffffffffffffffffffffffffe, decoded_data: (1, 2829212821739535453307122238363996301118061914926356190371847613976019992574), value: 0x0


Wed Aug 30 15:45:59 UTC 2023
