Tue Aug 29 18:50:18 UTC 2023
STRATEGY: bfs
MAX-DEPTH: 150
TIMEOUT: 86400
# Analysis results for #utility.yul

## Integer Arithmetic Bugs
- SWC ID: 101
- Severity: High
- Contract: LlamaAccount
- Function name: `name()`
- PC address: 13262
- Estimated Gas Usage: 2640 - 3582

### Description

The arithmetic operator can underflow.
It is possible to cause an integer overflow or underflow in the arithmetic operation.
In file: #utility.yul:854

### Code

```
eq(outOfPlaceEncoding, lt(length, 32))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: name(), txdata: 0x06fdde03, value: 0x0


Tue Aug 29 19:00:54 UTC 2023
