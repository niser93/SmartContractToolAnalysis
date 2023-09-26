Tue Aug  1 08:01:38 UTC 2023
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
Caller: [CREATOR], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffe09200000000000000000000000000000000000000000000000000000000000102, value: 0x0


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
Caller: [SOMEGUY], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff9cfd7ddffc00fffcb700ebaf0000000ffffffc008500ffff7fff00feff77ffff75, value: 0x0


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
Caller: [ATTACKER], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002c1fa99a61c0ec3e6060000017cdbf98ffffffffffffffffffffffffffffe29f6800000000000000000000000000000000000000000000000000000000001f888, value: 0x0


Tue Aug  1 09:09:40 UTC 2023
