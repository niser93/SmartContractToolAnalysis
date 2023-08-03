# JUICEBOX - Analysis results

# WARDEN REPORT

## Medium

| C4 Severity | REF  | Name                                                                                                                              | Wardens |        contract        |
|:-----------:|:----:|:----------------------------------------------------------------------------------------------------------------------------------|:-------:|:----------------------:|
|   Medium    | M-01 | Delegate architecture forces users to set zero slippage                                                                           |    7    | JBXBuybackDelegate.sol |
|   Medium    | M-02 | Low Liquidity in Uniswap V3 Pool Can Lead to ETH Lockup in ```JBXBuybackDelegate``` Contract                                      |   12    | JBXBuybackDelegate.sol |
|   Medium    | M-03 | Funding cycles that use ```JBXBuybackDelegate``` as a redeem data source (or any derived class) will slash all redeemable tokens  |    3    | JBXBuybackDelegate.sol |

# MYTHRIL REPORT
|                        | analysis duration (s) | analysis duration (m) | timeout (Y/N) | High | Medium | Low | valid finds |
|:----------------------:|:---------------------:|:---------------------:|:-------------:|:----:|:------:|:---:|:-----------:|
| JBXBuybackDelegate.sol |         2578          |          43           |       N       |  0   |   0    |  0  |      0      |             

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







