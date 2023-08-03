Sun Jul 30 00:22:01 UTC 2023
# Analysis results for contracts/Auction.sol

## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: Auction
- Function name: `addBid(uint256)`
- PC address: 1636
- Estimated Gas Usage: 2285 - 2900

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/Auction.sol:67

### Code

```
if (block.number > lotItem.endBlock) revert AuctionEnded()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x1, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: addBid(uint256), txdata: 0x14b0e2660000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x1


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: Auction
- Function name: `extractNonBidSD(uint256)`
- PC address: 3306
- Estimated Gas Usage: 1324 - 1609

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/Auction.sol:108

### Code

```
if (block.number <= lotItem.endBlock) revert AuctionNotEnded()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: extractNonBidSD(uint256), txdata: 0x6f0625080000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: Auction
- Function name: `withdrawUnselectedBid(uint256)`
- PC address: 4805
- Estimated Gas Usage: 7229 - 27514

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/Auction.sol:122

### Code

```
if (block.number <= lotItem.endBlock) revert AuctionNotEnded()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [SOMEGUY], function: withdrawUnselectedBid(uint256), txdata: 0x883375190000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: Auction
- Function name: `transferHighestBidToSSPM(uint256)`
- PC address: 5787
- Estimated Gas Usage: 8001 - 28286

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/Auction.sol:97

### Code

```
if (block.number <= lotItem.endBlock) revert AuctionNotEnded()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: transferHighestBidToSSPM(uint256), txdata: 0xa62851e90000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: Auction
- Function name: `claimSD(uint256)`
- PC address: 6521
- Estimated Gas Usage: 1389 - 1674

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: contracts/Auction.sol:82

### Code

```
if (block.number <= lotItem.endBlock) revert AuctionNotEnded()
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: claimSD(uint256), txdata: 0xce93d8c60000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


## Dependence on predictable environment variable
- SWC ID: 120
- Severity: Low
- Contract: Auction
- Function name: `createLot(uint256)`
- PC address: 10802
- Estimated Gas Usage: 8212 - 28827

### Description

A control flow decision is made based on The block.number environment variable.
The block.number environment variable is used to determine a control flow decision. Note that the values of variables like coinbase, gaslimit, block number and timestamp are predictable and can be manipulated by a malicious miner. Also keep in mind that attackers know hashes of earlier blocks. Don't use any of those environment variables as sources of randomness and be aware that use of these variables introduces a certain level of trust into miners.
In file: #utility.yul:255

### Code

```
if gt(x, sum) { panic_error_0x11() }
```

### Initial State:

Account: [CREATOR], balance: 0x0, nonce:0, storage:{}
Account: [ATTACKER], balance: 0x0, nonce:0, storage:{}

### Transaction Sequence

Caller: [CREATOR], calldata: , decoded_data: , value: 0x0
Caller: [ATTACKER], function: createLot(uint256), txdata: 0x7a78e12d0000000000000000000000000000000000000000000000000000000000000000, decoded_data: (0,), value: 0x0


Sun Jul 30 00:43:42 UTC 2023
