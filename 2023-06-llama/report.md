# LLAMA - Analysis results

## WARDEN REPORT

### HIGH

| Category                      | REF  | Name                                                                                                          | Wardens |        contract         |
|:------------------------------|:----:|:--------------------------------------------------------------------------------------------------------------|:-------:|:-----------------------:|
| Erroneus Account              | H-01 | In LlamaRelativeQuorum, the governance result might be incorrect as it counts the  wrong approval/disapproval |    5    | LlamaRelativeQuorum.sol |
| Inconsistent State Updates    | H-02 | Anyone can change approval/disapproval threshold for any action using LlamaRelativeQuorum strategy            |    3    | LlamaRelativeQuorum.sol |


### MEDIUM
| Category                                                                | REF  | Name                                                                              | Wardens |            contract             |
|:------------------------------------------------------------------------|:----:|:----------------------------------------------------------------------------------|:-------:|:-------------------------------:|
| Contract Implementation Specific Bugs (not payable implementation)      | M-01 | It is not possible to execute actions that require ETH (or other protocol token)  |   18    | LlamaCore.sol,LlamaExecutor.sol |
| Contract Implementation Specific Bugs (frontrun vulnerability)          | M-02 | User with disapproval role can gas grief the action executor                      |    2    |          LlamaCore.sol          |
| Contract Implementation Specific Bugs (DOS due to too much user action) | M-03 | LlamaPolicy could be DOS by creating large amount of actions                      |    7    |  LlamaPolicy.sol,LlamaCore.sol  |


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


|                                      | analysis duration (s) | analysis duration (m) | timeout (Y/N) |   High    | Medium | Low | valid finds |
|:------------------------------------:|:---------------------:|:---------------------:|:-------------:|:---------:|:------:|:---:|:-----------:|
|     LlamaAbsolutePeerReview.sol      |         5320          |          89           |       N       | 6 (6 IAB) |   0    |  4  |      0      |          
|       LlamaAbsoluteQuorum.sol        |         5299          |          88           |       N       |     0     |   0    |  4  |      0      |  
|           LlamaAccount.sol           |          614          |          10           |       N       | 1 (1 IAB) |   0    |  0  |      0      |       
|            LlamaCore.sol             |         4878          |          81           |       N       | 1 (1 IAB) |   0    |  0  |      0      |          
|          LlamaExecutor.sol           |          113          |           2           |       N       |     0     |   2    |  1  |      0      |          
|           LlamaFactory.sol           |           4           |           0           |       N       |     0     |   0    |  0  |      0      |   
|      LlamaGovernanceScript.sol       |          189          |           3           |       N       |     0     |   0    |  0  |      0      |
|           LlamaPolicy.sol            |           3           |           0           |       N       |     0     |   0    |  0  |      0      |          
|       LlamaPolicyMetadata.sol        |          68           |           1           |       N       |     0     |   0    |  0  |      0      |          
| LlamaPolicyMetadataParamRegistry.sol |          510          |           8           |       N       |     0     |   0    |  0  |      0      |          
|       LlamaRelativeQuorum.sol        |         11991         |          200          |       N       | 3 (3 IAB) |   0    |  4  |      0      |      


# BOT REPORT

## HIGH
No high in bot report

## MEDIUM
| C4 Severity | REF  | Name                                                                    |     contract     |
|:-----------:|:----:|:------------------------------------------------------------------------|:----------------:|
|   Medium    | M-01 | Some tokens may revert when zero value transfers are made               | LlamaAccount.sol |
|   Medium    | M-02 | ```_safeMint()``` should be used rather than _mint() wherever possible  | LlamaPolicy.sol  |

# COMPARISON

```Vulnerability found: Y``` means
1) Mythril found the vulnerability and describes vector attack, or
2) Mythril found a part of code and indicates enough information to lead to exploit/report vulnerability.

## COMPARISON BETWEEN MYTHRIL REPORT AND WARDEN REPORT

## HIGH
| REF  |        contract         | vulnerability found (Y/N) |
|:----:|:-----------------------:|:-------------------------:|
| H-01 | LlamaRelativeQuorum.sol |             N             |
| H-02 | LlamaRelativeQuorum.sol |             N             |

## MEDIUM
| REF  |            contract             | vulnerability found (Y/N) |
|:----:|:-------------------------------:|:-------------------------:|
| M-01 | LlamaCore.sol,LlamaExecutor.sol |             N             |
| M-02 |          LlamaCore.sol          |             N             |
| M-03 |  LlamaPolicy.sol,LlamaCore.sol  |             N             |



## COMPARISON BETWEEN MYTHRIL REPORT AND BOT REPORT

### MEDIUM
| REF  |     contract     | vulnerability found (Y/N) |
|:----:|:----------------:|:-------------------------:|
| M-01 | LlamaAccount.sol |             N             |
| M-02 | LlamaPolicy.sol  |             N             |



