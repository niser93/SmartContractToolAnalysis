# ASYMMETRY - Analysis results

# WARDEN REPORT

## High

| Category                              | REF  | Name                                                                                                                               | Wardens |       contract       |
|:--------------------------------------|:----:|:-----------------------------------------------------------------------------------------------------------------------------------|:-------:|:--------------------:|
| Precision Loss                        | H-01 | An attacker can manipulate the preDepositvePrice to steal from other users                                                         |   41    |      SafEth.sol      |
| Erroneus Account                      | H-02 | A temporary issue shows in the staking functionality which leads to the users receiving less minted tokens                         |   17    | SafEth.sol, Reth.sol |
| Inconsistent State Updates            | H-03 | Users can fail to unstake and lose their deserved ETH because malfunctioning or untrusted derivative cannot be removed             |   20    |      SafEth.sol      |
| Erroneus Account                      | H-04 | Price of sfrxEth derivative is calculated incorrectly                                                                              |   11    |      SafEth.sol      |
| Integer Bug (Integer Overflow)        | H-05 | Reth ```poolPrice``` calculation may overflow                                                                                      |    6    |       Reth.sol       |
| Contract Implementation Specific Bugs | H-06 | ```WstEth``` derivative assumes a ```~1=1``` peg of stETH to ETH                                                                   |   39    |      WstEth.sol      |
| Contract Implementation Specific Bugs | H-07 | ```Reth.sol```: Withdrawals are unreliable and depend on excess ```RocketDepositPool``` balance which can brick the whole protocol |   12    |       Reth.sol       |
| Atomicity Violations                  | H-08 | Staking, unstaking and rebalanceToWeight can be sandwiched (Mainly rETH deposit)                                                   |   74    |     SafEth.sol       |


## Medium

| Category                                                       | REF  | Name                                                                                                                                | Wardens |                   contract                    |
|:---------------------------------------------------------------|:----:|:------------------------------------------------------------------------------------------------------------------------------------|:-------:|:---------------------------------------------:|
| Precision Loss                                                 | M-01 | Division before multiplication truncate ```minOut``` and incurs heavy precision loss and result in insufficient slippage protection |   14    |             Reth.sol, SfrxEth.sol             |
| Erroneus Accoun                                                | M-02 | sFrxEth may revert on redeeming non-zero amount                                                                                     |    1    |            SafEth.sol, SfrxEth.sol            |
| Erroneus Accoun                                                | M-03 | Potential ```stake()``` DoS if sole safETH holder (ie: first depositor) unstakes ```totalSupply``` - 1                              |    2    |                  SafEth.sol                   |
| Contract Implementation Specific Bugs                          | M-04 | Lack of deadline for uniswap AMM                                                                                                    |   14    |                   Reth.sol                    |
| Contract Implementation Specific Bugs (using of Lido Protocol) | M-05 | Missing derivative limit and deposit availability checks will revert the whole stake() function                                     |   18    |       Reth.sol, SafEth.sol, WstEth.sol        |
| Contract Implementation Specific Bugs                          | M-06 | DoS due to external call failure                                                                                                    |   25    | Reth.sol, SafEth.sol, SfrxEth.sol, WstEth.sol |
| Contract Implementation Specific Bugs                          | M-07 | In de-peg scenario, forcing full exit from every derivative & immediately re-entering can cause big losses for depositors           |    8    |                  SafEth.sol                   |
| Contract Implementation Specific Bugs                          | M-08 | Possible DoS on ```unstake()```                                                                                                     |    3    |                   Reth.sol                    |
| Contract Implementation Specific Bugs                          | M-09 | Non-ideal rETH/WETH pool used pays unnecessary fees                                                                                 |    4    |                   Reth.sol                    |
| Erroneus Accoun                                                | M-10 | Stuck ether when use function ```stake``` with empty ```derivatives```(```derivativeCount``` = 0)                                   |   22    |                  SafEth.sol                   |
| Freezing Ether                                                 | M-11 | Residual ETH unreachable and unutilized in SafEth.sol                                                                               |   19    |                  SafEth.sol                   |
| Contract Implementation Specific Bugs                          | M-12 | No slippage protection on ```stake()``` in SafEth.sol                                                                               |   14    |                  SafEth.sol                   |

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
| experiment 1              | 460  |         8222          |          137          |               | 0 (0 IAB) |   0    |  3  |      0      |
| experiment 2              | 460  |         11401         |          190          |               | 0 (0 IAB) |   0    |  3  |      0      |
| experiment 3              | 460  |         8285          |          138          |               | 0 (0 IAB) |   0    |  3  |      0      |
| experiment 4              | 460  |         8850          |          148          |               | 0 (0 IAB) |   0    |  3  |      0      |
| experiment 5              | 460  |         8857          |          148          |               | 0 (0 IAB) |   0    |  3  |      0      |
| experiment 6              | 460  |         8364          |          139          |               | 0 (0 IAB) |   0    |  3  |      0      |
| Unique finds and averages | 460  |         8997          |          150          |               | 0 (0 IAB) |   0    |  3  |      0      |


# BOT REPORT
No high or medium in bot report

# COMPARISON

Vulnerability found: Y means
1) Mythril found the vulnerability and describes vector attack, or
2) Mythril found a part of code and indicates enough information to lead to exploit/report vulnerability.

## COMPARISON BETWEEN MYTHRIL REPORT AND WARDEN REPORT

## HIGH
| REF  |                    contract                    | vulnerability found (Y/N) |
|:----:|:----------------------------------------------:|:-------------------------:|
| H-01 |                   SafEth.sol                   |             N             |
| H-02 |              SafEth.sol, Reth.sol              |             N             |
| H-03 |                   SafEth.sol                   |             N             |
| H-04 |            SafEth.sol, SfrxEth.sol             |             N             |
| H-05 |                    Reth.sol                    |             N             |
| H-06 |                   WstEth.sol                   |             N             |
| H-07 |                    Reth.sol                    |             N             |
| H-08 | Reth.sol, SafEth.sol, SfrxEth.sol, WstEth.sol  |             N             |

## MEDIUM
| REF  |                   contract                    | vulnerability found (Y/N) |
|:----:|:---------------------------------------------:|:-------------------------:|
| M-01 |             Reth.sol, SfrxEth.sol             |             N             |
| M-02 |            SafEth.sol, SfrxEth.sol            |             N             |
| M-03 |                  SafEth.sol,                  |             N             |
| M-04 |                   Reth.sol,                   |             N             |
| M-05 |       Reth.sol, SafEth.sol, WstEth.sol        |             N             |
| M-06 | Reth.sol, SafEth.sol, SfrxEth.sol, WstEth.sol |             N             |
| M-07 |                  SafEth.sol                   |             N             |
| M-08 |                   Reth.sol,                   |             N             |
| M-09 |                   Reth.sol,                   |             N             |
| M-10 |                  SafEth.sol                   |             N             |
| M-11 |                  SafEth.sol                   |             N             |
| M-12 |                  SafEth.sol                   |             N             |


## COMPARISON BETWEEN MYTHRIL REPORT AND BOT REPORT
No high or medium in bot report







