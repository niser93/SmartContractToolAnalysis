Wed Aug 30 07:08:05 UTC 2023
STRATEGY: weighted-random
MAX-DEPTH: 1000
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
Caller: [SOMEGUY], function: markValidatorReadyToDeposit(bytes[],bytes[],bytes[]), txdata: 0x13797bff000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000004, decoded_data: ([], [], []), value: 0x0


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
Caller: [SOMEGUY], function: operatorStructById(uint256), txdata: 0xc8a00e7a8000000000000000000000000000000000000000000000000000000000000017, decoded_data: (57896044618658097711785492504343953926634992332820282019728792003956564819991,), value: 0x0


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
Caller: [SOMEGUY], function: validatorRegistry(uint256), txdata: 0x5a1239c18000000000000000000000000000000000000000000000000000000001a6a811, decoded_data: (57896044618658097711785492504343953926634992332820282019728792003956592519185,), value: 0x0


Wed Aug 30 13:59:02 UTC 2023
