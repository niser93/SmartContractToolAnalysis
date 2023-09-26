Thu Sep  7 15:28:44 UTC 2023
STRATEGY: pending
MAX-DEPTH: 500
TIMEOUT: 86400
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
Caller: [CREATOR], function: operatorStructById(uint256), txdata: 0xc8a00e7a00000000000000000000400000000000e208401088000083fc0ffe1ffffdffe1, decoded_data: (23945242826029813860213978513687183808634751683526625,), value: 0x0


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
Caller: [ATTACKER], function: validatorRegistry(uint256), txdata: 0x5a1239c17fffffffffffffffffffffffffffffefffffffffffffffffffffffffffffff90, decoded_data: (57896044618658097711785492504343953921190474462085266604314798285048273436560,), value: 0x0


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
Caller: [CREATOR], function: activateNodeOperator(uint256), txdata: 0x91dcd6b28000000000170001b00007000000000200201007fef76adcf900000000000000, decoded_data: (57896044618667559373582701236562302886066352383383499194964660143368079147008,), value: 0x0


Fri Sep  8 04:47:47 UTC 2023
