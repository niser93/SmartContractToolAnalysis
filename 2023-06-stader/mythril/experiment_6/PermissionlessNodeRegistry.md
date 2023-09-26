Fri Sep  8 05:50:39 UTC 2023
STRATEGY: pending
MAX-DEPTH: 500
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
Caller: [ATTACKER], function: markValidatorReadyToDeposit(bytes[],bytes[],bytes[]), txdata: 0x13797bff00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002a, decoded_data: ([], [], []), value: 0x0


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
Caller: [CREATOR], function: operatorStructById(uint256), txdata: 0xc8a00e7aa5f00000000000000000000000000000000000020000000000000000801fffc1, decoded_data: (75055663311785766320698477831559178552351515939434749666034360106099725565889,), value: 0x0


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
Caller: [SOMEGUY], function: validatorRegistry(uint256), txdata: 0x5a1239c1800000034c0224000a0000001fffffffffffffffffffffffffffffffffffffdb, decoded_data: (57896044707542552482341211290778996208883138556193434778501368510075142930395,), value: 0x0


Fri Sep  8 12:39:56 UTC 2023
