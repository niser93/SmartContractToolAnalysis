Wed Aug  2 16:06:35 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for #utility.yul

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
Caller: [ATTACKER], function: validatorRegistry(uint256), txdata: 0x5a1239c10000000000000000000000004000020000000000000000000000000003ffffe0, decoded_data: (365375583557297593071414501426869759979374510048,), value: 0x0


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
Caller: [ATTACKER], function: activateNodeOperator(uint256), txdata: 0x91dcd6b20000ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffd9, decoded_data: (1766847064778384329583297500742918515827483896875618958121606201292619737,), value: 0x0


Wed Aug  2 20:47:35 UTC 2023
