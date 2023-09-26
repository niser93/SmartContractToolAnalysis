Sun Aug  6 14:52:50 UTC 2023
STRATEGY: bfs
MAX-DEPTH: 150
TIMEOUT: 86400
# Analysis results for contracts/StaderOracle.sol

## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: StaderOracle
- Function name: `disableERInspectionMode()`
- PC address: 12733
- Estimated Gas Usage: 4311 - 39723

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/StaderOracle.sol:186

### Code

```
if (
            !staderConfig.onlyManagerRole(msg.sender) &&
            erInspectionModeStartBlock + MAX_ER_UPDATE_FREQUENCY > block.number
        ) {
            revert CooldownNotComplete();
        }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: disableERInspectionMode(), txdata: 0xe10025e6, value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: StaderOracle
- Function name: `setWithdrawnValidatorsUpdateFrequency(uint256)`
- PC address: 16318
- Estimated Gas Usage: 9689 - 65688

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: contracts/StaderOracle.sol:563

### Code

```
_updateFrequency == updateFrequencyMap[_key]
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: setWithdrawnValidatorsUpdateFrequency(uint256), txdata: 0xc06a6201400204000a011201010202020221080140010180028001020201800101042020, decoded_data: (28951583611497556010818575393718730096118729291162822011178426852299019395104,), value: 0x0
Caller: [CREATOR], function: setWithdrawnValidatorsUpdateFrequency(uint256), txdata: 0xc06a62010000000008000000000000000000000000000000000000000000000000000000, decoded_data: (842498333348457493583344221469363458551160763204392890034487820288,), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: StaderOracle
- Function name: `addTrustedNode(address)`
- PC address: 26641
- Estimated Gas Usage: 16845 - 93409

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:1492

### Code

```
eq(value, 0xffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: addTrustedNode(address), txdata: 0xd6275dd70000000000000000000000000101010101010101010101010101010101010101, decoded_data: ('0x0101010101010101010101010101010101010101',), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: StaderOracle
- Function name: `getERReportableBlock()`
- PC address: 27081
- Estimated Gas Usage: 1485 - 1770

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: #utility.yul:1571

### Code

```
if and(iszero(iszero(x)), gt(y, div(0xffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff, x))) { panic_error_0x11() }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: setERUpdateFrequency(uint256), txdata: 0xd0a8f6790000000000000000000000000000000000000000000000000000000000000101, decoded_data: (257,), value: 0x0
Caller: [CREATOR], function: getERReportableBlock(), txdata: 0xb5c25ba6, value: 0x0


Mon Aug  7 01:40:06 UTC 2023
