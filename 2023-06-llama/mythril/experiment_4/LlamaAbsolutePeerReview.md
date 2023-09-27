Thu Sep  7 22:34:42 UTC 2023
STRATEGY: naive-random
MAX-DEPTH: 250
TIMEOUT: 86400
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAbsolutePeerReview
- Function name: `isApprovalEnabled((uint256,address,uint8,address,address,uint256,bytes),address,uint8)`
- PC address: 1418
- Estimated Gas Usage: 2080 - 2505

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: src/strategies/LlamaAbsolutePeerReview.sol:67

### Code

```
actionInfo.creator == policyholder
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: isApprovalEnabled((uint256,address,uint8,address,address,uint256,bytes),address,uint8), txdata: 0x343d0d16000000000000000000000000000000000000000000000000000000000000000d00000000000000000000000002000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaAbsolutePeerReview
- Function name: `isActive((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 5919
- Estimated Gas Usage: 5281 - 42385

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: src/strategies/LlamaAbsoluteStrategyBase.sol:268

### Code

```
block.timestamp <= approvalEndTime(actionInfo) && (isFixedLengthApprovalPeriod || !isActionApproved(actionInfo))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: isActive((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xb0b061960000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000008000000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000080', 2, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAbsolutePeerReview
- Function name: `isDisapprovalEnabled((uint256,address,uint8,address,address,uint256,bytes),address,uint8)`
- PC address: 6286
- Estimated Gas Usage: 2928 - 3683

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: src/strategies/LlamaAbsolutePeerReview.sol:79

### Code

```
minDisapprovals == type(uint128).max
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: isDisapprovalEnabled((uint256,address,uint8,address,address,uint256,bytes),address,uint8), txdata: 0xc56270410000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000212101420185e4520080201100445412101090000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAbsolutePeerReview
- Function name: `isDisapprovalEnabled((uint256,address,uint8,address,address,uint256,bytes),address,uint8)`
- PC address: 6405
- Estimated Gas Usage: 2928 - 3683

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: src/strategies/LlamaAbsolutePeerReview.sol:80

### Code

```
actionInfo.creator == policyholder
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: isDisapprovalEnabled((uint256,address,uint8,address,address,uint256,bytes),address,uint8), txdata: 0xc5627041000000000000000000000000000000000000000000000000000000000000000d00000000000000000000000001000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: LlamaAbsolutePeerReview
- Function name: `isActive((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 6763
- Estimated Gas Usage: 10952 - 85676

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: src/strategies/LlamaAbsoluteStrategyBase.sol:273

### Code

```
llamaCore.getAction(actionInfo.id)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: isActive((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xb0b061960000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 0, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaAbsolutePeerReview
- Function name: `minExecutionTime((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 7995
- Estimated Gas Usage: 1482 - 1907

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: src/lib/LlamaUtils.sol:11

### Code

```
if (n > type(uint64).max) revert UnsafeCast(n)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: minExecutionTime((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xed93c1b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 0, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaAbsolutePeerReview
- Function name: `minExecutionTime((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 11453
- Estimated Gas Usage: 1416 - 1841

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: #utility.yul:822

### Code

```
if gt(x, sum) { panic_error_0x11() }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: minExecutionTime((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xed93c1b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 0, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAbsolutePeerReview
- Function name: `validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address)`
- PC address: 11747
- Estimated Gas Usage: 6292 - 44533

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:890

### Code

```
add(rel_offset_of_tail, base_ref)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address), txdata: 0xfb57244400000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAbsolutePeerReview
- Function name: `validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address)`
- PC address: 11757
- Estimated Gas Usage: 6292 - 44533

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:893

### Code

```
add(value, 0x20)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address), txdata: 0xfb572444000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffdc, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAbsolutePeerReview
- Function name: `validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address)`
- PC address: 11790
- Estimated Gas Usage: 6292 - 44533

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:895

### Code

```
sub(calldatasize(), mul(length, 0x01))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address), txdata: 0xfb572444000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ffffffbfffffffffffffbf907ffffffffffffdfffffffffffc00000000000ffb, value: 0x0


Fri Sep  8 00:02:26 UTC 2023
