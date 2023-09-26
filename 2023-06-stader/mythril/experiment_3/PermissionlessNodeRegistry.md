Sat Aug  5 10:10:50 UTC 2023
STRATEGY: bfs
MAX-DEPTH: 150
TIMEOUT: 86400
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `markValidatorReadyToDeposit(bytes[],bytes[],bytes[])`
- PC address: 18810
- Estimated Gas Usage: 16461 - 91873

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: node_modules/@openzeppelin/contracts-upgradeable/security/ReentrancyGuardUpgradeable.sol:63

### Code

```
_status != _ENTERED
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: markValidatorReadyToDeposit(bytes[],bytes[],bytes[]), txdata: 0x13797bff0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001b0000000000000000000000000000000000000000000000000000000000000014, decoded_data: ([], [], []), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `operatorStructById(uint256)`
- PC address: 30749
- Estimated Gas Usage: 6892 - 9724

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1218

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: operatorStructById(uint256), txdata: 0xc8a00e7a0000000000000000000000000010000000000000000000000000000000000000, decoded_data: (356811923176489970264571492362373784095686656,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `validatorRegistry(uint256)`
- PC address: 30749
- Estimated Gas Usage: 12472 - 16061

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1218

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: validatorRegistry(uint256), txdata: 0x5a1239c1fffffffffffffffffffffffe0000002080000000004002000000000000000000, decoded_data: (115792089237316195423570985005764904589667355754163771817281881012140203048960,), value: 0x0


Sat Aug  5 11:20:39 UTC 2023
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `markValidatorReadyToDeposit(bytes[],bytes[],bytes[])`
- PC address: 18810
- Estimated Gas Usage: 16461 - 91873

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: node_modules/@openzeppelin/contracts-upgradeable/security/ReentrancyGuardUpgradeable.sol:63

### Code

```
_status != _ENTERED
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: markValidatorReadyToDeposit(bytes[],bytes[],bytes[]), txdata: 0x13797bff0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c0000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([], [], []), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `operatorStructById(uint256)`
- PC address: 30749
- Estimated Gas Usage: 6892 - 9724

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1218

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: operatorStructById(uint256), txdata: 0xc8a00e7aa35f063846a72858f4a8309e9605504b566f1f2d31cb65fb9ae6000080000002, decoded_data: (73894887717902086987953662963637627690396734611453648628030238705915476836354,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `validatorRegistry(uint256)`
- PC address: 30749
- Estimated Gas Usage: 12472 - 16061

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1218

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: validatorRegistry(uint256), txdata: 0x5a1239c1f154ffbc6572da55cabf4fbd1dfd45cdec57f3a8000000000000000000000004, decoded_data: (109157576686480778089168772639882064476425714559325869272332676499657019359236,), value: 0x0


Sat Aug  5 16:55:13 UTC 2023
