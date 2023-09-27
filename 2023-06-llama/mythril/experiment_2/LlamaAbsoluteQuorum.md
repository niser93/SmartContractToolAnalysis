Mon Aug 28 03:38:48 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for src/strategies/LlamaAbsoluteStrategyBase.sol

## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaAbsoluteQuorum
- Function name: `isActive((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 5436
- Estimated Gas Usage: 5281 - 42385

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: src/strategies/LlamaAbsoluteStrategyBase.sol:268

### Code

```
block.timestamp <= approvalEndTime(actionInfo) && (isFixedLengthApprovalPeriod || !isActionApproved(actionInfo))
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: isActive((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xb0b061960000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000040', 32, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: LlamaAbsoluteQuorum
- Function name: `isActive((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 6161
- Estimated Gas Usage: 10952 - 85676

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: src/strategies/LlamaAbsoluteStrategyBase.sol:273

### Code

```
llamaCore.getAction(actionInfo.id)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: isActive((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xb0b061960000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 32, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaAbsoluteQuorum
- Function name: `minExecutionTime((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 7393
- Estimated Gas Usage: 1482 - 1907

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: src/lib/LlamaUtils.sol:11

### Code

```
if (n > type(uint64).max) revert UnsafeCast(n)
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [CREATOR], function: minExecutionTime((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xed93c1b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000000', 32, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 116
- Severity: Low
- Contract: LlamaAbsoluteQuorum
- Function name: `minExecutionTime((uint256,address,uint8,address,address,uint256,bytes))`
- PC address: 10765
- Estimated Gas Usage: 1416 - 1841

### Description

A control flow decision is made based on The block.timestamp environment variable.
The block.timestamp environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: #utility.yul:801

### Code

```
if gt(x, sum) { panic_error_0x11() }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: minExecutionTime((uint256,address,uint8,address,address,uint256,bytes)), txdata: 0xed93c1b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000, decoded_data: ([0, '0x0000000000000000000000000000000000000040', 64, '0x0000000000000000000000000000000000000000', '0x0000000000000000000000000000000000000000', 0, ''],), value: 0x0


Mon Aug 28 04:52:06 UTC 2023
