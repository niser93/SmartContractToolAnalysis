Thu Aug  3 12:14:20 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
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
- Function name: `setMissedAttestationPenaltyUpdateFrequency(uint256)`
- PC address: 16318
- Estimated Gas Usage: 9666 - 65665

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
Caller: [ATTACKER], function: setMissedAttestationPenaltyUpdateFrequency(uint256), txdata: 0xf51c0fe70808050240062280800240418250140911241411115022020521121884300300, decoded_data: (3632672134578495834868411588155610130130076727576700291651402938231534125824,), value: 0x0
Caller: [CREATOR], function: setMissedAttestationPenaltyUpdateFrequency(uint256), txdata: 0xf51c0fe70808048080042040800108018040100801041001014020800420021080100102, decoded_data: (3632668636524589404183521217754548309995656703723128612739924634314583572738,), value: 0x0


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
Caller: [CREATOR], function: addTrustedNode(address), txdata: 0xd6275dd70000000000000000000000000000000000000000000100000000000000000000, decoded_data: ('0x0000000000000000000100000000000000000000',), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: StaderOracle
- Function name: `getMissedAttestationPenaltyReportableBlock()`
- PC address: 27081
- Estimated Gas Usage: 1552 - 1837

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
Caller: [SOMEGUY], function: setMissedAttestationPenaltyUpdateFrequency(uint256), txdata: 0xf51c0fe70002000000000000000000000000000000000002000000000000000000000000, decoded_data: (3533694129556768659166595001485837031654967952207562944771887589673140224,), value: 0x0
Caller: [ATTACKER], function: getMissedAttestationPenaltyReportableBlock(), txdata: 0xa71b3907, value: 0x0


Thu Aug  3 22:35:28 UTC 2023
