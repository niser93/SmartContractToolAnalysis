Sun Aug 27 13:45:48 UTC 2023
STRATEGY: naive-random
MAX-DEPTH: 250
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
Caller: [CREATOR], function: operatorStructById(uint256), txdata: 0xc8a00e7a007fe500000000000000488000048900000000000000000000008000a26603c1, decoded_data: (225970077140269848964428467157302089260830392894682570762743600880359441345,), value: 0x0


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
Caller: [ATTACKER], function: validatorRegistry(uint256), txdata: 0x5a1239c1a0222026203220222062200007f7fff7ccfddfe07fefff7ffff30002897f1010, decoded_data: (72430350457276771633296464420463690320164101273956654341984251438937493409808,), value: 0x0


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
Caller: [ATTACKER], function: activateNodeOperator(uint256), txdata: 0x91dcd6b207bfbfffffffffff000000000000000000000000000f0e6ed7bb000000000010, decoded_data: (3504982864754119907533764681712083841936981757219360894116492703609703628816,), value: 0x0


Mon Aug 28 01:51:35 UTC 2023
