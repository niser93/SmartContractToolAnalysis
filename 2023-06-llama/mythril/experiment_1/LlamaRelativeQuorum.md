Wed Aug  2 03:30:41 UTC 2023
STRATEGY: standard(dfs)
MAX-DEPTH: 22
TIMEOUT: 86400
# Analysis results for #utility.yul

## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaRelativeQuorum
- Function name: `isActive((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 5133
- Estimated Gas Usage: 5237 - 42341

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: src/strategies/LlamaRelativeQuorum.sol:278

### Code

```
block.timestamp <= approvalEndTime(actionInfo) && (isFixedLengthApprovalPeriod || !isActionApproved(actionInfo))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: isActive((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xb0b061960000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 0, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: LlamaRelativeQuorum
- Function name: `isActive((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 5825
- Estimated Gas Usage: 11990 - 86904

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: src/strategies/LlamaRelativeQuorum.sol:283

### Code

```
llamaCore.getAction(actionInfo.id)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: isActive((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xb0b061960000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000010', 1, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaRelativeQuorum
- Function name: `minExecutionTime((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 7084
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
Caller: [ATTACKER], function: minExecutionTime((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xed93c1b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 0, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaRelativeQuorum
- Function name: `minExecutionTime((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 10677
- Estimated Gas Usage: 1416 - 1841

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: #utility.yul:837

### Code

```
if gt(x, sum) { panic_error_0x11() }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: minExecutionTime((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xed93c1b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 0, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaRelativeQuorum
- Function name: `validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address)`
- PC address: 10971
- Estimated Gas Usage: 6292 - 44533

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:905

### Code

```
add(rel_offset_of_tail, base_ref)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address), txdata: 0xfb57244400000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaRelativeQuorum
- Function name: `validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address)`
- PC address: 10981
- Estimated Gas Usage: 6292 - 44533

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:908

### Code

```
add(value, 0x20)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address), txdata: 0xfb572444000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffdc, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaRelativeQuorum
- Function name: `validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address)`
- PC address: 11014
- Estimated Gas Usage: 6292 - 44533

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:910

### Code

```
sub(calldatasize(), mul(length, 0x01))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: validateActionCancelation((uint256,address,uint8,address,address,uint256,bytes),address), txdata: 0xfb572444000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000008080010000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000cf285b4000000000000000000000000000000000000000000000000000000003, value: 0x0


Wed Aug  2 06:50:32 UTC 2023
