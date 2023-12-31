# JUICEBOX - Analysis results

# WARDEN REPORT

## Medium

| Category                              | REF  | Name                                                                                                                              | Wardens |        contract        |
|:--------------------------------------|:----:|:----------------------------------------------------------------------------------------------------------------------------------|:-------:|:----------------------:|
| Contract Implementation Specific Bugs | M-01 | Delegate architecture forces users to set zero slippage                                                                           |    7    | JBXBuybackDelegate.sol |
| Freezing Ether                        | M-02 | Low Liquidity in Uniswap V3 Pool Can Lead to ETH Lockup in ```JBXBuybackDelegate``` Contract                                      |   12    | JBXBuybackDelegate.sol |
| Erroneus Account                      | M-03 | Funding cycles that use ```JBXBuybackDelegate``` as a redeem data source (or any derived class) will slash all redeemable tokens  |    3    | JBXBuybackDelegate.sol |

# MYTHRIL REPORT

|              |    Strategy     | Max Depth | Timeout |                       Description file                       |
|:------------:|:---------------:|:---------:|:-------:|:------------------------------------------------------------:|
| experiment 1 |  standard(dfs)  |    22     |  86400  | [experiment_1/_description.md](experiment_1/_description.md) |
| experiment 2 |       dfs       |    200    |  86400  | [experiment_2/_description.md](experiment_2/_description.md) |
| experiment 3 |       bfs       |    150    |  86400  | [experiment_3/_description.md](experiment_3/_description.md) |
| experiment 4 |  naive-random   |    250    |  86400  | [experiment_4/_description.md](experiment_4/_description.md) |
| experiment 5 | weighted-random |   1000    |  86400  | [experiment_5/_description.md](experiment_5/_description.md) |
| experiment 6 |     pending     |    500    |  86400  | [experiment_6/_description.md](experiment_6/_description.md) |

|                           | SLOC | analysis duration (s) | analysis duration (m) | timeout (Y/N) |   High    | Medium | Low | valid finds |
|:--------------------------|:----:|:---------------------:|:---------------------:|:-------------:|:---------:|:------:|:---:|:-----------:|
| experiment 1              | 160  |         2578          |          43           |               | 0 (0 IAB) |   0    |  0  |      0      |
| experiment 2              | 160  |         3079          |          51           |               | 0 (0 IAB) |   0    |  0  |      0      |
| experiment 3              | 160  |         2613          |          44           |               | 0 (0 IAB) |   0    |  0  |      0      |
| experiment 4              | 160  |         2812          |          47           |               | 0 (0 IAB) |   0    |  0  |      0      |
| experiment 5              | 160  |         2191          |          37           |               | 0 (0 IAB) |   0    |  0  |      0      |
| experiment 6              | 160  |         2007          |          33           |               | 0 (0 IAB) |   0    |  0  |      0      |
| Unique finds and averages | 160  |         2547          |          43           |               | 0 (0 IAB) |   0    |  0  |      0      |

# BOT REPORT

## HIGH
No high in bot report

## MEDIUM
| C4 Severity | REF  | Name                                                                   |        contract        |
|:-----------:|:----:|:-----------------------------------------------------------------------|:----------------------:|
|   Medium    | M-01 | Fee-on-transfer/rebasing tokens will have problems when swapping       | JBXBuybackDelegate.sol |
|   Medium    | M-02 | Unsafe use of ```transfer()```/```transferFrom()``` with ```IERC20 ``` | JBXBuybackDelegate.sol |
|   Medium    | M-03 | Return values of ```transfer()```/```transferFrom()``` not checked     | JBXBuybackDelegate.sol |

# COMPARISON

Vulnerability found: Y means
1) Mythril found the vulnerability and describes vector attack, or
2) Mythril found a part of code and indicates enough information to lead to exploit/report vulnerability.

## COMPARISON BETWEEN MYTHRIL REPORT AND WARDEN REPORT

### MEDIUM
| REF  |        contract        | vulnerability found (Y/N) |
|:----:|:----------------------:|:-------------------------:|
| M-01 | JBXBuybackDelegate.sol |             N             |
| M-02 | JBXBuybackDelegate.sol |             N             |
| M-03 | JBXBuybackDelegate.sol |             N             |

## COMPARISON BETWEEN MYTHRIL REPORT AND BOT REPORT

### MEDIUM
| REF  |        contract        | vulnerability found (Y/N) |
|:----:|:----------------------:|:-------------------------:|
| M-01 | JBXBuybackDelegate.sol |             N             |
| M-02 | JBXBuybackDelegate.sol |             N             |
| M-03 | JBXBuybackDelegate.sol |             N             |







