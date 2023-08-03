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

|             | analysis duration (s) | analysis duration (m) | timeout (Y/N) | High | Medium | Low | valid finds |
|:-----------:|:---------------------:|:---------------------:|:-------------:|:----:|:------:|:---:|:-----------:|
|  Reth.sol   |          109          |           2           |       N       |  0   |   0    |  1  |      0      |
| SafEth.sol  |         7872          |          131          |       N       |  0   |   0    |  1  |      0      |
| SfrxEth.sol |          128          |           2           |       N       |  0   |   0    |  1  |      0      |
| WstEth.sol  |          113          |           2           |       N       |  0   |   0    |  0  |      0      |


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
| M-06 | Reth.sol, SafEth.sol, SfrxEth.sol, WstEth.sol |             Y             |
| M-07 |                  SafEth.sol                   |             N             |
| M-08 |                   Reth.sol,                   |             N             |
| M-09 |                   Reth.sol,                   |             N             |
| M-10 |                  SafEth.sol                   |             N             |
| M-11 |                  SafEth.sol                   |             N             |
| M-12 |                  SafEth.sol                   |             N             |


## COMPARISON BETWEEN MYTHRIL REPORT AND BOT REPORT
No high or medium in bot report







