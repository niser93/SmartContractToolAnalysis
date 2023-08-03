Mon Jul 31 18:56:58 UTC 2023
# Analysis results for SafEth/derivatives/SfrxEth.sol

## Multiple Calls in a Single Transaction
- SWC ID: 113
- Severity: Low
- Contract: SfrxEth
- Function name: `ethPerDerivative(uint256)`
- PC address: 1212
- Estimated Gas Usage: 3495 - 73090

### Description

Multiple calls are executed in the same transaction.
This call is executed following another call within the same transaction. It is possible that the call never gets executed if a prior call fails permanently. This might be caused intentionally by a malicious callee. If possible, refactor the code such that each transaction only executes one external call or make sure that all callees can be trusted (i.e. they’re part of your own codebase).
In file: SafEth/derivatives/SfrxEth.sol:116

### Code

```
IFrxEthEthPool(FRX_ETH_CRV_POOL_ADDRESS).price_oracle()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: ethPerDerivative(uint256), txdata: 0x2bd6de1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d1d, decoded_data: (13168512109341841832484543393144899324489527667857162184879489945997963762973,), value: 0x0


Mon Jul 31 18:59:06 UTC 2023
