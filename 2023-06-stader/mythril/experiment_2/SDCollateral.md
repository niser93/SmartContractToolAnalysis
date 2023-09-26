Thu Aug  3 10:04:51 UTC 2023
STRATEGY: dfs
MAX-DEPTH: 200
TIMEOUT: 86400
# Analysis results for contracts/SDCollateral.sol

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: SDCollateral
- Function name: `convertSDToETH(uint256)`
- PC address: 4758
- Estimated Gas Usage: 6044 - 110766

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/SDCollateral.sol:206

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getSDPriceInETH()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: convertSDToETH(uint256), txdata: 0xdfdafccb0000000000000000000000000000000000000000000000000000000000000001, decoded_data: (1,), value: 0x0


## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: SDCollateral
- Function name: `convertETHToSD(uint256)`
- PC address: 5484
- Estimated Gas Usage: 6088 - 110810

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: contracts/SDCollateral.sol:211

### Code

```
IStaderOracle(staderConfig.getStaderOracle()).getSDPriceInETH()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: convertETHToSD(uint256), txdata: 0xe614e17c0000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


Thu Aug  3 10:57:58 UTC 2023
