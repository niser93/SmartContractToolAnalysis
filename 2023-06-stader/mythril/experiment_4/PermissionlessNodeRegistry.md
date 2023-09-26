Mon Aug 28 02:55:44 UTC 2023
STRATEGY: naive-random
MAX-DEPTH: 250
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
Caller: [SOMEGUY], function: markValidatorReadyToDeposit(bytes[],bytes[],bytes[]), txdata: 0x13797bff000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006, decoded_data: ([], [], []), value: 0x0


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
Caller: [ATTACKER], function: operatorStructById(uint256), txdata: 0xc8a00e7a7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff9d, decoded_data: (57896044618658097711785492504343953926634992332820282019728792003956564819869,), value: 0x0


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
Caller: [ATTACKER], function: validatorRegistry(uint256), txdata: 0x5a1239c18000000000000000000000000000000003feffffffffff800000000000000008, decoded_data: (57896044618658097711785492504343953926640304052506563146031595460266534371336,), value: 0x0


Mon Aug 28 09:42:15 UTC 2023
