Thu Aug  3 01:51:22 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for node_modules/@openzeppelin/contracts-upgradeable/security/ReentrancyGuardUpgradeable.sol

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
Caller: [CREATOR], function: markValidatorReadyToDeposit(bytes[],bytes[],bytes[]), txdata: 0x13797bff00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001c, decoded_data: ([], [], []), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: PermissionlessNodeRegistry
- Function name: `markValidatorReadyToDeposit(bytes[],bytes[],bytes[])`
- PC address: 29752
- Estimated Gas Usage: 1688 - 2254

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1027

### Code

```
sub(calldatasize(), mul(length, 0x01))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: updateVerifiedKeysBatchSize(uint256), txdata: 0xaf533aa8110191b511057fffffffffe00000000000030000000000000000000000000000, decoded_data: (7692090907743509899822863680468202377300330642961903351783879466127217131520,), value: 0x0
Caller: [ATTACKER], function: isExistingOperator(address), txdata: 0xf9c4dda40000000000000000000000000000000000000000000000000000000000000000b0, decoded_data: ('0x0000000000000000000000000000000000000000',), value: 0x0


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
Caller: [ATTACKER], function: validatorRegistry(uint256), txdata: 0x5a1239c1000000000000000000000000000000000000000000ffffffffffffffffffffd8, decoded_data: (309485009821345068724781016,), value: 0x0


Thu Aug  3 07:32:05 UTC 2023
