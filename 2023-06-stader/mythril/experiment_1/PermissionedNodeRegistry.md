Sun Jul 30 22:03:04 UTC 2023
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedNodeRegistry
- Function name: `operatorStructById(uint256)`
- PC address: 29824
- Estimated Gas Usage: 6915 - 9747

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1263

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: operatorStructById(uint256), txdata: 0xc8a00e7a8000000000000000000000000000000000000000000000000000000000000008, decoded_data: (57896044618658097711785492504343953926634992332820282019728792003956564819976,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedNodeRegistry
- Function name: `validatorRegistry(uint256)`
- PC address: 29824
- Estimated Gas Usage: 12494 - 16083

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1263

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: validatorRegistry(uint256), txdata: 0x5a1239c10000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionedNodeRegistry
- Function name: `activateNodeOperator(uint256)`
- PC address: 30742
- Estimated Gas Usage: 16473 - 93132

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1431

### Code

```
eq(value, 0xffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: activateNodeOperator(uint256), txdata: 0x91dcd6b28000000000170001b00007000000000200201007fef7eadcf900000000000001, decoded_data: (57896044618667559373582701236562302886066352383383499799427569950682666500097,), value: 0x0


Mon Jul 31 00:09:18 UTC 2023
