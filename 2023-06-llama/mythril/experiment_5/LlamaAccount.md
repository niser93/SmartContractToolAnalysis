Sun Sep 10 15:04:31 UTC 2023
STRATEGY: weighted-random
MAX-DEPTH: 1000
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


Sun Sep 10 15:14:45 UTC 2023
