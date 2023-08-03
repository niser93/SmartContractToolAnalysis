Mon Jul 31 13:27:40 UTC 2023
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
Caller: [ATTACKER], function: disableERInspectionMode(), txdata: 0xe10025e6, value: 0x0


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
Caller: [ATTACKER], function: addTrustedNode(address), txdata: 0xd6275dd70000000000000000000000000101010101010101010101018080010101010101, decoded_data: ('0x0101010101010101010101018080010101010101',), value: 0x0


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
Caller: [ATTACKER], function: setERUpdateFrequency(uint256), txdata: 0xd0a8f6790000000000000000000000000000000000000000000000000000000000000183, decoded_data: (387,), value: 0x0
Caller: [CREATOR], function: getERReportableBlock(), txdata: 0xb5c25ba6, value: 0x0


Tue Aug  1 00:26:18 UTC 2023
