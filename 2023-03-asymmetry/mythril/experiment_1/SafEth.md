Mon Jul 31 21:10:09 UTC 2023
STRATEGY: standard(dfs)
MAX-DEPTH: 22
TIMEOUT: 86400
# Analysis results for SafEth/SafEth.sol

## External Call To User-Supplied Address
- SWC ID: 107
- Severity: Low
- Contract: SafEth
- Function name: `unstake(uint256)`
- PC address: 2835
- Estimated Gas Usage: 19643 - 96086

### Description

A call to a user-supplied address is executed.
An external message call to an address specified by the caller is executed. Note that the callee account might contain arbitrary code and could re-enter any function within this contract. Reentering the contract in an intermediate state may lead to unexpected behaviour. Make sure that no state modifications are executed after this call and/or reentrancy guards are in place.
In file: SafEth/SafEth.sol:124

### Code

```
address(msg.sender).call{value: ethAmountToWithdraw}(
            ""
        )
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: unstake(uint256), txdata: 0x2e17de780000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


Mon Jul 31 23:21:21 UTC 2023
