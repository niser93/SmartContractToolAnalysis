Sun Aug 27 11:37:37 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for src/lib/Checkpoints.sol

## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaPolicy
- Function name: `getPastQuantity(address,uint8,uint256)`
- PC address: 11248
- Estimated Gas Usage: 1181 - 1656

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: src/lib/Checkpoints.sol:38

### Code

```
require(timestamp < block.timestamp, "Checkpoints: timestamp is not in the past")
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: getPastQuantity(address,uint8,uint256), txdata: 0xcd8c321f000000000000000000000000010101200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ('0x0101012000000000000000000000000000000000', 0, 0), value: 0x0


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaPolicy
- Function name: `name()`
- PC address: 19241
- Estimated Gas Usage: 2641 - 3583

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:362

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: name(), txdata: 0x06fdde03, value: 0x0


Sun Aug 27 11:44:16 UTC 2023
