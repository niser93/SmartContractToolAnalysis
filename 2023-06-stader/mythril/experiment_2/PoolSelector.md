Thu Aug  3 08:34:14 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for contracts/PoolSelector.sol

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
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc1000000000000000000000000000000000000000000000000000000000000004040000640906bb34754311426facb4df61dd8feec800040000000000000000000, decoded_data: (64, 28948065460452991633745515251612497148800111342602174199464982176746442850304), value: 0x0


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
Caller: [CREATOR], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d0000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0, 0), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000883ca618bffffffffffbfffffffffffffffffffffffffffffffffffffffffffe, decoded_data: (0, 61621704588363179124113749599506571075745704857286003948200559077836365758462), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000008006f61ede8fefd7effffff6e565102101ffffbfffffeffffffffffffaffffec, decoded_data: (0, 57908344362885019462972057512677654753865522914664055568470687311113182248940), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000185c5f9eb36d73ffffffdf4a5195f3b7473f63f38ff9a360eefffffffffdc74d, decoded_data: (0, 11018718240428449805314198162127213949566359552726656353004756221776233350989), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: PoolSelector
- Function name: `computePoolAllocationForDeposit(uint8,uint256)`
- PC address: 1395
- Estimated Gas Usage: 9119 - 148783

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
Caller: [CREATOR], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d0000000000000000000000000000000000000000000000000000000000000100, decoded_data: (256,), value: 0x0
Caller: [ATTACKER], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc1000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000fe, decoded_data: (0, 254), value: 0x0


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
Caller: [SOMEGUY], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d000000000000000000000000000000000000000000000000000000000000e000, decoded_data: (57344,), value: 0x0
Caller: [SOMEGUY], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000005361, decoded_data: (0, 21345), value: 0x0


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
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000843ca61cfffffffffffffffffffffffffffffffffffffffffffffffff7fffffe, decoded_data: (0, 59812453308609886906011055209965853107586381296600021508177372057183478349822), value: 0x0


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
Caller: [SOMEGUY], function: updatePoolAllocationMaxSize(uint16), txdata: 0x21cc020d000000000000000000000000000000000000000000000000000000000000c000, decoded_data: (49152,), value: 0x0
Caller: [CREATOR], function: computePoolAllocationForDeposit(uint8,uint256), txdata: 0x00df7bc10000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000228c, decoded_data: (0, 8844), value: 0x0


Thu Aug  3 08:54:48 UTC 2023
