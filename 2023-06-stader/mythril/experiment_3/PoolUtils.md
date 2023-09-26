Sun Aug  6 11:44:59 UTC 2023
STRATEGY: bfs
MAX-DEPTH: 150
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
Caller: [SOMEGUY], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffc080000000000000000000000000000000000000000000000000000000000003e1, value: 0x0


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
Caller: [ATTACKER], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff9cffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff5b, value: 0x0


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
Caller: [ATTACKER], function: processValidatorExitList(bytes[]), txdata: 0xff6bceec00000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000002800000000000000000000000000000000000000000000000000000800ffff921800000000000000000000000000000000000000000000000000000000000015c, value: 0x0


Sun Aug  6 12:53:35 UTC 2023
