Fri Sep  8 14:17:34 UTC 2023
STRATEGY: pending
MAX-DEPTH: 500
TIMEOUT: 86400
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolUtils
- Function name: `processValidatorExitList(bytes[])`
- PC address: 14201
- Estimated Gas Usage: 5706 - 46850

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:775

### Code

```
add(base_ref, rel_offset_of_tail)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffe0ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff81, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolUtils
- Function name: `processValidatorExitList(bytes[])`
- PC address: 14236
- Estimated Gas Usage: 5706 - 46850

### Description

The arithmetic operator can overflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:779

### Code

```
add(addr, 32)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff9c80000000000000000000000000000000000000000000000000000000e0001443, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PoolUtils
- Function name: `processValidatorExitList(bytes[])`
- PC address: 14244
- Estimated Gas Usage: 5706 - 46850

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:780

### Code

```
sub(calldatasize(), mul(length, 0x01))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002c0072242800132a0027bd403929941b11f89d18f7add211c7824009aa44b87c7800000000000000000000000000000000000000000000000000000000000800c, value: 0x0


Fri Sep  8 15:21:45 UTC 2023
