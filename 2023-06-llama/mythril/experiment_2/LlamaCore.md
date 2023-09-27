Sun Aug 27 09:19:42 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaCore
- Function name: `name()`
- PC address: 21211
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


## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaCore
- Function name: `executeAction((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 21320
- Estimated Gas Usage: 1612 - 2508

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:362

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: authorizedScripts(address), txdata: 0x82c376180000000000000000000000000000000000000000000000000000000000000002, decoded_data: ('0x0000000000000000000000000000000000000002',), value: 0x0


Sun Aug 27 11:35:06 UTC 2023
