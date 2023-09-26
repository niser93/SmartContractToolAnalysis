Tue Aug 29 16:19:03 UTC 2023
STRATEGY: weighted-random
MAX-DEPTH: 1000
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
Caller: [ATTACKER], function: operatorStructById(uint256), txdata: 0xc8a00e7a000000000000000000000000deadbeefdeadbeefdeadbeefdeadbeefdeadbeef, decoded_data: (1271270613000041655817448348132275889066893754095,), value: 0x0


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
Caller: [SOMEGUY], function: activateNodeOperator(uint256), txdata: 0x91dcd6b28000000000000000ff3002033f00138800000000000000000000000007ffffd0, decoded_data: (57896044618658097718042672550732389480700862614291688646504168895847115784144,), value: 0x0


Wed Aug 30 06:00:56 UTC 2023
