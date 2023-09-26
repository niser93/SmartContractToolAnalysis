
# SMARTCHECK ANALYSIS

## SOLIDITY_ADDRESS_HARDCODED
The contract contains unknown address. This address might be used for some malicious activity. Please check hardcoded address and it's usage.


### Auction.sol

```

Auction.sol#1701
Severity: Low
1701             buffer[i] = _SYMBOLS[value & 0xf];



Auction.sol#1827
Severity: Low
1827     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### ETHx.sol

```

ETHx.sol#1994
Severity: Low
1994             buffer[i] = _SYMBOLS[value & 0xf];



ETHx.sol#2120
Severity: Low
2120     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



ETHx.sol#1376
Severity: Low
1376         _beforeTokenTransfer(address(0), account, amount);



ETHx.sol#1385
Severity: Low
1385         _afterTokenTransfer(address(0), account, amount);



ETHx.sol#1402
Severity: Low
1402         _beforeTokenTransfer(account, address(0), amount);



ETHx.sol#1414
Severity: Low
1414         _afterTokenTransfer(account, address(0), amount);



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#1509
Severity: Low
1509             buffer[i] = _SYMBOLS[value & 0xf];



OperatorRewardsCollector.sol#1635
Severity: Low
1635     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### Penalty.sol

```

Penalty.sol#1971
Severity: Low
1971             buffer[i] = _SYMBOLS[value & 0xf];



Penalty.sol#2097
Severity: Low
2097     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#2049
Severity: Low
2049             buffer[i] = _SYMBOLS[value & 0xf];



PermissionedNodeRegistry.sol#2175
Severity: Low
2175     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### PermissionedPool.sol

```

PermissionedPool.sol#1974
Severity: Low
1974             buffer[i] = _SYMBOLS[value & 0xf];



PermissionedPool.sol#2100
Severity: Low
2100     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#1881
Severity: Low
1881             buffer[i] = _SYMBOLS[value & 0xf];



PermissionlessNodeRegistry.sol#2007
Severity: Low
2007     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#1959
Severity: Low
1959             buffer[i] = _SYMBOLS[value & 0xf];



PermissionlessPool.sol#2085
Severity: Low
2085     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### PoolSelector.sol

```

PoolSelector.sol#1967
Severity: Low
1967             buffer[i] = _SYMBOLS[value & 0xf];



PoolSelector.sol#2093
Severity: Low
2093     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### PoolUtils.sol

```

PoolUtils.sol#1544
Severity: Low
1544             buffer[i] = _SYMBOLS[value & 0xf];



PoolUtils.sol#1670
Severity: Low
1670     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### SDCollateral.sol

```

SDCollateral.sol#2242
Severity: Low
2242             buffer[i] = _SYMBOLS[value & 0xf];



SDCollateral.sol#2368
Severity: Low
2368     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### SocializingPool.sol

```

SocializingPool.sol#1723
Severity: Low
1723             buffer[i] = _SYMBOLS[value & 0xf];



SocializingPool.sol#1849
Severity: Low
1849     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### StaderConfig.sol

```

StaderConfig.sol#1496
Severity: Low
1496             buffer[i] = _SYMBOLS[value & 0xf];



StaderConfig.sol#1622
Severity: Low
1622     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#1522
Severity: Low
1522             buffer[i] = _SYMBOLS[value & 0xf];



StaderInsuranceFund.sol#1648
Severity: Low
1648     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### StaderOracle.sol

```

StaderOracle.sol#2071
Severity: Low
2071             buffer[i] = _SYMBOLS[value & 0xf];



StaderOracle.sol#2197
Severity: Low
2197     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#1995
Severity: Low
1995             buffer[i] = _SYMBOLS[value & 0xf];



StaderStakePoolsManager.sol#2121
Severity: Low
2121     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



StaderStakePoolsManager.sol#1377
Severity: Low
1377         _beforeTokenTransfer(address(0), account, amount);



StaderStakePoolsManager.sol#1386
Severity: Low
1386         _afterTokenTransfer(address(0), account, amount);



StaderStakePoolsManager.sol#1403
Severity: Low
1403         _beforeTokenTransfer(account, address(0), amount);



StaderStakePoolsManager.sol#1415
Severity: Low
1415         _afterTokenTransfer(account, address(0), amount);



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#1994
Severity: Low
1994             buffer[i] = _SYMBOLS[value & 0xf];



UserWithdrawalManager.sol#2120
Severity: Low
2120     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



UserWithdrawalManager.sol#1376
Severity: Low
1376         _beforeTokenTransfer(address(0), account, amount);



UserWithdrawalManager.sol#1385
Severity: Low
1385         _afterTokenTransfer(address(0), account, amount);



UserWithdrawalManager.sol#1402
Severity: Low
1402         _beforeTokenTransfer(account, address(0), amount);



UserWithdrawalManager.sol#1414
Severity: Low
1414         _afterTokenTransfer(account, address(0), amount);



```

### VaultFactory.sol

```

VaultFactory.sol#1691
Severity: Low
1691             buffer[i] = _SYMBOLS[value & 0xf];



VaultFactory.sol#1817
Severity: Low
1817     bytes32 public constant DEFAULT_ADMIN_ROLE = 0x00;



VaultFactory.sol#2086
Severity: Low
2086         return abi.encodePacked(bytes1(0x01), bytes11(0x0), address(_withdrawVault));



VaultFactory.sol#2086
Severity: Low
2086         return abi.encodePacked(bytes1(0x01), bytes11(0x0), address(_withdrawVault));



```

## SOLIDITY_GAS_LIMIT_IN_LOOPS
Ethereum is a very resource-constrained environment. Prices per computational step are orders of magnitude higher than with centralized providers. Moreover, Ethereum miners impose a limit on the total number of gas consumed in a block. If ```array.length``` is large enough, the function exceeds the block gas limit, and transactions calling it will never be confirmed:

```
for (uint256 i = 0; i < array.length ; i++) {
cosltyFunc();
}
```

This becomes a security issue, if an external actor influences ```array.length```.
E.g., if array enumerates all registered addresses, an adversary can register many addresses, causing the problem described above.[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#gas-limitations)
Infinite loops


### Auction.sol

```

Auction.sol#1671
Severity: Low
1671             while (true) {



```

### ETHx.sol

```

ETHx.sol#1964
Severity: Low
1964             while (true) {



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#1479
Severity: Low
1479             while (true) {



```

### Penalty.sol

```

Penalty.sol#2459
Severity: Medium
2459         for (uint256 i; i < reportedValidatorCount; ) {



Penalty.sol#1941
Severity: Low
1941             while (true) {



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#2522
Severity: Medium
2522         for (uint256 i = 0; i < permissionedNosLength; i++) {



PermissionedNodeRegistry.sol#2019
Severity: Low
2019             while (true) {



```

### PermissionedPool.sol

```

PermissionedPool.sol#1944
Severity: Low
1944             while (true) {



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#1851
Severity: Low
1851             while (true) {



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#1929
Severity: Low
1929             while (true) {



```

### PoolSelector.sol

```

PoolSelector.sol#2368
Severity: Medium
2368         for (uint256 j; j < poolCount; ) {



PoolSelector.sol#2408
Severity: Medium
2408         for (uint256 i = 0; i < poolTargetLength; i++) {



PoolSelector.sol#1937
Severity: Low
1937             while (true) {



```

### PoolUtils.sol

```

PoolUtils.sol#1932
Severity: Medium
1932         for (uint256 i; i < exitValidatorCount; ) {



PoolUtils.sol#1514
Severity: Low
1514             while (true) {



```

### SDCollateral.sol

```

SDCollateral.sol#2212
Severity: Low
2212             while (true) {



```

### SocializingPool.sol

```

SocializingPool.sol#2292
Severity: Medium
2292         for (uint256 i = 0; i < proof.length; i++) {



SocializingPool.sol#2305
Severity: Medium
2305         for (uint256 i = 0; i < proof.length; i++) {



SocializingPool.sol#1693
Severity: Low
1693             while (true) {



```

### StaderConfig.sol

```

StaderConfig.sol#1466
Severity: Low
1466             while (true) {



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#1492
Severity: Low
1492             while (true) {



```

### StaderOracle.sol

```

StaderOracle.sol#2942
Severity: Medium
2942             for (uint256 i; i < keyCount; ) {



StaderOracle.sol#2041
Severity: Low
2041             while (true) {



StaderOracle.sol#2762
Severity: Low
2762         while ((j >= 1) && (_sdPrice < sdPrices[j - 1])) {



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#1965
Severity: Low
1965             while (true) {



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#1964
Severity: Low
1964             while (true) {



```

### VaultFactory.sol

```

VaultFactory.sol#1661
Severity: Low
1661             while (true) {



```

## SOLIDITY_MSGVALUE_EQUALS_ZERO
The ```msg.value == 0``` condition check is meaningless in most cases.


### Auction.sol

```

Auction.sol#2266
Severity: Low
2266         if (msg.value == 0) revert InSufficientETH();



```

## SOLIDITY_PRIVATE_MODIFIER_DONT_HIDE_DATA
Contrary to a popular misconception, the ```private``` modifier does not make a variable invisible. Miners have access to all contractsâ€™ code and data. Developers must account for the lack of privacy in Ethereum.

[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#privacy)

Privacy.


### Auction.sol

```

Auction.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



Auction.sol#1170
Severity: Low
1170     uint8 private _initialized;



Auction.sol#1175
Severity: Low
1175     bool private _initializing;



Auction.sol#1304
Severity: Low
1304     uint256[50] private __gap;



Auction.sol#1656
Severity: Low
1656     bytes16 private constant _SYMBOLS = "0123456789abcdef";



Auction.sol#1657
Severity: Low
1657     uint8 private constant _ADDRESS_LENGTH = 20;



Auction.sol#1773
Severity: Low
1773     uint256[50] private __gap;



Auction.sol#1825
Severity: Low
1825     mapping(bytes32 => RoleData) private _roles;



Auction.sol#2023
Severity: Low
2023     uint256[49] private __gap;



Auction.sol#2048
Severity: Low
2048     bool private _paused;



Auction.sol#2135
Severity: Low
2135     uint256[49] private __gap;



Auction.sol#2168
Severity: Low
2168     uint256 private constant _NOT_ENTERED = 1;



Auction.sol#2169
Severity: Low
2169     uint256 private constant _ENTERED = 2;



Auction.sol#2171
Severity: Low
2171     uint256 private _status;



Auction.sol#2213
Severity: Low
2213     uint256[49] private __gap;



```

### ETHx.sol

```

ETHx.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



ETHx.sol#983
Severity: Low
983     uint8 private _initialized;



ETHx.sol#988
Severity: Low
988     bool private _initializing;



ETHx.sol#1117
Severity: Low
1117     uint256[50] private __gap;



ETHx.sol#1146
Severity: Low
1146     mapping(address => uint256) private _balances;



ETHx.sol#1148
Severity: Low
1148     mapping(address => mapping(address => uint256)) private _allowances;



ETHx.sol#1150
Severity: Low
1150     uint256 private _totalSupply;



ETHx.sol#1152
Severity: Low
1152     string private _name;



ETHx.sol#1153
Severity: Low
1153     string private _symbol;



ETHx.sol#1509
Severity: Low
1509     uint256[45] private __gap;



ETHx.sol#1949
Severity: Low
1949     bytes16 private constant _SYMBOLS = "0123456789abcdef";



ETHx.sol#1950
Severity: Low
1950     uint8 private constant _ADDRESS_LENGTH = 20;



ETHx.sol#2066
Severity: Low
2066     uint256[50] private __gap;



ETHx.sol#2118
Severity: Low
2118     mapping(bytes32 => RoleData) private _roles;



ETHx.sol#2316
Severity: Low
2316     uint256[49] private __gap;



ETHx.sol#2341
Severity: Low
2341     bool private _paused;



ETHx.sol#2428
Severity: Low
2428     uint256[49] private __gap;



```

### NodeELRewardVault.sol

```

NodeELRewardVault.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



OperatorRewardsCollector.sol#978
Severity: Low
978     uint8 private _initialized;



OperatorRewardsCollector.sol#983
Severity: Low
983     bool private _initializing;



OperatorRewardsCollector.sol#1112
Severity: Low
1112     uint256[50] private __gap;



OperatorRewardsCollector.sol#1464
Severity: Low
1464     bytes16 private constant _SYMBOLS = "0123456789abcdef";



OperatorRewardsCollector.sol#1465
Severity: Low
1465     uint8 private constant _ADDRESS_LENGTH = 20;



OperatorRewardsCollector.sol#1581
Severity: Low
1581     uint256[50] private __gap;



OperatorRewardsCollector.sol#1633
Severity: Low
1633     mapping(bytes32 => RoleData) private _roles;



OperatorRewardsCollector.sol#1831
Severity: Low
1831     uint256[49] private __gap;



OperatorRewardsCollector.sol#1856
Severity: Low
1856     bool private _paused;



OperatorRewardsCollector.sol#1943
Severity: Low
1943     uint256[49] private __gap;



```

### Penalty.sol

```

Penalty.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



Penalty.sol#1440
Severity: Low
1440     uint8 private _initialized;



Penalty.sol#1445
Severity: Low
1445     bool private _initializing;



Penalty.sol#1574
Severity: Low
1574     uint256[50] private __gap;



Penalty.sol#1926
Severity: Low
1926     bytes16 private constant _SYMBOLS = "0123456789abcdef";



Penalty.sol#1927
Severity: Low
1927     uint8 private constant _ADDRESS_LENGTH = 20;



Penalty.sol#2043
Severity: Low
2043     uint256[50] private __gap;



Penalty.sol#2095
Severity: Low
2095     mapping(bytes32 => RoleData) private _roles;



Penalty.sol#2293
Severity: Low
2293     uint256[49] private __gap;



Penalty.sol#2326
Severity: Low
2326     uint256 private constant _NOT_ENTERED = 1;



Penalty.sol#2327
Severity: Low
2327     uint256 private constant _ENTERED = 2;



Penalty.sol#2329
Severity: Low
2329     uint256 private _status;



Penalty.sol#2371
Severity: Low
2371     uint256[49] private __gap;



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



PermissionedNodeRegistry.sol#1320
Severity: Low
1320     uint8 private _initialized;



PermissionedNodeRegistry.sol#1325
Severity: Low
1325     bool private _initializing;



PermissionedNodeRegistry.sol#1454
Severity: Low
1454     uint256[50] private __gap;



PermissionedNodeRegistry.sol#1477
Severity: Low
1477     bool private _paused;



PermissionedNodeRegistry.sol#1564
Severity: Low
1564     uint256[49] private __gap;



PermissionedNodeRegistry.sol#2004
Severity: Low
2004     bytes16 private constant _SYMBOLS = "0123456789abcdef";



PermissionedNodeRegistry.sol#2005
Severity: Low
2005     uint8 private constant _ADDRESS_LENGTH = 20;



PermissionedNodeRegistry.sol#2121
Severity: Low
2121     uint256[50] private __gap;



PermissionedNodeRegistry.sol#2173
Severity: Low
2173     mapping(bytes32 => RoleData) private _roles;



PermissionedNodeRegistry.sol#2371
Severity: Low
2371     uint256[49] private __gap;



PermissionedNodeRegistry.sol#2404
Severity: Low
2404     uint256 private constant _NOT_ENTERED = 1;



PermissionedNodeRegistry.sol#2405
Severity: Low
2405     uint256 private constant _ENTERED = 2;



PermissionedNodeRegistry.sol#2407
Severity: Low
2407     uint256 private _status;



PermissionedNodeRegistry.sol#2449
Severity: Low
2449     uint256[49] private __gap;



```

### PermissionedPool.sol

```

PermissionedPool.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



PermissionedPool.sol#1443
Severity: Low
1443     uint8 private _initialized;



PermissionedPool.sol#1448
Severity: Low
1448     bool private _initializing;



PermissionedPool.sol#1577
Severity: Low
1577     uint256[50] private __gap;



PermissionedPool.sol#1929
Severity: Low
1929     bytes16 private constant _SYMBOLS = "0123456789abcdef";



PermissionedPool.sol#1930
Severity: Low
1930     uint8 private constant _ADDRESS_LENGTH = 20;



PermissionedPool.sol#2046
Severity: Low
2046     uint256[50] private __gap;



PermissionedPool.sol#2098
Severity: Low
2098     mapping(bytes32 => RoleData) private _roles;



PermissionedPool.sol#2296
Severity: Low
2296     uint256[49] private __gap;



PermissionedPool.sol#2329
Severity: Low
2329     uint256 private constant _NOT_ENTERED = 1;



PermissionedPool.sol#2330
Severity: Low
2330     uint256 private constant _ENTERED = 2;



PermissionedPool.sol#2332
Severity: Low
2332     uint256 private _status;



PermissionedPool.sol#2374
Severity: Low
2374     uint256[49] private __gap;



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



PermissionlessNodeRegistry.sol#1152
Severity: Low
1152     uint8 private _initialized;



PermissionlessNodeRegistry.sol#1157
Severity: Low
1157     bool private _initializing;



PermissionlessNodeRegistry.sol#1286
Severity: Low
1286     uint256[50] private __gap;



PermissionlessNodeRegistry.sol#1309
Severity: Low
1309     bool private _paused;



PermissionlessNodeRegistry.sol#1396
Severity: Low
1396     uint256[49] private __gap;



PermissionlessNodeRegistry.sol#1836
Severity: Low
1836     bytes16 private constant _SYMBOLS = "0123456789abcdef";



PermissionlessNodeRegistry.sol#1837
Severity: Low
1837     uint8 private constant _ADDRESS_LENGTH = 20;



PermissionlessNodeRegistry.sol#1953
Severity: Low
1953     uint256[50] private __gap;



PermissionlessNodeRegistry.sol#2005
Severity: Low
2005     mapping(bytes32 => RoleData) private _roles;



PermissionlessNodeRegistry.sol#2203
Severity: Low
2203     uint256[49] private __gap;



PermissionlessNodeRegistry.sol#2236
Severity: Low
2236     uint256 private constant _NOT_ENTERED = 1;



PermissionlessNodeRegistry.sol#2237
Severity: Low
2237     uint256 private constant _ENTERED = 2;



PermissionlessNodeRegistry.sol#2239
Severity: Low
2239     uint256 private _status;



PermissionlessNodeRegistry.sol#2281
Severity: Low
2281     uint256[49] private __gap;



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



PermissionlessPool.sol#1428
Severity: Low
1428     uint8 private _initialized;



PermissionlessPool.sol#1433
Severity: Low
1433     bool private _initializing;



PermissionlessPool.sol#1562
Severity: Low
1562     uint256[50] private __gap;



PermissionlessPool.sol#1914
Severity: Low
1914     bytes16 private constant _SYMBOLS = "0123456789abcdef";



PermissionlessPool.sol#1915
Severity: Low
1915     uint8 private constant _ADDRESS_LENGTH = 20;



PermissionlessPool.sol#2031
Severity: Low
2031     uint256[50] private __gap;



PermissionlessPool.sol#2083
Severity: Low
2083     mapping(bytes32 => RoleData) private _roles;



PermissionlessPool.sol#2281
Severity: Low
2281     uint256[49] private __gap;



PermissionlessPool.sol#2314
Severity: Low
2314     uint256 private constant _NOT_ENTERED = 1;



PermissionlessPool.sol#2315
Severity: Low
2315     uint256 private constant _ENTERED = 2;



PermissionlessPool.sol#2317
Severity: Low
2317     uint256 private _status;



PermissionlessPool.sol#2359
Severity: Low
2359     uint256[49] private __gap;



```

### PoolSelector.sol

```

PoolSelector.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



PoolSelector.sol#1436
Severity: Low
1436     uint8 private _initialized;



PoolSelector.sol#1441
Severity: Low
1441     bool private _initializing;



PoolSelector.sol#1570
Severity: Low
1570     uint256[50] private __gap;



PoolSelector.sol#1922
Severity: Low
1922     bytes16 private constant _SYMBOLS = "0123456789abcdef";



PoolSelector.sol#1923
Severity: Low
1923     uint8 private constant _ADDRESS_LENGTH = 20;



PoolSelector.sol#2039
Severity: Low
2039     uint256[50] private __gap;



PoolSelector.sol#2091
Severity: Low
2091     mapping(bytes32 => RoleData) private _roles;



PoolSelector.sol#2289
Severity: Low
2289     uint256[49] private __gap;



```

### PoolUtils.sol

```

PoolUtils.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



PoolUtils.sol#1013
Severity: Low
1013     uint8 private _initialized;



PoolUtils.sol#1018
Severity: Low
1018     bool private _initializing;



PoolUtils.sol#1147
Severity: Low
1147     uint256[50] private __gap;



PoolUtils.sol#1499
Severity: Low
1499     bytes16 private constant _SYMBOLS = "0123456789abcdef";



PoolUtils.sol#1500
Severity: Low
1500     uint8 private constant _ADDRESS_LENGTH = 20;



PoolUtils.sol#1616
Severity: Low
1616     uint256[50] private __gap;



PoolUtils.sol#1668
Severity: Low
1668     mapping(bytes32 => RoleData) private _roles;



PoolUtils.sol#1866
Severity: Low
1866     uint256[49] private __gap;



PoolUtils.sol#1870
Severity: Low
1870     uint64 private constant PUBKEY_LENGTH = 48;



PoolUtils.sol#1871
Severity: Low
1871     uint64 private constant SIGNATURE_LENGTH = 96;



```

### SDCollateral.sol

```

SDCollateral.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



SDCollateral.sol#1711
Severity: Low
1711     uint8 private _initialized;



SDCollateral.sol#1716
Severity: Low
1716     bool private _initializing;



SDCollateral.sol#1845
Severity: Low
1845     uint256[50] private __gap;



SDCollateral.sol#2197
Severity: Low
2197     bytes16 private constant _SYMBOLS = "0123456789abcdef";



SDCollateral.sol#2198
Severity: Low
2198     uint8 private constant _ADDRESS_LENGTH = 20;



SDCollateral.sol#2314
Severity: Low
2314     uint256[50] private __gap;



SDCollateral.sol#2366
Severity: Low
2366     mapping(bytes32 => RoleData) private _roles;



SDCollateral.sol#2564
Severity: Low
2564     uint256[49] private __gap;



SDCollateral.sol#2597
Severity: Low
2597     uint256 private constant _NOT_ENTERED = 1;



SDCollateral.sol#2598
Severity: Low
2598     uint256 private constant _ENTERED = 2;



SDCollateral.sol#2600
Severity: Low
2600     uint256 private _status;



SDCollateral.sol#2642
Severity: Low
2642     uint256[49] private __gap;



```

### SocializingPool.sol

```

SocializingPool.sol#446
Severity: Low
446     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



SocializingPool.sol#1192
Severity: Low
1192     uint8 private _initialized;



SocializingPool.sol#1197
Severity: Low
1197     bool private _initializing;



SocializingPool.sol#1326
Severity: Low
1326     uint256[50] private __gap;



SocializingPool.sol#1678
Severity: Low
1678     bytes16 private constant _SYMBOLS = "0123456789abcdef";



SocializingPool.sol#1679
Severity: Low
1679     uint8 private constant _ADDRESS_LENGTH = 20;



SocializingPool.sol#1795
Severity: Low
1795     uint256[50] private __gap;



SocializingPool.sol#1847
Severity: Low
1847     mapping(bytes32 => RoleData) private _roles;



SocializingPool.sol#2045
Severity: Low
2045     uint256[49] private __gap;



SocializingPool.sol#2070
Severity: Low
2070     bool private _paused;



SocializingPool.sol#2157
Severity: Low
2157     uint256[49] private __gap;



SocializingPool.sol#2190
Severity: Low
2190     uint256 private constant _NOT_ENTERED = 1;



SocializingPool.sol#2191
Severity: Low
2191     uint256 private constant _ENTERED = 2;



SocializingPool.sol#2193
Severity: Low
2193     uint256 private _status;



SocializingPool.sol#2235
Severity: Low
2235     uint256[49] private __gap;



```

### StaderConfig.sol

```

StaderConfig.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



StaderConfig.sol#965
Severity: Low
965     uint8 private _initialized;



StaderConfig.sol#970
Severity: Low
970     bool private _initializing;



StaderConfig.sol#1099
Severity: Low
1099     uint256[50] private __gap;



StaderConfig.sol#1451
Severity: Low
1451     bytes16 private constant _SYMBOLS = "0123456789abcdef";



StaderConfig.sol#1452
Severity: Low
1452     uint8 private constant _ADDRESS_LENGTH = 20;



StaderConfig.sol#1568
Severity: Low
1568     uint256[50] private __gap;



StaderConfig.sol#1620
Severity: Low
1620     mapping(bytes32 => RoleData) private _roles;



StaderConfig.sol#1818
Severity: Low
1818     uint256[49] private __gap;



StaderConfig.sol#1885
Severity: Low
1885     mapping(bytes32 => uint256) private constantsMap;



StaderConfig.sol#1886
Severity: Low
1886     mapping(bytes32 => uint256) private variablesMap;



StaderConfig.sol#1887
Severity: Low
1887     mapping(bytes32 => address) private accountsMap;



StaderConfig.sol#1888
Severity: Low
1888     mapping(bytes32 => address) private contractsMap;



StaderConfig.sol#1889
Severity: Low
1889     mapping(bytes32 => address) private tokensMap;



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



StaderInsuranceFund.sol#991
Severity: Low
991     uint8 private _initialized;



StaderInsuranceFund.sol#996
Severity: Low
996     bool private _initializing;



StaderInsuranceFund.sol#1125
Severity: Low
1125     uint256[50] private __gap;



StaderInsuranceFund.sol#1477
Severity: Low
1477     bytes16 private constant _SYMBOLS = "0123456789abcdef";



StaderInsuranceFund.sol#1478
Severity: Low
1478     uint8 private constant _ADDRESS_LENGTH = 20;



StaderInsuranceFund.sol#1594
Severity: Low
1594     uint256[50] private __gap;



StaderInsuranceFund.sol#1646
Severity: Low
1646     mapping(bytes32 => RoleData) private _roles;



StaderInsuranceFund.sol#1844
Severity: Low
1844     uint256[49] private __gap;



StaderInsuranceFund.sol#1877
Severity: Low
1877     uint256 private constant _NOT_ENTERED = 1;



StaderInsuranceFund.sol#1878
Severity: Low
1878     uint256 private constant _ENTERED = 2;



StaderInsuranceFund.sol#1880
Severity: Low
1880     uint256 private _status;



StaderInsuranceFund.sol#1922
Severity: Low
1922     uint256[49] private __gap;



```

### StaderOracle.sol

```

StaderOracle.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



StaderOracle.sol#1342
Severity: Low
1342     uint8 private _initialized;



StaderOracle.sol#1347
Severity: Low
1347     bool private _initializing;



StaderOracle.sol#1476
Severity: Low
1476     uint256[50] private __gap;



StaderOracle.sol#1499
Severity: Low
1499     bool private _paused;



StaderOracle.sol#1586
Severity: Low
1586     uint256[49] private __gap;



StaderOracle.sol#2026
Severity: Low
2026     bytes16 private constant _SYMBOLS = "0123456789abcdef";



StaderOracle.sol#2027
Severity: Low
2027     uint8 private constant _ADDRESS_LENGTH = 20;



StaderOracle.sol#2143
Severity: Low
2143     uint256[50] private __gap;



StaderOracle.sol#2195
Severity: Low
2195     mapping(bytes32 => RoleData) private _roles;



StaderOracle.sol#2393
Severity: Low
2393     uint256[49] private __gap;



StaderOracle.sol#2426
Severity: Low
2426     uint256 private constant _NOT_ENTERED = 1;



StaderOracle.sol#2427
Severity: Low
2427     uint256 private constant _ENTERED = 2;



StaderOracle.sol#2429
Severity: Low
2429     uint256 private _status;



StaderOracle.sol#2471
Severity: Low
2471     uint256[49] private __gap;



StaderOracle.sol#2502
Severity: Low
2502     mapping(bytes32 => bool) private nodeSubmissionKeys;



StaderOracle.sol#2503
Severity: Low
2503     mapping(bytes32 => uint8) private submissionCountKeys;



StaderOracle.sol#2505
Severity: Low
2505     uint256[] private sdPrices;



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#446
Severity: Low
446     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



StaderStakePoolsManager.sol#984
Severity: Low
984     uint8 private _initialized;



StaderStakePoolsManager.sol#989
Severity: Low
989     bool private _initializing;



StaderStakePoolsManager.sol#1118
Severity: Low
1118     uint256[50] private __gap;



StaderStakePoolsManager.sol#1147
Severity: Low
1147     mapping(address => uint256) private _balances;



StaderStakePoolsManager.sol#1149
Severity: Low
1149     mapping(address => mapping(address => uint256)) private _allowances;



StaderStakePoolsManager.sol#1151
Severity: Low
1151     uint256 private _totalSupply;



StaderStakePoolsManager.sol#1153
Severity: Low
1153     string private _name;



StaderStakePoolsManager.sol#1154
Severity: Low
1154     string private _symbol;



StaderStakePoolsManager.sol#1510
Severity: Low
1510     uint256[45] private __gap;



StaderStakePoolsManager.sol#1950
Severity: Low
1950     bytes16 private constant _SYMBOLS = "0123456789abcdef";



StaderStakePoolsManager.sol#1951
Severity: Low
1951     uint8 private constant _ADDRESS_LENGTH = 20;



StaderStakePoolsManager.sol#2067
Severity: Low
2067     uint256[50] private __gap;



StaderStakePoolsManager.sol#2119
Severity: Low
2119     mapping(bytes32 => RoleData) private _roles;



StaderStakePoolsManager.sol#2317
Severity: Low
2317     uint256[49] private __gap;



StaderStakePoolsManager.sol#2342
Severity: Low
2342     bool private _paused;



StaderStakePoolsManager.sol#2429
Severity: Low
2429     uint256[49] private __gap;



StaderStakePoolsManager.sol#3564
Severity: Low
3564     uint256 private constant _NOT_ENTERED = 1;



StaderStakePoolsManager.sol#3565
Severity: Low
3565     uint256 private constant _ENTERED = 2;



StaderStakePoolsManager.sol#3567
Severity: Low
3567     uint256 private _status;



StaderStakePoolsManager.sol#3609
Severity: Low
3609     uint256[49] private __gap;



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



UserWithdrawalManager.sol#983
Severity: Low
983     uint8 private _initialized;



UserWithdrawalManager.sol#988
Severity: Low
988     bool private _initializing;



UserWithdrawalManager.sol#1117
Severity: Low
1117     uint256[50] private __gap;



UserWithdrawalManager.sol#1146
Severity: Low
1146     mapping(address => uint256) private _balances;



UserWithdrawalManager.sol#1148
Severity: Low
1148     mapping(address => mapping(address => uint256)) private _allowances;



UserWithdrawalManager.sol#1150
Severity: Low
1150     uint256 private _totalSupply;



UserWithdrawalManager.sol#1152
Severity: Low
1152     string private _name;



UserWithdrawalManager.sol#1153
Severity: Low
1153     string private _symbol;



UserWithdrawalManager.sol#1509
Severity: Low
1509     uint256[45] private __gap;



UserWithdrawalManager.sol#1949
Severity: Low
1949     bytes16 private constant _SYMBOLS = "0123456789abcdef";



UserWithdrawalManager.sol#1950
Severity: Low
1950     uint8 private constant _ADDRESS_LENGTH = 20;



UserWithdrawalManager.sol#2066
Severity: Low
2066     uint256[50] private __gap;



UserWithdrawalManager.sol#2118
Severity: Low
2118     mapping(bytes32 => RoleData) private _roles;



UserWithdrawalManager.sol#2316
Severity: Low
2316     uint256[49] private __gap;



UserWithdrawalManager.sol#2341
Severity: Low
2341     bool private _paused;



UserWithdrawalManager.sol#2428
Severity: Low
2428     uint256[49] private __gap;



UserWithdrawalManager.sol#3436
Severity: Low
3436     uint256 private constant _NOT_ENTERED = 1;



UserWithdrawalManager.sol#3437
Severity: Low
3437     uint256 private constant _ENTERED = 2;



UserWithdrawalManager.sol#3439
Severity: Low
3439     uint256 private _status;



UserWithdrawalManager.sol#3481
Severity: Low
3481     uint256[49] private __gap;



```

### UtilLib.sol

```

UtilLib.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



```

### VaultFactory.sol

```

VaultFactory.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



VaultFactory.sol#1160
Severity: Low
1160     uint8 private _initialized;



VaultFactory.sol#1165
Severity: Low
1165     bool private _initializing;



VaultFactory.sol#1294
Severity: Low
1294     uint256[50] private __gap;



VaultFactory.sol#1646
Severity: Low
1646     bytes16 private constant _SYMBOLS = "0123456789abcdef";



VaultFactory.sol#1647
Severity: Low
1647     uint8 private constant _ADDRESS_LENGTH = 20;



VaultFactory.sol#1763
Severity: Low
1763     uint256[50] private __gap;



VaultFactory.sol#1815
Severity: Low
1815     mapping(bytes32 => RoleData) private _roles;



VaultFactory.sol#2013
Severity: Low
2013     uint256[49] private __gap;



```

### VaultProxy.sol

```

VaultProxy.sol#445
Severity: Low
445     uint64 private constant VALIDATOR_PUBKEY_LENGTH = 48;



```

## SOLIDITY_SHOULD_NOT_BE_PURE
In Solidity, function that do not read from the state or modify it can be declared as ```pure```.


### Auction.sol

```

Auction.sol#1360
Severity: Low
1360     function mulDiv(



Auction.sol#1662
Severity: Low
1662     function toString(uint256 value) internal pure returns (string memory) {



```

### ETHx.sol

```

ETHx.sol#1653
Severity: Low
1653     function mulDiv(



ETHx.sol#1955
Severity: Low
1955     function toString(uint256 value) internal pure returns (string memory) {



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#1168
Severity: Low
1168     function mulDiv(



OperatorRewardsCollector.sol#1470
Severity: Low
1470     function toString(uint256 value) internal pure returns (string memory) {



```

### Penalty.sol

```

Penalty.sol#1630
Severity: Low
1630     function mulDiv(



Penalty.sol#1932
Severity: Low
1932     function toString(uint256 value) internal pure returns (string memory) {



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#870
Severity: Low
870     function mulDiv(



PermissionedNodeRegistry.sol#1708
Severity: Low
1708     function mulDiv(



PermissionedNodeRegistry.sol#2010
Severity: Low
2010     function toString(uint256 value) internal pure returns (string memory) {



```

### PermissionedPool.sol

```

PermissionedPool.sol#907
Severity: Low
907     function mulDiv(



PermissionedPool.sol#1633
Severity: Low
1633     function mulDiv(



PermissionedPool.sol#1935
Severity: Low
1935     function toString(uint256 value) internal pure returns (string memory) {



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#1540
Severity: Low
1540     function mulDiv(



PermissionlessNodeRegistry.sol#1842
Severity: Low
1842     function toString(uint256 value) internal pure returns (string memory) {



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#892
Severity: Low
892     function mulDiv(



PermissionlessPool.sol#1618
Severity: Low
1618     function mulDiv(



PermissionlessPool.sol#1920
Severity: Low
1920     function toString(uint256 value) internal pure returns (string memory) {



```

### PoolSelector.sol

```

PoolSelector.sol#675
Severity: Low
675     function mulDiv(



PoolSelector.sol#1626
Severity: Low
1626     function mulDiv(



PoolSelector.sol#1928
Severity: Low
1928     function toString(uint256 value) internal pure returns (string memory) {



```

### PoolUtils.sol

```

PoolUtils.sol#1203
Severity: Low
1203     function mulDiv(



PoolUtils.sol#1505
Severity: Low
1505     function toString(uint256 value) internal pure returns (string memory) {



```

### SDCollateral.sol

```

SDCollateral.sol#1175
Severity: Low
1175     function mulDiv(



SDCollateral.sol#1901
Severity: Low
1901     function mulDiv(



SDCollateral.sol#2203
Severity: Low
2203     function toString(uint256 value) internal pure returns (string memory) {



```

### SocializingPool.sol

```

SocializingPool.sol#1382
Severity: Low
1382     function mulDiv(



SocializingPool.sol#1684
Severity: Low
1684     function toString(uint256 value) internal pure returns (string memory) {



```

### StaderConfig.sol

```

StaderConfig.sol#1155
Severity: Low
1155     function mulDiv(



StaderConfig.sol#1457
Severity: Low
1457     function toString(uint256 value) internal pure returns (string memory) {



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#1181
Severity: Low
1181     function mulDiv(



StaderInsuranceFund.sol#1483
Severity: Low
1483     function toString(uint256 value) internal pure returns (string memory) {



```

### StaderOracle.sol

```

StaderOracle.sol#1730
Severity: Low
1730     function mulDiv(



StaderOracle.sol#2032
Severity: Low
2032     function toString(uint256 value) internal pure returns (string memory) {



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#1654
Severity: Low
1654     function mulDiv(



StaderStakePoolsManager.sol#1956
Severity: Low
1956     function toString(uint256 value) internal pure returns (string memory) {



StaderStakePoolsManager.sol#3136
Severity: Low
3136     function mulDiv(



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#1653
Severity: Low
1653     function mulDiv(



UserWithdrawalManager.sol#1955
Severity: Low
1955     function toString(uint256 value) internal pure returns (string memory) {



UserWithdrawalManager.sol#3065
Severity: Low
3065     function mulDiv(



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#996
Severity: Low
996     function mulDiv(



```

### VaultFactory.sol

```

VaultFactory.sol#767
Severity: Low
767     function predictDeterministicAddress(



VaultFactory.sol#1350
Severity: Low
1350     function mulDiv(



VaultFactory.sol#1652
Severity: Low
1652     function toString(uint256 value) internal pure returns (string memory) {



```

## SOLIDITY_SHOULD_RETURN_STRUCT
Consider using struct instead of multiple return values for ```internal``` or ```private``` functions. It can improve code readability.


### Auction.sol

```

Auction.sol#238
Severity: Low
238         returns (



Auction.sol#253
Severity: Low
253         returns (



Auction.sol#402
Severity: Low
402         returns (



```

### ETHx.sol

```

ETHx.sol#238
Severity: Low
238         returns (



ETHx.sol#253
Severity: Low
253         returns (



ETHx.sol#402
Severity: Low
402         returns (



```

### NodeELRewardVault.sol

```

NodeELRewardVault.sol#238
Severity: Low
238         returns (



NodeELRewardVault.sol#253
Severity: Low
253         returns (



NodeELRewardVault.sol#402
Severity: Low
402         returns (



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#238
Severity: Low
238         returns (



OperatorRewardsCollector.sol#253
Severity: Low
253         returns (



OperatorRewardsCollector.sol#402
Severity: Low
402         returns (



```

### Penalty.sol

```

Penalty.sol#238
Severity: Low
238         returns (



Penalty.sol#253
Severity: Low
253         returns (



Penalty.sol#402
Severity: Low
402         returns (



Penalty.sol#787
Severity: Low
787         returns (



Penalty.sol#793
Severity: Low
793     function getRewardCycleDetails(uint256 _index) external view returns (uint256 _startBlock, uint256 _endBlock);



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#238
Severity: Low
238         returns (



PermissionedNodeRegistry.sol#253
Severity: Low
253         returns (



PermissionedNodeRegistry.sol#402
Severity: Low
402         returns (



PermissionedNodeRegistry.sol#665
Severity: Low
665         returns (



```

### PermissionedPool.sol

```

PermissionedPool.sol#238
Severity: Low
238         returns (



PermissionedPool.sol#253
Severity: Low
253         returns (



PermissionedPool.sol#402
Severity: Low
402         returns (



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#238
Severity: Low
238         returns (



PermissionlessNodeRegistry.sol#253
Severity: Low
253         returns (



PermissionlessNodeRegistry.sol#402
Severity: Low
402         returns (



PermissionlessNodeRegistry.sol#705
Severity: Low
705         returns (



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#238
Severity: Low
238         returns (



PermissionlessPool.sol#253
Severity: Low
253         returns (



PermissionlessPool.sol#402
Severity: Low
402         returns (



```

### PoolSelector.sol

```

PoolSelector.sol#238
Severity: Low
238         returns (



PoolSelector.sol#253
Severity: Low
253         returns (



PoolSelector.sol#402
Severity: Low
402         returns (



PoolSelector.sol#621
Severity: Low
621     function poolAllocationForExcessETHDeposit(uint256 _excessETH) external returns (uint256[] memory, uint8[] memory);



PoolSelector.sol#866
Severity: Low
866     function tryAdd(uint256 a, uint256 b) internal pure returns (bool, uint256) {



PoolSelector.sol#879
Severity: Low
879     function trySub(uint256 a, uint256 b) internal pure returns (bool, uint256) {



PoolSelector.sol#891
Severity: Low
891     function tryMul(uint256 a, uint256 b) internal pure returns (bool, uint256) {



PoolSelector.sol#908
Severity: Low
908     function tryDiv(uint256 a, uint256 b) internal pure returns (bool, uint256) {



PoolSelector.sol#920
Severity: Low
920     function tryMod(uint256 a, uint256 b) internal pure returns (bool, uint256) {



PoolSelector.sol#2357
Severity: Low
2357         returns (uint256[] memory selectedPoolCapacity, uint8[] memory poolIdArray)



```

### PoolUtils.sol

```

PoolUtils.sol#238
Severity: Low
238         returns (



PoolUtils.sol#253
Severity: Low
253         returns (



PoolUtils.sol#402
Severity: Low
402         returns (



```

### SDCollateral.sol

```

SDCollateral.sol#238
Severity: Low
238         returns (



SDCollateral.sol#253
Severity: Low
253         returns (



SDCollateral.sol#402
Severity: Low
402         returns (



SDCollateral.sol#834
Severity: Low
834         returns (



SDCollateral.sol#840
Severity: Low
840     function getRewardCycleDetails(uint256 _index) external view returns (uint256 _startBlock, uint256 _endBlock);



SDCollateral.sol#2922
Severity: Low
2922         returns (



```

### SocializingPool.sol

```

SocializingPool.sol#239
Severity: Low
239         returns (



SocializingPool.sol#254
Severity: Low
254         returns (



SocializingPool.sol#403
Severity: Low
403         returns (



SocializingPool.sol#690
Severity: Low
690         returns (



SocializingPool.sol#696
Severity: Low
696     function getRewardCycleDetails(uint256 _index) external view returns (uint256 _startBlock, uint256 _endBlock);



```

### StaderConfig.sol

```

StaderConfig.sol#238
Severity: Low
238         returns (



StaderConfig.sol#253
Severity: Low
253         returns (



StaderConfig.sol#402
Severity: Low
402         returns (



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#238
Severity: Low
238         returns (



StaderInsuranceFund.sol#253
Severity: Low
253         returns (



StaderInsuranceFund.sol#402
Severity: Low
402         returns (



```

### StaderOracle.sol

```

StaderOracle.sol#238
Severity: Low
238         returns (



StaderOracle.sol#253
Severity: Low
253         returns (



StaderOracle.sol#402
Severity: Low
402         returns (



StaderOracle.sol#689
Severity: Low
689         returns (



StaderOracle.sol#695
Severity: Low
695     function getRewardCycleDetails(uint256 _index) external view returns (uint256 _startBlock, uint256 _endBlock);



StaderOracle.sol#1045
Severity: Low
1045     returns (



StaderOracle.sol#1056
Severity: Low
1056     returns (



StaderOracle.sol#3097
Severity: Low
3097         returns (



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#239
Severity: Low
239         returns (



StaderStakePoolsManager.sol#254
Severity: Low
254         returns (



StaderStakePoolsManager.sol#403
Severity: Low
403         returns (



StaderStakePoolsManager.sol#2532
Severity: Low
2532     function poolAllocationForExcessETHDeposit(uint256 _excessETH) external returns (uint256[] memory, uint8[] memory);



StaderStakePoolsManager.sol#2622
Severity: Low
2622         returns (



StaderStakePoolsManager.sol#2628
Severity: Low
2628     function getRewardCycleDetails(uint256 _index) external view returns (uint256 _startBlock, uint256 _endBlock);



StaderStakePoolsManager.sol#3327
Severity: Low
3327     function tryAdd(uint256 a, uint256 b) internal pure returns (bool, uint256) {



StaderStakePoolsManager.sol#3340
Severity: Low
3340     function trySub(uint256 a, uint256 b) internal pure returns (bool, uint256) {



StaderStakePoolsManager.sol#3352
Severity: Low
3352     function tryMul(uint256 a, uint256 b) internal pure returns (bool, uint256) {



StaderStakePoolsManager.sol#3369
Severity: Low
3369     function tryDiv(uint256 a, uint256 b) internal pure returns (bool, uint256) {



StaderStakePoolsManager.sol#3381
Severity: Low
3381     function tryMod(uint256 a, uint256 b) internal pure returns (bool, uint256) {



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#238
Severity: Low
238         returns (



UserWithdrawalManager.sol#253
Severity: Low
253         returns (



UserWithdrawalManager.sol#402
Severity: Low
402         returns (



UserWithdrawalManager.sol#2599
Severity: Low
2599         returns (



UserWithdrawalManager.sol#2605
Severity: Low
2605     function getRewardCycleDetails(uint256 _index) external view returns (uint256 _startBlock, uint256 _endBlock);



```

### UtilLib.sol

```

UtilLib.sol#238
Severity: Low
238         returns (



UtilLib.sol#253
Severity: Low
253         returns (



UtilLib.sol#402
Severity: Low
402         returns (



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#238
Severity: Low
238         returns (



ValidatorWithdrawalVault.sol#253
Severity: Low
253         returns (



ValidatorWithdrawalVault.sol#402
Severity: Low
402         returns (



ValidatorWithdrawalVault.sol#849
Severity: Low
849         returns (



```

### VaultFactory.sol

```

VaultFactory.sol#238
Severity: Low
238         returns (



VaultFactory.sol#253
Severity: Low
253         returns (



VaultFactory.sol#402
Severity: Low
402         returns (



```

### VaultProxy.sol

```

VaultProxy.sol#238
Severity: Low
238         returns (



VaultProxy.sol#253
Severity: Low
253         returns (



VaultProxy.sol#402
Severity: Low
402         returns (



```

## SOLIDITY_UPGRADE_TO_050
Prepare your code for Solidity 0.5.0 release.


### Auction.sol

```

Auction.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



Auction.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



Auction.sol#1295
Severity: Low
1295     function _msgData() internal view virtual returns (bytes calldata) {



```

### ETHx.sol

```

ETHx.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



ETHx.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



ETHx.sol#1108
Severity: Low
1108     function _msgData() internal view virtual returns (bytes calldata) {



```

### NodeELRewardVault.sol

```

NodeELRewardVault.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



NodeELRewardVault.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



OperatorRewardsCollector.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



OperatorRewardsCollector.sol#1103
Severity: Low
1103     function _msgData() internal view virtual returns (bytes calldata) {



```

### Penalty.sol

```

Penalty.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



Penalty.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



Penalty.sol#1565
Severity: Low
1565     function _msgData() internal view virtual returns (bytes calldata) {



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



PermissionedNodeRegistry.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



PermissionedNodeRegistry.sol#1445
Severity: Low
1445     function _msgData() internal view virtual returns (bytes calldata) {



```

### PermissionedPool.sol

```

PermissionedPool.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



PermissionedPool.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



PermissionedPool.sol#1568
Severity: Low
1568     function _msgData() internal view virtual returns (bytes calldata) {



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



PermissionlessNodeRegistry.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



PermissionlessNodeRegistry.sol#1277
Severity: Low
1277     function _msgData() internal view virtual returns (bytes calldata) {



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



PermissionlessPool.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



PermissionlessPool.sol#1553
Severity: Low
1553     function _msgData() internal view virtual returns (bytes calldata) {



```

### PoolSelector.sol

```

PoolSelector.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



PoolSelector.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



PoolSelector.sol#1561
Severity: Low
1561     function _msgData() internal view virtual returns (bytes calldata) {



```

### PoolUtils.sol

```

PoolUtils.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



PoolUtils.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



PoolUtils.sol#1138
Severity: Low
1138     function _msgData() internal view virtual returns (bytes calldata) {



PoolUtils.sol#2023
Severity: Low
2023     function isExistingPubkey(bytes calldata _pubkey) public view override returns (bool) {



```

### SDCollateral.sol

```

SDCollateral.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



SDCollateral.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



SDCollateral.sol#1836
Severity: Low
1836     function _msgData() internal view virtual returns (bytes calldata) {



```

### SocializingPool.sol

```

SocializingPool.sol#562
Severity: Low
562     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



SocializingPool.sol#571
Severity: Low
571     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



SocializingPool.sol#1317
Severity: Low
1317     function _msgData() internal view virtual returns (bytes calldata) {



SocializingPool.sol#2275
Severity: Low
2275         bytes32[] calldata proof,



SocializingPool.sol#2303
Severity: Low
2303     function processProofCalldata(bytes32[] calldata proof, bytes32 leaf) internal pure returns (bytes32) {



```

### StaderConfig.sol

```

StaderConfig.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



StaderConfig.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



StaderConfig.sol#1090
Severity: Low
1090     function _msgData() internal view virtual returns (bytes calldata) {



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



StaderInsuranceFund.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



StaderInsuranceFund.sol#1116
Severity: Low
1116     function _msgData() internal view virtual returns (bytes calldata) {



```

### StaderOracle.sol

```

StaderOracle.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



StaderOracle.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



StaderOracle.sol#1467
Severity: Low
1467     function _msgData() internal view virtual returns (bytes calldata) {



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#562
Severity: Low
562     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



StaderStakePoolsManager.sol#571
Severity: Low
571     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



StaderStakePoolsManager.sol#1109
Severity: Low
1109     function _msgData() internal view virtual returns (bytes calldata) {



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



UserWithdrawalManager.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



UserWithdrawalManager.sol#1108
Severity: Low
1108     function _msgData() internal view virtual returns (bytes calldata) {



```

### UtilLib.sol

```

UtilLib.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



UtilLib.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



ValidatorWithdrawalVault.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



```

### VaultFactory.sol

```

VaultFactory.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



VaultFactory.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



VaultFactory.sol#1285
Severity: Low
1285     function _msgData() internal view virtual returns (bytes calldata) {



```

### VaultProxy.sol

```

VaultProxy.sol#561
Severity: Low
561     function getPubkeyRoot(bytes calldata _pubkey) internal pure returns (bytes32) {



VaultProxy.sol#570
Severity: Low
570     function getValidatorSettleStatus(bytes calldata _pubkey, IStaderConfig _staderConfig)



```

## SOLIDITY_USING_INLINE_ASSEMBLY
Inline assembly is a way to access the Ethereum Virtual Machine at a low level. This discards several important safety features of Solidity.


### Auction.sol

```

Auction.sol#1371
Severity: Low
1371             assembly {



Auction.sol#1391
Severity: Low
1391             assembly {



Auction.sol#1405
Severity: Low
1405             assembly {



Auction.sol#1668
Severity: Low
1668             assembly {



Auction.sol#1674
Severity: Low
1674                 assembly {



```

### ETHx.sol

```

ETHx.sol#1664
Severity: Low
1664             assembly {



ETHx.sol#1684
Severity: Low
1684             assembly {



ETHx.sol#1698
Severity: Low
1698             assembly {



ETHx.sol#1961
Severity: Low
1961             assembly {



ETHx.sol#1967
Severity: Low
1967                 assembly {



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#1179
Severity: Low
1179             assembly {



OperatorRewardsCollector.sol#1199
Severity: Low
1199             assembly {



OperatorRewardsCollector.sol#1213
Severity: Low
1213             assembly {



OperatorRewardsCollector.sol#1476
Severity: Low
1476             assembly {



OperatorRewardsCollector.sol#1482
Severity: Low
1482                 assembly {



```

### Penalty.sol

```

Penalty.sol#1641
Severity: Low
1641             assembly {



Penalty.sol#1661
Severity: Low
1661             assembly {



Penalty.sol#1675
Severity: Low
1675             assembly {



Penalty.sol#1938
Severity: Low
1938             assembly {



Penalty.sol#1944
Severity: Low
1944                 assembly {



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#881
Severity: Low
881             assembly {



PermissionedNodeRegistry.sol#901
Severity: Low
901             assembly {



PermissionedNodeRegistry.sol#915
Severity: Low
915             assembly {



PermissionedNodeRegistry.sol#1719
Severity: Low
1719             assembly {



PermissionedNodeRegistry.sol#1739
Severity: Low
1739             assembly {



PermissionedNodeRegistry.sol#1753
Severity: Low
1753             assembly {



PermissionedNodeRegistry.sol#2016
Severity: Low
2016             assembly {



PermissionedNodeRegistry.sol#2022
Severity: Low
2022                 assembly {



```

### PermissionedPool.sol

```

PermissionedPool.sol#918
Severity: Low
918             assembly {



PermissionedPool.sol#938
Severity: Low
938             assembly {



PermissionedPool.sol#952
Severity: Low
952             assembly {



PermissionedPool.sol#1644
Severity: Low
1644             assembly {



PermissionedPool.sol#1664
Severity: Low
1664             assembly {



PermissionedPool.sol#1678
Severity: Low
1678             assembly {



PermissionedPool.sol#1941
Severity: Low
1941             assembly {



PermissionedPool.sol#1947
Severity: Low
1947                 assembly {



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#1551
Severity: Low
1551             assembly {



PermissionlessNodeRegistry.sol#1571
Severity: Low
1571             assembly {



PermissionlessNodeRegistry.sol#1585
Severity: Low
1585             assembly {



PermissionlessNodeRegistry.sol#1848
Severity: Low
1848             assembly {



PermissionlessNodeRegistry.sol#1854
Severity: Low
1854                 assembly {



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#903
Severity: Low
903             assembly {



PermissionlessPool.sol#923
Severity: Low
923             assembly {



PermissionlessPool.sol#937
Severity: Low
937             assembly {



PermissionlessPool.sol#1629
Severity: Low
1629             assembly {



PermissionlessPool.sol#1649
Severity: Low
1649             assembly {



PermissionlessPool.sol#1663
Severity: Low
1663             assembly {



PermissionlessPool.sol#1926
Severity: Low
1926             assembly {



PermissionlessPool.sol#1932
Severity: Low
1932                 assembly {



```

### PoolSelector.sol

```

PoolSelector.sol#686
Severity: Low
686             assembly {



PoolSelector.sol#706
Severity: Low
706             assembly {



PoolSelector.sol#720
Severity: Low
720             assembly {



PoolSelector.sol#1637
Severity: Low
1637             assembly {



PoolSelector.sol#1657
Severity: Low
1657             assembly {



PoolSelector.sol#1671
Severity: Low
1671             assembly {



PoolSelector.sol#1934
Severity: Low
1934             assembly {



PoolSelector.sol#1940
Severity: Low
1940                 assembly {



```

### PoolUtils.sol

```

PoolUtils.sol#1214
Severity: Low
1214             assembly {



PoolUtils.sol#1234
Severity: Low
1234             assembly {



PoolUtils.sol#1248
Severity: Low
1248             assembly {



PoolUtils.sol#1511
Severity: Low
1511             assembly {



PoolUtils.sol#1517
Severity: Low
1517                 assembly {



```

### SDCollateral.sol

```

SDCollateral.sol#1186
Severity: Low
1186             assembly {



SDCollateral.sol#1206
Severity: Low
1206             assembly {



SDCollateral.sol#1220
Severity: Low
1220             assembly {



SDCollateral.sol#1912
Severity: Low
1912             assembly {



SDCollateral.sol#1932
Severity: Low
1932             assembly {



SDCollateral.sol#1946
Severity: Low
1946             assembly {



SDCollateral.sol#2209
Severity: Low
2209             assembly {



SDCollateral.sol#2215
Severity: Low
2215                 assembly {



```

### SocializingPool.sol

```

SocializingPool.sol#1393
Severity: Low
1393             assembly {



SocializingPool.sol#1413
Severity: Low
1413             assembly {



SocializingPool.sol#1427
Severity: Low
1427             assembly {



SocializingPool.sol#1690
Severity: Low
1690             assembly {



SocializingPool.sol#1696
Severity: Low
1696                 assembly {



```

### StaderConfig.sol

```

StaderConfig.sol#1166
Severity: Low
1166             assembly {



StaderConfig.sol#1186
Severity: Low
1186             assembly {



StaderConfig.sol#1200
Severity: Low
1200             assembly {



StaderConfig.sol#1463
Severity: Low
1463             assembly {



StaderConfig.sol#1469
Severity: Low
1469                 assembly {



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#1192
Severity: Low
1192             assembly {



StaderInsuranceFund.sol#1212
Severity: Low
1212             assembly {



StaderInsuranceFund.sol#1226
Severity: Low
1226             assembly {



StaderInsuranceFund.sol#1489
Severity: Low
1489             assembly {



StaderInsuranceFund.sol#1495
Severity: Low
1495                 assembly {



```

### StaderOracle.sol

```

StaderOracle.sol#1741
Severity: Low
1741             assembly {



StaderOracle.sol#1761
Severity: Low
1761             assembly {



StaderOracle.sol#1775
Severity: Low
1775             assembly {



StaderOracle.sol#2038
Severity: Low
2038             assembly {



StaderOracle.sol#2044
Severity: Low
2044                 assembly {



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#1665
Severity: Low
1665             assembly {



StaderStakePoolsManager.sol#1685
Severity: Low
1685             assembly {



StaderStakePoolsManager.sol#1699
Severity: Low
1699             assembly {



StaderStakePoolsManager.sol#1962
Severity: Low
1962             assembly {



StaderStakePoolsManager.sol#1968
Severity: Low
1968                 assembly {



StaderStakePoolsManager.sol#3147
Severity: Low
3147             assembly {



StaderStakePoolsManager.sol#3167
Severity: Low
3167             assembly {



StaderStakePoolsManager.sol#3181
Severity: Low
3181             assembly {



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#1664
Severity: Low
1664             assembly {



UserWithdrawalManager.sol#1684
Severity: Low
1684             assembly {



UserWithdrawalManager.sol#1698
Severity: Low
1698             assembly {



UserWithdrawalManager.sol#1961
Severity: Low
1961             assembly {



UserWithdrawalManager.sol#1967
Severity: Low
1967                 assembly {



UserWithdrawalManager.sol#3076
Severity: Low
3076             assembly {



UserWithdrawalManager.sol#3096
Severity: Low
3096             assembly {



UserWithdrawalManager.sol#3110
Severity: Low
3110             assembly {



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#1007
Severity: Low
1007             assembly {



ValidatorWithdrawalVault.sol#1027
Severity: Low
1027             assembly {



ValidatorWithdrawalVault.sol#1041
Severity: Low
1041             assembly {



```

### VaultFactory.sol

```

VaultFactory.sol#733
Severity: Low
733         assembly {



VaultFactory.sol#753
Severity: Low
753         assembly {



VaultFactory.sol#773
Severity: Low
773         assembly {



VaultFactory.sol#1361
Severity: Low
1361             assembly {



VaultFactory.sol#1381
Severity: Low
1381             assembly {



VaultFactory.sol#1395
Severity: Low
1395             assembly {



VaultFactory.sol#1658
Severity: Low
1658             assembly {



VaultFactory.sol#1664
Severity: Low
1664                 assembly {



```

## SOLIDITY_VISIBILITY
The default function visibility level in contracts is ```public```, in interfaces - ```external```, state variable default visibility level is ```internal```.

In contracts, the fallback function can be ```external``` or ```public```. In interfaces, all the functions should be declared as ```external```. Explicitly define function visibility to prevent confusion.


### Auction.sol

```

Auction.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



Auction.sol#393
Severity: Low
393     function onlyValidKeys(



Auction.sol#955
Severity: Low
955     function sendValue(address payable recipient, uint256 amount) internal {



Auction.sol#2227
Severity: Low
2227     constructor() {



Auction.sol#6
Severity: Low
6     error InvalidLimits();



Auction.sol#6
Severity: Low
6     error InvalidLimits();



Auction.sol#7
Severity: Low
7     error InvalidMinDepositValue();



Auction.sol#7
Severity: Low
7     error InvalidMinDepositValue();



Auction.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



Auction.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



Auction.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



Auction.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



Auction.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



Auction.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



Auction.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



Auction.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



Auction.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



Auction.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



Auction.sol#198
Severity: Low
198     error maxKeyLimitReached();



Auction.sol#198
Severity: Low
198     error maxKeyLimitReached();



Auction.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



Auction.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



Auction.sol#200
Severity: Low
200     error InvalidKeyCount();



Auction.sol#200
Severity: Low
200     error InvalidKeyCount();



Auction.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



Auction.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



Auction.sol#202
Severity: Low
202     error OperatorIsDeactivate();



Auction.sol#202
Severity: Low
202     error OperatorIsDeactivate();



Auction.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



Auction.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



Auction.sol#204
Severity: Low
204     error PageNumberIsZero();



Auction.sol#204
Severity: Low
204     error PageNumberIsZero();



Auction.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



Auction.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



Auction.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



Auction.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



Auction.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



Auction.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



Auction.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



Auction.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



Auction.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



Auction.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



Auction.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



Auction.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



Auction.sol#240
Severity: Low
240             bytes calldata pubkey,



Auction.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



Auction.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



Auction.sol#242
Severity: Low
242             bytes calldata depositSignature,



Auction.sol#242
Severity: Low
242             bytes calldata depositSignature,



Auction.sol#243
Severity: Low
243             address withdrawVaultAddress,



Auction.sol#244
Severity: Low
244             uint256 operatorId,



Auction.sol#245
Severity: Low
245             uint256 depositTime,



Auction.sol#246
Severity: Low
246             uint256 withdrawnTime



Auction.sol#256
Severity: Low
256             string calldata operatorName,



Auction.sol#257
Severity: Low
257             address payable operatorRewardAddress,



Auction.sol#258
Severity: Low
258             address operatorAddress



Auction.sol#324
Severity: Low
324     error EmptyNameString();



Auction.sol#324
Severity: Low
324     error EmptyNameString();



Auction.sol#325
Severity: Low
325     error PoolIdNotPresent();



Auction.sol#325
Severity: Low
325     error PoolIdNotPresent();



Auction.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



Auction.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



Auction.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



Auction.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



Auction.sol#328
Severity: Low
328     error NameCrossedMaxLength();



Auction.sol#328
Severity: Low
328     error NameCrossedMaxLength();



Auction.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



Auction.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



Auction.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



Auction.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



Auction.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



Auction.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



Auction.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



Auction.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



Auction.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



Auction.sol#396
Severity: Low
396         bytes calldata _depositSignature



Auction.sol#410
Severity: Low
410     error CallerNotOwner();



Auction.sol#410
Severity: Low
410     error CallerNotOwner();



Auction.sol#411
Severity: Low
411     error AlreadyInitialized();



Auction.sol#411
Severity: Low
411     error AlreadyInitialized();



Auction.sol#437
Severity: Low
437     error ZeroAddress();



Auction.sol#437
Severity: Low
437     error ZeroAddress();



Auction.sol#438
Severity: Low
438     error InvalidPubkeyLength();



Auction.sol#438
Severity: Low
438     error InvalidPubkeyLength();



Auction.sol#439
Severity: Low
439     error CallerNotManager();



Auction.sol#439
Severity: Low
439     error CallerNotManager();



Auction.sol#440
Severity: Low
440     error CallerNotOperator();



Auction.sol#440
Severity: Low
440     error CallerNotOperator();



Auction.sol#441
Severity: Low
441     error CallerNotStaderContract();



Auction.sol#441
Severity: Low
441     error CallerNotStaderContract();



Auction.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



Auction.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



Auction.sol#443
Severity: Low
443     error TransferFailed();



Auction.sol#443
Severity: Low
443     error TransferFailed();



Auction.sol#604
Severity: Low
604     error InSufficientETH();



Auction.sol#604
Severity: Low
604     error InSufficientETH();



Auction.sol#605
Severity: Low
605     error ETHWithdrawFailed();



Auction.sol#605
Severity: Low
605     error ETHWithdrawFailed();



Auction.sol#606
Severity: Low
606     error AuctionEnded();



Auction.sol#606
Severity: Low
606     error AuctionEnded();



Auction.sol#607
Severity: Low
607     error AuctionNotEnded();



Auction.sol#607
Severity: Low
607     error AuctionNotEnded();



Auction.sol#608
Severity: Low
608     error ShortDuration();



Auction.sol#608
Severity: Low
608     error ShortDuration();



Auction.sol#609
Severity: Low
609     error notQualified();



Auction.sol#609
Severity: Low
609     error notQualified();



Auction.sol#610
Severity: Low
610     error AlreadyClaimed();



Auction.sol#610
Severity: Low
610     error AlreadyClaimed();



Auction.sol#611
Severity: Low
611     error NoBidPlaced();



Auction.sol#611
Severity: Low
611     error NoBidPlaced();



Auction.sol#612
Severity: Low
612     error BidWasSuccessful();



Auction.sol#612
Severity: Low
612     error BidWasSuccessful();



Auction.sol#613
Severity: Low
613     error InSufficientBid();



Auction.sol#613
Severity: Low
613     error InSufficientBid();



Auction.sol#614
Severity: Low
614     error LotWasAuctioned();



Auction.sol#614
Severity: Low
614     error LotWasAuctioned();



Auction.sol#615
Severity: Low
615     error SDTransferFailed();



Auction.sol#615
Severity: Low
615     error SDTransferFailed();



Auction.sol#673
Severity: Low
673     error InvalidDepositAmount();



Auction.sol#673
Severity: Low
673     error InvalidDepositAmount();



Auction.sol#674
Severity: Low
674     error UnsupportedOperation();



Auction.sol#674
Severity: Low
674     error UnsupportedOperation();



Auction.sol#675
Severity: Low
675     error InsufficientBalance();



Auction.sol#675
Severity: Low
675     error InsufficientBalance();



Auction.sol#676
Severity: Low
676     error TransferFailed();



Auction.sol#676
Severity: Low
676     error TransferFailed();



Auction.sol#677
Severity: Low
677     error PoolIdDoesNotExit();



Auction.sol#677
Severity: Low
677     error PoolIdDoesNotExit();



Auction.sol#678
Severity: Low
678     error CooldownNotComplete();



Auction.sol#678
Severity: Low
678     error CooldownNotComplete();



Auction.sol#679
Severity: Low
679     error UnsupportedOperationInSafeMode();



Auction.sol#679
Severity: Low
679     error UnsupportedOperationInSafeMode();



Auction.sol#955
Severity: Low
955     function sendValue(address payable recipient, uint256 amount) internal {



Auction.sol#955
Severity: Low
955     function sendValue(address payable recipient, uint256 amount) internal {



Auction.sol#956
Severity: Low
956         require(address(this).balance >= amount, "Address: insufficient balance");



Auction.sol#956
Severity: Low
956         require(address(this).balance >= amount, "Address: insufficient balance");



Auction.sol#956
Severity: Low
956         require(address(this).balance >= amount, "Address: insufficient balance");



Auction.sol#956
Severity: Low
956         require(address(this).balance >= amount, "Address: insufficient balance");



Auction.sol#958
Severity: Low
958         (bool success, ) = recipient.call{value: amount}("");



Auction.sol#958
Severity: Low
958         (bool success, ) = recipient.call{value: amount}("");



Auction.sol#958
Severity: Low
958         (bool success, ) = recipient.call{value: amount}("");



```

### ETHx.sol

```

ETHx.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



ETHx.sol#393
Severity: Low
393     function onlyValidKeys(



ETHx.sol#768
Severity: Low
768     function sendValue(address payable recipient, uint256 amount) internal {



ETHx.sol#2445
Severity: Low
2445     constructor() {



ETHx.sol#6
Severity: Low
6     error InvalidLimits();



ETHx.sol#6
Severity: Low
6     error InvalidLimits();



ETHx.sol#7
Severity: Low
7     error InvalidMinDepositValue();



ETHx.sol#7
Severity: Low
7     error InvalidMinDepositValue();



ETHx.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



ETHx.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



ETHx.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



ETHx.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



ETHx.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



ETHx.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



ETHx.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



ETHx.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



ETHx.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



ETHx.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



ETHx.sol#198
Severity: Low
198     error maxKeyLimitReached();



ETHx.sol#198
Severity: Low
198     error maxKeyLimitReached();



ETHx.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



ETHx.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



ETHx.sol#200
Severity: Low
200     error InvalidKeyCount();



ETHx.sol#200
Severity: Low
200     error InvalidKeyCount();



ETHx.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



ETHx.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



ETHx.sol#202
Severity: Low
202     error OperatorIsDeactivate();



ETHx.sol#202
Severity: Low
202     error OperatorIsDeactivate();



ETHx.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



ETHx.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



ETHx.sol#204
Severity: Low
204     error PageNumberIsZero();



ETHx.sol#204
Severity: Low
204     error PageNumberIsZero();



ETHx.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



ETHx.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



ETHx.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



ETHx.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



ETHx.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



ETHx.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



ETHx.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



ETHx.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



ETHx.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



ETHx.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



ETHx.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



ETHx.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



ETHx.sol#240
Severity: Low
240             bytes calldata pubkey,



ETHx.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



ETHx.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



ETHx.sol#242
Severity: Low
242             bytes calldata depositSignature,



ETHx.sol#242
Severity: Low
242             bytes calldata depositSignature,



ETHx.sol#243
Severity: Low
243             address withdrawVaultAddress,



ETHx.sol#244
Severity: Low
244             uint256 operatorId,



ETHx.sol#245
Severity: Low
245             uint256 depositTime,



ETHx.sol#246
Severity: Low
246             uint256 withdrawnTime



ETHx.sol#256
Severity: Low
256             string calldata operatorName,



ETHx.sol#257
Severity: Low
257             address payable operatorRewardAddress,



ETHx.sol#258
Severity: Low
258             address operatorAddress



ETHx.sol#324
Severity: Low
324     error EmptyNameString();



ETHx.sol#324
Severity: Low
324     error EmptyNameString();



ETHx.sol#325
Severity: Low
325     error PoolIdNotPresent();



ETHx.sol#325
Severity: Low
325     error PoolIdNotPresent();



ETHx.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



ETHx.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



ETHx.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



ETHx.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



ETHx.sol#328
Severity: Low
328     error NameCrossedMaxLength();



ETHx.sol#328
Severity: Low
328     error NameCrossedMaxLength();



ETHx.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



ETHx.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



ETHx.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



ETHx.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



ETHx.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



ETHx.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



ETHx.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



ETHx.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



ETHx.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



ETHx.sol#396
Severity: Low
396         bytes calldata _depositSignature



ETHx.sol#410
Severity: Low
410     error CallerNotOwner();



ETHx.sol#410
Severity: Low
410     error CallerNotOwner();



ETHx.sol#411
Severity: Low
411     error AlreadyInitialized();



ETHx.sol#411
Severity: Low
411     error AlreadyInitialized();



ETHx.sol#437
Severity: Low
437     error ZeroAddress();



ETHx.sol#437
Severity: Low
437     error ZeroAddress();



ETHx.sol#438
Severity: Low
438     error InvalidPubkeyLength();



ETHx.sol#438
Severity: Low
438     error InvalidPubkeyLength();



ETHx.sol#439
Severity: Low
439     error CallerNotManager();



ETHx.sol#439
Severity: Low
439     error CallerNotManager();



ETHx.sol#440
Severity: Low
440     error CallerNotOperator();



ETHx.sol#440
Severity: Low
440     error CallerNotOperator();



ETHx.sol#441
Severity: Low
441     error CallerNotStaderContract();



ETHx.sol#441
Severity: Low
441     error CallerNotStaderContract();



ETHx.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



ETHx.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



ETHx.sol#443
Severity: Low
443     error TransferFailed();



ETHx.sol#443
Severity: Low
443     error TransferFailed();



ETHx.sol#768
Severity: Low
768     function sendValue(address payable recipient, uint256 amount) internal {



ETHx.sol#768
Severity: Low
768     function sendValue(address payable recipient, uint256 amount) internal {



ETHx.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



ETHx.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



ETHx.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



ETHx.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



ETHx.sol#771
Severity: Low
771         (bool success, ) = recipient.call{value: amount}("");



ETHx.sol#771
Severity: Low
771         (bool success, ) = recipient.call{value: amount}("");



ETHx.sol#771
Severity: Low
771         (bool success, ) = recipient.call{value: amount}("");



```

### NodeELRewardVault.sol

```

NodeELRewardVault.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



NodeELRewardVault.sol#393
Severity: Low
393     function onlyValidKeys(



NodeELRewardVault.sol#686
Severity: Low
686     constructor() {}



NodeELRewardVault.sol#6
Severity: Low
6     error InvalidLimits();



NodeELRewardVault.sol#6
Severity: Low
6     error InvalidLimits();



NodeELRewardVault.sol#7
Severity: Low
7     error InvalidMinDepositValue();



NodeELRewardVault.sol#7
Severity: Low
7     error InvalidMinDepositValue();



NodeELRewardVault.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



NodeELRewardVault.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



NodeELRewardVault.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



NodeELRewardVault.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



NodeELRewardVault.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



NodeELRewardVault.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



NodeELRewardVault.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



NodeELRewardVault.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



NodeELRewardVault.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



NodeELRewardVault.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



NodeELRewardVault.sol#198
Severity: Low
198     error maxKeyLimitReached();



NodeELRewardVault.sol#198
Severity: Low
198     error maxKeyLimitReached();



NodeELRewardVault.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



NodeELRewardVault.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



NodeELRewardVault.sol#200
Severity: Low
200     error InvalidKeyCount();



NodeELRewardVault.sol#200
Severity: Low
200     error InvalidKeyCount();



NodeELRewardVault.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



NodeELRewardVault.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



NodeELRewardVault.sol#202
Severity: Low
202     error OperatorIsDeactivate();



NodeELRewardVault.sol#202
Severity: Low
202     error OperatorIsDeactivate();



NodeELRewardVault.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



NodeELRewardVault.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



NodeELRewardVault.sol#204
Severity: Low
204     error PageNumberIsZero();



NodeELRewardVault.sol#204
Severity: Low
204     error PageNumberIsZero();



NodeELRewardVault.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



NodeELRewardVault.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



NodeELRewardVault.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



NodeELRewardVault.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



NodeELRewardVault.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



NodeELRewardVault.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



NodeELRewardVault.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



NodeELRewardVault.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



NodeELRewardVault.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



NodeELRewardVault.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



NodeELRewardVault.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



NodeELRewardVault.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



NodeELRewardVault.sol#240
Severity: Low
240             bytes calldata pubkey,



NodeELRewardVault.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



NodeELRewardVault.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



NodeELRewardVault.sol#242
Severity: Low
242             bytes calldata depositSignature,



NodeELRewardVault.sol#242
Severity: Low
242             bytes calldata depositSignature,



NodeELRewardVault.sol#243
Severity: Low
243             address withdrawVaultAddress,



NodeELRewardVault.sol#244
Severity: Low
244             uint256 operatorId,



NodeELRewardVault.sol#245
Severity: Low
245             uint256 depositTime,



NodeELRewardVault.sol#246
Severity: Low
246             uint256 withdrawnTime



NodeELRewardVault.sol#256
Severity: Low
256             string calldata operatorName,



NodeELRewardVault.sol#257
Severity: Low
257             address payable operatorRewardAddress,



NodeELRewardVault.sol#258
Severity: Low
258             address operatorAddress



NodeELRewardVault.sol#324
Severity: Low
324     error EmptyNameString();



NodeELRewardVault.sol#324
Severity: Low
324     error EmptyNameString();



NodeELRewardVault.sol#325
Severity: Low
325     error PoolIdNotPresent();



NodeELRewardVault.sol#325
Severity: Low
325     error PoolIdNotPresent();



NodeELRewardVault.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



NodeELRewardVault.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



NodeELRewardVault.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



NodeELRewardVault.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



NodeELRewardVault.sol#328
Severity: Low
328     error NameCrossedMaxLength();



NodeELRewardVault.sol#328
Severity: Low
328     error NameCrossedMaxLength();



NodeELRewardVault.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



NodeELRewardVault.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



NodeELRewardVault.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



NodeELRewardVault.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



NodeELRewardVault.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



NodeELRewardVault.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



NodeELRewardVault.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



NodeELRewardVault.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



NodeELRewardVault.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



NodeELRewardVault.sol#396
Severity: Low
396         bytes calldata _depositSignature



NodeELRewardVault.sol#410
Severity: Low
410     error CallerNotOwner();



NodeELRewardVault.sol#410
Severity: Low
410     error CallerNotOwner();



NodeELRewardVault.sol#411
Severity: Low
411     error AlreadyInitialized();



NodeELRewardVault.sol#411
Severity: Low
411     error AlreadyInitialized();



NodeELRewardVault.sol#437
Severity: Low
437     error ZeroAddress();



NodeELRewardVault.sol#437
Severity: Low
437     error ZeroAddress();



NodeELRewardVault.sol#438
Severity: Low
438     error InvalidPubkeyLength();



NodeELRewardVault.sol#438
Severity: Low
438     error InvalidPubkeyLength();



NodeELRewardVault.sol#439
Severity: Low
439     error CallerNotManager();



NodeELRewardVault.sol#439
Severity: Low
439     error CallerNotManager();



NodeELRewardVault.sol#440
Severity: Low
440     error CallerNotOperator();



NodeELRewardVault.sol#440
Severity: Low
440     error CallerNotOperator();



NodeELRewardVault.sol#441
Severity: Low
441     error CallerNotStaderContract();



NodeELRewardVault.sol#441
Severity: Low
441     error CallerNotStaderContract();



NodeELRewardVault.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



NodeELRewardVault.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



NodeELRewardVault.sol#443
Severity: Low
443     error TransferFailed();



NodeELRewardVault.sol#443
Severity: Low
443     error TransferFailed();



NodeELRewardVault.sol#604
Severity: Low
604     error NotEnoughRewardToWithdraw();



NodeELRewardVault.sol#604
Severity: Low
604     error NotEnoughRewardToWithdraw();



NodeELRewardVault.sol#605
Severity: Low
605     error ETHTransferFailed(address recipient, uint256 amount);



NodeELRewardVault.sol#605
Severity: Low
605     error ETHTransferFailed(address recipient, uint256 amount);



NodeELRewardVault.sol#605
Severity: Low
605     error ETHTransferFailed(address recipient, uint256 amount);



NodeELRewardVault.sol#618
Severity: Low
618     error InvalidDepositAmount();



NodeELRewardVault.sol#618
Severity: Low
618     error InvalidDepositAmount();



NodeELRewardVault.sol#619
Severity: Low
619     error UnsupportedOperation();



NodeELRewardVault.sol#619
Severity: Low
619     error UnsupportedOperation();



NodeELRewardVault.sol#620
Severity: Low
620     error InsufficientBalance();



NodeELRewardVault.sol#620
Severity: Low
620     error InsufficientBalance();



NodeELRewardVault.sol#621
Severity: Low
621     error TransferFailed();



NodeELRewardVault.sol#621
Severity: Low
621     error TransferFailed();



NodeELRewardVault.sol#622
Severity: Low
622     error PoolIdDoesNotExit();



NodeELRewardVault.sol#622
Severity: Low
622     error PoolIdDoesNotExit();



NodeELRewardVault.sol#623
Severity: Low
623     error CooldownNotComplete();



NodeELRewardVault.sol#623
Severity: Low
623     error CooldownNotComplete();



NodeELRewardVault.sol#624
Severity: Low
624     error UnsupportedOperationInSafeMode();



NodeELRewardVault.sol#624
Severity: Low
624     error UnsupportedOperationInSafeMode();



NodeELRewardVault.sol#692
Severity: Low
692     receive() external payable {



NodeELRewardVault.sol#693
Severity: Low
693         emit ETHReceived(msg.sender, msg.value);



NodeELRewardVault.sol#693
Severity: Low
693         emit ETHReceived(msg.sender, msg.value);



NodeELRewardVault.sol#693
Severity: Low
693         emit ETHReceived(msg.sender, msg.value);



```

### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



OperatorRewardsCollector.sol#393
Severity: Low
393     function onlyValidKeys(



OperatorRewardsCollector.sol#763
Severity: Low
763     function sendValue(address payable recipient, uint256 amount) internal {



OperatorRewardsCollector.sol#1957
Severity: Low
1957     constructor() {



OperatorRewardsCollector.sol#6
Severity: Low
6     error InvalidLimits();



OperatorRewardsCollector.sol#6
Severity: Low
6     error InvalidLimits();



OperatorRewardsCollector.sol#7
Severity: Low
7     error InvalidMinDepositValue();



OperatorRewardsCollector.sol#7
Severity: Low
7     error InvalidMinDepositValue();



OperatorRewardsCollector.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



OperatorRewardsCollector.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



OperatorRewardsCollector.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



OperatorRewardsCollector.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



OperatorRewardsCollector.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



OperatorRewardsCollector.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



OperatorRewardsCollector.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



OperatorRewardsCollector.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



OperatorRewardsCollector.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



OperatorRewardsCollector.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



OperatorRewardsCollector.sol#198
Severity: Low
198     error maxKeyLimitReached();



OperatorRewardsCollector.sol#198
Severity: Low
198     error maxKeyLimitReached();



OperatorRewardsCollector.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



OperatorRewardsCollector.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



OperatorRewardsCollector.sol#200
Severity: Low
200     error InvalidKeyCount();



OperatorRewardsCollector.sol#200
Severity: Low
200     error InvalidKeyCount();



OperatorRewardsCollector.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



OperatorRewardsCollector.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



OperatorRewardsCollector.sol#202
Severity: Low
202     error OperatorIsDeactivate();



OperatorRewardsCollector.sol#202
Severity: Low
202     error OperatorIsDeactivate();



OperatorRewardsCollector.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



OperatorRewardsCollector.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



OperatorRewardsCollector.sol#204
Severity: Low
204     error PageNumberIsZero();



OperatorRewardsCollector.sol#204
Severity: Low
204     error PageNumberIsZero();



OperatorRewardsCollector.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



OperatorRewardsCollector.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



OperatorRewardsCollector.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



OperatorRewardsCollector.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



OperatorRewardsCollector.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



OperatorRewardsCollector.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



OperatorRewardsCollector.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



OperatorRewardsCollector.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



OperatorRewardsCollector.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



OperatorRewardsCollector.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



OperatorRewardsCollector.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



OperatorRewardsCollector.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



OperatorRewardsCollector.sol#240
Severity: Low
240             bytes calldata pubkey,



OperatorRewardsCollector.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



OperatorRewardsCollector.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



OperatorRewardsCollector.sol#242
Severity: Low
242             bytes calldata depositSignature,



OperatorRewardsCollector.sol#242
Severity: Low
242             bytes calldata depositSignature,



OperatorRewardsCollector.sol#243
Severity: Low
243             address withdrawVaultAddress,



OperatorRewardsCollector.sol#244
Severity: Low
244             uint256 operatorId,



OperatorRewardsCollector.sol#245
Severity: Low
245             uint256 depositTime,



OperatorRewardsCollector.sol#246
Severity: Low
246             uint256 withdrawnTime



OperatorRewardsCollector.sol#256
Severity: Low
256             string calldata operatorName,



OperatorRewardsCollector.sol#257
Severity: Low
257             address payable operatorRewardAddress,



OperatorRewardsCollector.sol#258
Severity: Low
258             address operatorAddress



OperatorRewardsCollector.sol#324
Severity: Low
324     error EmptyNameString();



OperatorRewardsCollector.sol#324
Severity: Low
324     error EmptyNameString();



OperatorRewardsCollector.sol#325
Severity: Low
325     error PoolIdNotPresent();



OperatorRewardsCollector.sol#325
Severity: Low
325     error PoolIdNotPresent();



OperatorRewardsCollector.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



OperatorRewardsCollector.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



OperatorRewardsCollector.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



OperatorRewardsCollector.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



OperatorRewardsCollector.sol#328
Severity: Low
328     error NameCrossedMaxLength();



OperatorRewardsCollector.sol#328
Severity: Low
328     error NameCrossedMaxLength();



OperatorRewardsCollector.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



OperatorRewardsCollector.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



OperatorRewardsCollector.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



OperatorRewardsCollector.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



OperatorRewardsCollector.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



OperatorRewardsCollector.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



OperatorRewardsCollector.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



OperatorRewardsCollector.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



OperatorRewardsCollector.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



OperatorRewardsCollector.sol#396
Severity: Low
396         bytes calldata _depositSignature



OperatorRewardsCollector.sol#410
Severity: Low
410     error CallerNotOwner();



OperatorRewardsCollector.sol#410
Severity: Low
410     error CallerNotOwner();



OperatorRewardsCollector.sol#411
Severity: Low
411     error AlreadyInitialized();



OperatorRewardsCollector.sol#411
Severity: Low
411     error AlreadyInitialized();



OperatorRewardsCollector.sol#437
Severity: Low
437     error ZeroAddress();



OperatorRewardsCollector.sol#437
Severity: Low
437     error ZeroAddress();



OperatorRewardsCollector.sol#438
Severity: Low
438     error InvalidPubkeyLength();



OperatorRewardsCollector.sol#438
Severity: Low
438     error InvalidPubkeyLength();



OperatorRewardsCollector.sol#439
Severity: Low
439     error CallerNotManager();



OperatorRewardsCollector.sol#439
Severity: Low
439     error CallerNotManager();



OperatorRewardsCollector.sol#440
Severity: Low
440     error CallerNotOperator();



OperatorRewardsCollector.sol#440
Severity: Low
440     error CallerNotOperator();



OperatorRewardsCollector.sol#441
Severity: Low
441     error CallerNotStaderContract();



OperatorRewardsCollector.sol#441
Severity: Low
441     error CallerNotStaderContract();



OperatorRewardsCollector.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



OperatorRewardsCollector.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



OperatorRewardsCollector.sol#443
Severity: Low
443     error TransferFailed();



OperatorRewardsCollector.sol#443
Severity: Low
443     error TransferFailed();



OperatorRewardsCollector.sol#763
Severity: Low
763     function sendValue(address payable recipient, uint256 amount) internal {



OperatorRewardsCollector.sol#763
Severity: Low
763     function sendValue(address payable recipient, uint256 amount) internal {



OperatorRewardsCollector.sol#764
Severity: Low
764         require(address(this).balance >= amount, "Address: insufficient balance");



OperatorRewardsCollector.sol#764
Severity: Low
764         require(address(this).balance >= amount, "Address: insufficient balance");



OperatorRewardsCollector.sol#764
Severity: Low
764         require(address(this).balance >= amount, "Address: insufficient balance");



OperatorRewardsCollector.sol#764
Severity: Low
764         require(address(this).balance >= amount, "Address: insufficient balance");



OperatorRewardsCollector.sol#766
Severity: Low
766         (bool success, ) = recipient.call{value: amount}("");



OperatorRewardsCollector.sol#766
Severity: Low
766         (bool success, ) = recipient.call{value: amount}("");



OperatorRewardsCollector.sol#766
Severity: Low
766         (bool success, ) = recipient.call{value: amount}("");



```

### Penalty.sol

```

Penalty.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



Penalty.sol#393
Severity: Low
393     function onlyValidKeys(



Penalty.sol#753
Severity: Low
753     function claim(



Penalty.sol#1225
Severity: Low
1225     function sendValue(address payable recipient, uint256 amount) internal {



Penalty.sol#2387
Severity: Low
2387     constructor() {



Penalty.sol#6
Severity: Low
6     error InvalidLimits();



Penalty.sol#6
Severity: Low
6     error InvalidLimits();



Penalty.sol#7
Severity: Low
7     error InvalidMinDepositValue();



Penalty.sol#7
Severity: Low
7     error InvalidMinDepositValue();



Penalty.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



Penalty.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



Penalty.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



Penalty.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



Penalty.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



Penalty.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



Penalty.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



Penalty.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



Penalty.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



Penalty.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



Penalty.sol#198
Severity: Low
198     error maxKeyLimitReached();



Penalty.sol#198
Severity: Low
198     error maxKeyLimitReached();



Penalty.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



Penalty.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



Penalty.sol#200
Severity: Low
200     error InvalidKeyCount();



Penalty.sol#200
Severity: Low
200     error InvalidKeyCount();



Penalty.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



Penalty.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



Penalty.sol#202
Severity: Low
202     error OperatorIsDeactivate();



Penalty.sol#202
Severity: Low
202     error OperatorIsDeactivate();



Penalty.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



Penalty.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



Penalty.sol#204
Severity: Low
204     error PageNumberIsZero();



Penalty.sol#204
Severity: Low
204     error PageNumberIsZero();



Penalty.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



Penalty.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



Penalty.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



Penalty.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



Penalty.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



Penalty.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



Penalty.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



Penalty.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



Penalty.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



Penalty.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



Penalty.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



Penalty.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



Penalty.sol#240
Severity: Low
240             bytes calldata pubkey,



Penalty.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



Penalty.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



Penalty.sol#242
Severity: Low
242             bytes calldata depositSignature,



Penalty.sol#242
Severity: Low
242             bytes calldata depositSignature,



Penalty.sol#243
Severity: Low
243             address withdrawVaultAddress,



Penalty.sol#244
Severity: Low
244             uint256 operatorId,



Penalty.sol#245
Severity: Low
245             uint256 depositTime,



Penalty.sol#246
Severity: Low
246             uint256 withdrawnTime



Penalty.sol#256
Severity: Low
256             string calldata operatorName,



Penalty.sol#257
Severity: Low
257             address payable operatorRewardAddress,



Penalty.sol#258
Severity: Low
258             address operatorAddress



Penalty.sol#324
Severity: Low
324     error EmptyNameString();



Penalty.sol#324
Severity: Low
324     error EmptyNameString();



Penalty.sol#325
Severity: Low
325     error PoolIdNotPresent();



Penalty.sol#325
Severity: Low
325     error PoolIdNotPresent();



Penalty.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



Penalty.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



Penalty.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



Penalty.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



Penalty.sol#328
Severity: Low
328     error NameCrossedMaxLength();



Penalty.sol#328
Severity: Low
328     error NameCrossedMaxLength();



Penalty.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



Penalty.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



Penalty.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



Penalty.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



Penalty.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



Penalty.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



Penalty.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



Penalty.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



Penalty.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



Penalty.sol#396
Severity: Low
396         bytes calldata _depositSignature



Penalty.sol#410
Severity: Low
410     error CallerNotOwner();



Penalty.sol#410
Severity: Low
410     error CallerNotOwner();



Penalty.sol#411
Severity: Low
411     error AlreadyInitialized();



Penalty.sol#411
Severity: Low
411     error AlreadyInitialized();



Penalty.sol#437
Severity: Low
437     error ZeroAddress();



Penalty.sol#437
Severity: Low
437     error ZeroAddress();



Penalty.sol#438
Severity: Low
438     error InvalidPubkeyLength();



Penalty.sol#438
Severity: Low
438     error InvalidPubkeyLength();



Penalty.sol#439
Severity: Low
439     error CallerNotManager();



Penalty.sol#439
Severity: Low
439     error CallerNotManager();



Penalty.sol#440
Severity: Low
440     error CallerNotOperator();



Penalty.sol#440
Severity: Low
440     error CallerNotOperator();



Penalty.sol#441
Severity: Low
441     error CallerNotStaderContract();



Penalty.sol#441
Severity: Low
441     error CallerNotStaderContract();



Penalty.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



Penalty.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



Penalty.sol#443
Severity: Low
443     error TransferFailed();



Penalty.sol#443
Severity: Low
443     error TransferFailed();



Penalty.sol#605
Severity: Low
605     error ValidatorSettled();



Penalty.sol#605
Severity: Low
605     error ValidatorSettled();



Penalty.sol#723
Severity: Low
723     error ETHTransferFailed(address recipient, uint256 amount);



Penalty.sol#723
Severity: Low
723     error ETHTransferFailed(address recipient, uint256 amount);



Penalty.sol#723
Severity: Low
723     error ETHTransferFailed(address recipient, uint256 amount);



Penalty.sol#724
Severity: Low
724     error SDTransferFailed();



Penalty.sol#724
Severity: Low
724     error SDTransferFailed();



Penalty.sol#725
Severity: Low
725     error RewardAlreadyHandled();



Penalty.sol#725
Severity: Low
725     error RewardAlreadyHandled();



Penalty.sol#726
Severity: Low
726     error RewardAlreadyClaimed(address operator, uint256 cycle);



Penalty.sol#726
Severity: Low
726     error RewardAlreadyClaimed(address operator, uint256 cycle);



Penalty.sol#726
Severity: Low
726     error RewardAlreadyClaimed(address operator, uint256 cycle);



Penalty.sol#727
Severity: Low
727     error InsufficientETHRewards();



Penalty.sol#727
Severity: Low
727     error InsufficientETHRewards();



Penalty.sol#728
Severity: Low
728     error InsufficientSDRewards();



Penalty.sol#728
Severity: Low
728     error InsufficientSDRewards();



Penalty.sol#729
Severity: Low
729     error InvalidAmount();



Penalty.sol#729
Severity: Low
729     error InvalidAmount();



Penalty.sol#730
Severity: Low
730     error InvalidProof(uint256 cycle, address operator);



Penalty.sol#730
Severity: Low
730     error InvalidProof(uint256 cycle, address operator);



Penalty.sol#730
Severity: Low
730     error InvalidProof(uint256 cycle, address operator);



Penalty.sol#731
Severity: Low
731     error InvalidCycleIndex();



Penalty.sol#731
Severity: Low
731     error InvalidCycleIndex();



Penalty.sol#732
Severity: Low
732     error FutureCycleIndex();



Penalty.sol#732
Severity: Low
732     error FutureCycleIndex();



Penalty.sol#755
Severity: Low
755         uint256[] calldata _amountSD,



Penalty.sol#756
Severity: Low
756         uint256[] calldata _amountETH,



Penalty.sol#756
Severity: Low
756         uint256[] calldata _amountETH,



Penalty.sol#757
Severity: Low
757         bytes32[][] calldata _merkleProof



Penalty.sol#855
Severity: Low
855     error InvalidUpdate();



Penalty.sol#855
Severity: Low
855     error InvalidUpdate();



Penalty.sol#856
Severity: Low
856     error NodeAlreadyTrusted();



Penalty.sol#856
Severity: Low
856     error NodeAlreadyTrusted();



Penalty.sol#857
Severity: Low
857     error NodeNotTrusted();



Penalty.sol#857
Severity: Low
857     error NodeNotTrusted();



Penalty.sol#858
Severity: Low
858     error ZeroFrequency();



Penalty.sol#858
Severity: Low
858     error ZeroFrequency();



Penalty.sol#859
Severity: Low
859     error FrequencyUnchanged();



Penalty.sol#859
Severity: Low
859     error FrequencyUnchanged();



Penalty.sol#860
Severity: Low
860     error DuplicateSubmissionFromNode();



Penalty.sol#860
Severity: Low
860     error DuplicateSubmissionFromNode();



Penalty.sol#861
Severity: Low
861     error ReportingFutureBlockData();



Penalty.sol#861
Severity: Low
861     error ReportingFutureBlockData();



Penalty.sol#862
Severity: Low
862     error InvalidMerkleRootIndex();



Penalty.sol#862
Severity: Low
862     error InvalidMerkleRootIndex();



Penalty.sol#863
Severity: Low
863     error ReportingPreviousCycleData();



Penalty.sol#863
Severity: Low
863     error ReportingPreviousCycleData();



Penalty.sol#864
Severity: Low
864     error InvalidMAPDIndex();



Penalty.sol#864
Severity: Low
864     error InvalidMAPDIndex();



Penalty.sol#865
Severity: Low
865     error PageNumberAlreadyReported();



Penalty.sol#865
Severity: Low
865     error PageNumberAlreadyReported();



Penalty.sol#866
Severity: Low
866     error NotATrustedNode();



Penalty.sol#866
Severity: Low
866     error NotATrustedNode();



Penalty.sol#867
Severity: Low
867     error InvalidERDataSource();



Penalty.sol#867
Severity: Low
867     error InvalidERDataSource();



Penalty.sol#868
Severity: Low
868     error InspectionModeActive();



Penalty.sol#868
Severity: Low
868     error InspectionModeActive();



Penalty.sol#869
Severity: Low
869     error UpdateFrequencyNotSet();



Penalty.sol#869
Severity: Low
869     error UpdateFrequencyNotSet();



Penalty.sol#870
Severity: Low
870     error InvalidReportingBlock();



Penalty.sol#870
Severity: Low
870     error InvalidReportingBlock();



Penalty.sol#871
Severity: Low
871     error ERChangeLimitCrossed();



Penalty.sol#871
Severity: Low
871     error ERChangeLimitCrossed();



Penalty.sol#872
Severity: Low
872     error ERChangeLimitNotCrossed();



Penalty.sol#872
Severity: Low
872     error ERChangeLimitNotCrossed();



Penalty.sol#873
Severity: Low
873     error ERPermissibleChangeOutofBounds();



Penalty.sol#873
Severity: Low
873     error ERPermissibleChangeOutofBounds();



Penalty.sol#874
Severity: Low
874     error InsufficientTrustedNodes();



Penalty.sol#874
Severity: Low
874     error InsufficientTrustedNodes();



Penalty.sol#875
Severity: Low
875     error CooldownNotComplete();



Penalty.sol#875
Severity: Low
875     error CooldownNotComplete();



Penalty.sol#1225
Severity: Low
1225     function sendValue(address payable recipient, uint256 amount) internal {



Penalty.sol#1225
Severity: Low
1225     function sendValue(address payable recipient, uint256 amount) internal {



Penalty.sol#1226
Severity: Low
1226         require(address(this).balance >= amount, "Address: insufficient balance");



Penalty.sol#1226
Severity: Low
1226         require(address(this).balance >= amount, "Address: insufficient balance");



Penalty.sol#1226
Severity: Low
1226         require(address(this).balance >= amount, "Address: insufficient balance");



Penalty.sol#1226
Severity: Low
1226         require(address(this).balance >= amount, "Address: insufficient balance");



Penalty.sol#1228
Severity: Low
1228         (bool success, ) = recipient.call{value: amount}("");



Penalty.sol#1228
Severity: Low
1228         (bool success, ) = recipient.call{value: amount}("");



Penalty.sol#1228
Severity: Low
1228         (bool success, ) = recipient.call{value: amount}("");



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



PermissionedNodeRegistry.sol#393
Severity: Low
393     function onlyValidKeys(



PermissionedNodeRegistry.sol#782
Severity: Low
782     function onboardNodeOperator(string calldata _operatorName, address payable _operatorRewardAddress)



PermissionedNodeRegistry.sol#786
Severity: Low
786     function addValidatorKeys(



PermissionedNodeRegistry.sol#812
Severity: Low
812     function updateOperatorDetails(string calldata _operatorName, address payable _rewardAddress) external;



PermissionedNodeRegistry.sol#1105
Severity: Low
1105     function sendValue(address payable recipient, uint256 amount) internal {



PermissionedNodeRegistry.sol#2493
Severity: Low
2493     constructor() {



PermissionedNodeRegistry.sol#2537
Severity: Low
2537     function onboardNodeOperator(string calldata _operatorName, address payable _operatorRewardAddress)



PermissionedNodeRegistry.sol#6
Severity: Low
6     error InvalidLimits();



PermissionedNodeRegistry.sol#6
Severity: Low
6     error InvalidLimits();



PermissionedNodeRegistry.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionedNodeRegistry.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionedNodeRegistry.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionedNodeRegistry.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionedNodeRegistry.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionedNodeRegistry.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionedNodeRegistry.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionedNodeRegistry.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionedNodeRegistry.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionedNodeRegistry.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionedNodeRegistry.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionedNodeRegistry.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionedNodeRegistry.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionedNodeRegistry.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionedNodeRegistry.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionedNodeRegistry.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionedNodeRegistry.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionedNodeRegistry.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionedNodeRegistry.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionedNodeRegistry.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionedNodeRegistry.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionedNodeRegistry.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionedNodeRegistry.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionedNodeRegistry.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionedNodeRegistry.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionedNodeRegistry.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionedNodeRegistry.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionedNodeRegistry.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionedNodeRegistry.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionedNodeRegistry.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionedNodeRegistry.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionedNodeRegistry.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionedNodeRegistry.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionedNodeRegistry.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionedNodeRegistry.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionedNodeRegistry.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionedNodeRegistry.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



PermissionedNodeRegistry.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



PermissionedNodeRegistry.sol#240
Severity: Low
240             bytes calldata pubkey,



PermissionedNodeRegistry.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionedNodeRegistry.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionedNodeRegistry.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionedNodeRegistry.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionedNodeRegistry.sol#243
Severity: Low
243             address withdrawVaultAddress,



PermissionedNodeRegistry.sol#244
Severity: Low
244             uint256 operatorId,



PermissionedNodeRegistry.sol#245
Severity: Low
245             uint256 depositTime,



PermissionedNodeRegistry.sol#246
Severity: Low
246             uint256 withdrawnTime



PermissionedNodeRegistry.sol#256
Severity: Low
256             string calldata operatorName,



PermissionedNodeRegistry.sol#257
Severity: Low
257             address payable operatorRewardAddress,



PermissionedNodeRegistry.sol#258
Severity: Low
258             address operatorAddress



PermissionedNodeRegistry.sol#324
Severity: Low
324     error EmptyNameString();



PermissionedNodeRegistry.sol#324
Severity: Low
324     error EmptyNameString();



PermissionedNodeRegistry.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionedNodeRegistry.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionedNodeRegistry.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionedNodeRegistry.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionedNodeRegistry.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionedNodeRegistry.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionedNodeRegistry.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionedNodeRegistry.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionedNodeRegistry.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionedNodeRegistry.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionedNodeRegistry.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionedNodeRegistry.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionedNodeRegistry.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionedNodeRegistry.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionedNodeRegistry.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionedNodeRegistry.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionedNodeRegistry.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



PermissionedNodeRegistry.sol#396
Severity: Low
396         bytes calldata _depositSignature



PermissionedNodeRegistry.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionedNodeRegistry.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionedNodeRegistry.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionedNodeRegistry.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionedNodeRegistry.sol#437
Severity: Low
437     error ZeroAddress();



PermissionedNodeRegistry.sol#437
Severity: Low
437     error ZeroAddress();



PermissionedNodeRegistry.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionedNodeRegistry.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionedNodeRegistry.sol#439
Severity: Low
439     error CallerNotManager();



PermissionedNodeRegistry.sol#439
Severity: Low
439     error CallerNotManager();



PermissionedNodeRegistry.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionedNodeRegistry.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionedNodeRegistry.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionedNodeRegistry.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionedNodeRegistry.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionedNodeRegistry.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionedNodeRegistry.sol#443
Severity: Low
443     error TransferFailed();



PermissionedNodeRegistry.sol#443
Severity: Low
443     error TransferFailed();



PermissionedNodeRegistry.sol#644
Severity: Low
644     error InvalidRewardAmount();



PermissionedNodeRegistry.sol#644
Severity: Low
644     error InvalidRewardAmount();



PermissionedNodeRegistry.sol#645
Severity: Low
645     error NotEnoughRewardToDistribute();



PermissionedNodeRegistry.sol#645
Severity: Low
645     error NotEnoughRewardToDistribute();



PermissionedNodeRegistry.sol#646
Severity: Low
646     error CallerNotNodeRegistryContract();



PermissionedNodeRegistry.sol#646
Severity: Low
646     error CallerNotNodeRegistryContract();



PermissionedNodeRegistry.sol#686
Severity: Low
686     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



PermissionedNodeRegistry.sol#686
Severity: Low
686     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



PermissionedNodeRegistry.sol#687
Severity: Low
687     error InvalidPoolId();



PermissionedNodeRegistry.sol#687
Severity: Low
687     error InvalidPoolId();



PermissionedNodeRegistry.sol#688
Severity: Low
688     error InvalidPoolLimit();



PermissionedNodeRegistry.sol#688
Severity: Low
688     error InvalidPoolLimit();



PermissionedNodeRegistry.sol#689
Severity: Low
689     error SDTransferFailed();



PermissionedNodeRegistry.sol#689
Severity: Low
689     error SDTransferFailed();



PermissionedNodeRegistry.sol#690
Severity: Low
690     error NoStateChange();



PermissionedNodeRegistry.sol#690
Severity: Low
690     error NoStateChange();



PermissionedNodeRegistry.sol#750
Severity: Low
750     error NotAPermissionedNodeOperator();



PermissionedNodeRegistry.sol#750
Severity: Low
750     error NotAPermissionedNodeOperator();



PermissionedNodeRegistry.sol#751
Severity: Low
751     error OperatorAlreadyDeactivate();



PermissionedNodeRegistry.sol#751
Severity: Low
751     error OperatorAlreadyDeactivate();



PermissionedNodeRegistry.sol#752
Severity: Low
752     error OperatorAlreadyActive();



PermissionedNodeRegistry.sol#752
Severity: Low
752     error OperatorAlreadyActive();



PermissionedNodeRegistry.sol#753
Severity: Low
753     error MaxOperatorLimitReached();



PermissionedNodeRegistry.sol#753
Severity: Low
753     error MaxOperatorLimitReached();



PermissionedNodeRegistry.sol#784
Severity: Low
784         returns (address mevFeeRecipientAddress);



PermissionedNodeRegistry.sol#788
Severity: Low
788         bytes[] calldata _preDepositSignature,



PermissionedNodeRegistry.sol#789
Severity: Low
789         bytes[] calldata _depositSignature



PermissionedNodeRegistry.sol#1105
Severity: Low
1105     function sendValue(address payable recipient, uint256 amount) internal {



PermissionedNodeRegistry.sol#1105
Severity: Low
1105     function sendValue(address payable recipient, uint256 amount) internal {



PermissionedNodeRegistry.sol#1106
Severity: Low
1106         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedNodeRegistry.sol#1106
Severity: Low
1106         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedNodeRegistry.sol#1106
Severity: Low
1106         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedNodeRegistry.sol#1106
Severity: Low
1106         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedNodeRegistry.sol#1108
Severity: Low
1108         (bool success, ) = recipient.call{value: amount}("");



PermissionedNodeRegistry.sol#1108
Severity: Low
1108         (bool success, ) = recipient.call{value: amount}("");



PermissionedNodeRegistry.sol#1108
Severity: Low
1108         (bool success, ) = recipient.call{value: amount}("");



PermissionedNodeRegistry.sol#2540
Severity: Low
2540         whenNotPaused



PermissionedNodeRegistry.sol#2541
Severity: Low
2541         returns (address)



PermissionedNodeRegistry.sol#2543
Severity: Low
2543         address poolUtils = staderConfig.getPoolUtils();



PermissionedNodeRegistry.sol#2544
Severity: Low
2544         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionedPool()) {



PermissionedNodeRegistry.sol#2544
Severity: Low
2544         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionedPool()) {



PermissionedNodeRegistry.sol#2544
Severity: Low
2544         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionedPool()) {



PermissionedNodeRegistry.sol#2544
Severity: Low
2544         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionedPool()) {



PermissionedNodeRegistry.sol#2544
Severity: Low
2544         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionedPool()) {



PermissionedNodeRegistry.sol#2545
Severity: Low
2545             revert DuplicatePoolIDOrPoolNotAdded();



PermissionedNodeRegistry.sol#2545
Severity: Low
2545             revert DuplicatePoolIDOrPoolNotAdded();



```

### PermissionedPool.sol

```

PermissionedPool.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



PermissionedPool.sol#393
Severity: Low
393     function onlyValidKeys(



PermissionedPool.sol#695
Severity: Low
695     function deposit(



PermissionedPool.sol#819
Severity: Low
819     function onboardNodeOperator(string calldata _operatorName, address payable _operatorRewardAddress)



PermissionedPool.sol#823
Severity: Low
823     function addValidatorKeys(



PermissionedPool.sol#849
Severity: Low
849     function updateOperatorDetails(string calldata _operatorName, address payable _rewardAddress) external;



PermissionedPool.sol#1228
Severity: Low
1228     function sendValue(address payable recipient, uint256 amount) internal {



PermissionedPool.sol#2392
Severity: Low
2392     constructor() {



PermissionedPool.sol#6
Severity: Low
6     error InvalidLimits();



PermissionedPool.sol#6
Severity: Low
6     error InvalidLimits();



PermissionedPool.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionedPool.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionedPool.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionedPool.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionedPool.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionedPool.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionedPool.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionedPool.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionedPool.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionedPool.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionedPool.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionedPool.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionedPool.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionedPool.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionedPool.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionedPool.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionedPool.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionedPool.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionedPool.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionedPool.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionedPool.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionedPool.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionedPool.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionedPool.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionedPool.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionedPool.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionedPool.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionedPool.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionedPool.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionedPool.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionedPool.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionedPool.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionedPool.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionedPool.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionedPool.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionedPool.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionedPool.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



PermissionedPool.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



PermissionedPool.sol#240
Severity: Low
240             bytes calldata pubkey,



PermissionedPool.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionedPool.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionedPool.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionedPool.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionedPool.sol#243
Severity: Low
243             address withdrawVaultAddress,



PermissionedPool.sol#244
Severity: Low
244             uint256 operatorId,



PermissionedPool.sol#245
Severity: Low
245             uint256 depositTime,



PermissionedPool.sol#246
Severity: Low
246             uint256 withdrawnTime



PermissionedPool.sol#256
Severity: Low
256             string calldata operatorName,



PermissionedPool.sol#257
Severity: Low
257             address payable operatorRewardAddress,



PermissionedPool.sol#258
Severity: Low
258             address operatorAddress



PermissionedPool.sol#324
Severity: Low
324     error EmptyNameString();



PermissionedPool.sol#324
Severity: Low
324     error EmptyNameString();



PermissionedPool.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionedPool.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionedPool.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionedPool.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionedPool.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionedPool.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionedPool.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionedPool.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionedPool.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionedPool.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionedPool.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionedPool.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionedPool.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionedPool.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionedPool.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionedPool.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionedPool.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



PermissionedPool.sol#396
Severity: Low
396         bytes calldata _depositSignature



PermissionedPool.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionedPool.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionedPool.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionedPool.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionedPool.sol#437
Severity: Low
437     error ZeroAddress();



PermissionedPool.sol#437
Severity: Low
437     error ZeroAddress();



PermissionedPool.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionedPool.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionedPool.sol#439
Severity: Low
439     error CallerNotManager();



PermissionedPool.sol#439
Severity: Low
439     error CallerNotManager();



PermissionedPool.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionedPool.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionedPool.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionedPool.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionedPool.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionedPool.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionedPool.sol#443
Severity: Low
443     error TransferFailed();



PermissionedPool.sol#443
Severity: Low
443     error TransferFailed();



PermissionedPool.sol#636
Severity: Low
636     error UnsupportedOperation();



PermissionedPool.sol#636
Severity: Low
636     error UnsupportedOperation();



PermissionedPool.sol#637
Severity: Low
637     error InvalidCommission();



PermissionedPool.sol#637
Severity: Low
637     error InvalidCommission();



PermissionedPool.sol#638
Severity: Low
638     error CouldNotDetermineExcessETH();



PermissionedPool.sol#638
Severity: Low
638     error CouldNotDetermineExcessETH();



PermissionedPool.sol#697
Severity: Low
697         bytes calldata withdrawal_credentials,



PermissionedPool.sol#698
Severity: Low
698         bytes calldata signature,



PermissionedPool.sol#698
Severity: Low
698         bytes calldata signature,



PermissionedPool.sol#699
Severity: Low
699         bytes32 deposit_data_root



PermissionedPool.sol#713
Severity: Low
713     error InvalidAmountProvided();



PermissionedPool.sol#713
Severity: Low
713     error InvalidAmountProvided();



PermissionedPool.sol#714
Severity: Low
714     error TransferFailed();



PermissionedPool.sol#714
Severity: Low
714     error TransferFailed();



PermissionedPool.sol#715
Severity: Low
715     error InSufficientBalance();



PermissionedPool.sol#715
Severity: Low
715     error InSufficientBalance();



PermissionedPool.sol#731
Severity: Low
731     error InvalidDepositAmount();



PermissionedPool.sol#731
Severity: Low
731     error InvalidDepositAmount();



PermissionedPool.sol#732
Severity: Low
732     error UnsupportedOperation();



PermissionedPool.sol#732
Severity: Low
732     error UnsupportedOperation();



PermissionedPool.sol#733
Severity: Low
733     error InsufficientBalance();



PermissionedPool.sol#733
Severity: Low
733     error InsufficientBalance();



PermissionedPool.sol#734
Severity: Low
734     error TransferFailed();



PermissionedPool.sol#734
Severity: Low
734     error TransferFailed();



PermissionedPool.sol#735
Severity: Low
735     error PoolIdDoesNotExit();



PermissionedPool.sol#735
Severity: Low
735     error PoolIdDoesNotExit();



PermissionedPool.sol#736
Severity: Low
736     error CooldownNotComplete();



PermissionedPool.sol#736
Severity: Low
736     error CooldownNotComplete();



PermissionedPool.sol#737
Severity: Low
737     error UnsupportedOperationInSafeMode();



PermissionedPool.sol#737
Severity: Low
737     error UnsupportedOperationInSafeMode();



PermissionedPool.sol#787
Severity: Low
787     error NotAPermissionedNodeOperator();



PermissionedPool.sol#787
Severity: Low
787     error NotAPermissionedNodeOperator();



PermissionedPool.sol#788
Severity: Low
788     error OperatorAlreadyDeactivate();



PermissionedPool.sol#788
Severity: Low
788     error OperatorAlreadyDeactivate();



PermissionedPool.sol#789
Severity: Low
789     error OperatorAlreadyActive();



PermissionedPool.sol#789
Severity: Low
789     error OperatorAlreadyActive();



PermissionedPool.sol#790
Severity: Low
790     error MaxOperatorLimitReached();



PermissionedPool.sol#790
Severity: Low
790     error MaxOperatorLimitReached();



PermissionedPool.sol#821
Severity: Low
821         returns (address mevFeeRecipientAddress);



PermissionedPool.sol#825
Severity: Low
825         bytes[] calldata _preDepositSignature,



PermissionedPool.sol#826
Severity: Low
826         bytes[] calldata _depositSignature



PermissionedPool.sol#1228
Severity: Low
1228     function sendValue(address payable recipient, uint256 amount) internal {



PermissionedPool.sol#1228
Severity: Low
1228     function sendValue(address payable recipient, uint256 amount) internal {



PermissionedPool.sol#1229
Severity: Low
1229         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedPool.sol#1229
Severity: Low
1229         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedPool.sol#1229
Severity: Low
1229         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedPool.sol#1229
Severity: Low
1229         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionedPool.sol#1231
Severity: Low
1231         (bool success, ) = recipient.call{value: amount}("");



PermissionedPool.sol#1231
Severity: Low
1231         (bool success, ) = recipient.call{value: amount}("");



PermissionedPool.sol#1231
Severity: Low
1231         (bool success, ) = recipient.call{value: amount}("");



PermissionedPool.sol#2408
Severity: Low
2408     receive() external payable {



PermissionedPool.sol#2409
Severity: Low
2409         revert UnsupportedOperation();



PermissionedPool.sol#2409
Severity: Low
2409         revert UnsupportedOperation();



```

### PermissionlessNodeRegistry.sol

```

PermissionlessNodeRegistry.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



PermissionlessNodeRegistry.sol#393
Severity: Low
393     function onlyValidKeys(



PermissionlessNodeRegistry.sol#635
Severity: Low
635     function preDepositOnBeaconChain(



PermissionlessNodeRegistry.sol#827
Severity: Low
827     function onboardNodeOperator(



PermissionlessNodeRegistry.sol#833
Severity: Low
833     function addValidatorKeys(



PermissionlessNodeRegistry.sol#851
Severity: Low
851     function updateOperatorDetails(string calldata _operatorName, address payable _rewardAddress) external;



PermissionlessNodeRegistry.sol#937
Severity: Low
937     function sendValue(address payable recipient, uint256 amount) internal {



PermissionlessNodeRegistry.sol#2323
Severity: Low
2323     constructor() {



PermissionlessNodeRegistry.sol#2350
Severity: Low
2350     function onboardNodeOperator(



PermissionlessNodeRegistry.sol#6
Severity: Low
6     error InvalidLimits();



PermissionlessNodeRegistry.sol#6
Severity: Low
6     error InvalidLimits();



PermissionlessNodeRegistry.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionlessNodeRegistry.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionlessNodeRegistry.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionlessNodeRegistry.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionlessNodeRegistry.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionlessNodeRegistry.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionlessNodeRegistry.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionlessNodeRegistry.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionlessNodeRegistry.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionlessNodeRegistry.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionlessNodeRegistry.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionlessNodeRegistry.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionlessNodeRegistry.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionlessNodeRegistry.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionlessNodeRegistry.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionlessNodeRegistry.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionlessNodeRegistry.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionlessNodeRegistry.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionlessNodeRegistry.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionlessNodeRegistry.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionlessNodeRegistry.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionlessNodeRegistry.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionlessNodeRegistry.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionlessNodeRegistry.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionlessNodeRegistry.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionlessNodeRegistry.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionlessNodeRegistry.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionlessNodeRegistry.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionlessNodeRegistry.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionlessNodeRegistry.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionlessNodeRegistry.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionlessNodeRegistry.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionlessNodeRegistry.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionlessNodeRegistry.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionlessNodeRegistry.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionlessNodeRegistry.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionlessNodeRegistry.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



PermissionlessNodeRegistry.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



PermissionlessNodeRegistry.sol#240
Severity: Low
240             bytes calldata pubkey,



PermissionlessNodeRegistry.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionlessNodeRegistry.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionlessNodeRegistry.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionlessNodeRegistry.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionlessNodeRegistry.sol#243
Severity: Low
243             address withdrawVaultAddress,



PermissionlessNodeRegistry.sol#244
Severity: Low
244             uint256 operatorId,



PermissionlessNodeRegistry.sol#245
Severity: Low
245             uint256 depositTime,



PermissionlessNodeRegistry.sol#246
Severity: Low
246             uint256 withdrawnTime



PermissionlessNodeRegistry.sol#256
Severity: Low
256             string calldata operatorName,



PermissionlessNodeRegistry.sol#257
Severity: Low
257             address payable operatorRewardAddress,



PermissionlessNodeRegistry.sol#258
Severity: Low
258             address operatorAddress



PermissionlessNodeRegistry.sol#324
Severity: Low
324     error EmptyNameString();



PermissionlessNodeRegistry.sol#324
Severity: Low
324     error EmptyNameString();



PermissionlessNodeRegistry.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionlessNodeRegistry.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionlessNodeRegistry.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionlessNodeRegistry.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionlessNodeRegistry.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionlessNodeRegistry.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionlessNodeRegistry.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionlessNodeRegistry.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionlessNodeRegistry.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionlessNodeRegistry.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionlessNodeRegistry.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionlessNodeRegistry.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionlessNodeRegistry.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionlessNodeRegistry.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionlessNodeRegistry.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionlessNodeRegistry.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionlessNodeRegistry.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



PermissionlessNodeRegistry.sol#396
Severity: Low
396         bytes calldata _depositSignature



PermissionlessNodeRegistry.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionlessNodeRegistry.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionlessNodeRegistry.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionlessNodeRegistry.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionlessNodeRegistry.sol#437
Severity: Low
437     error ZeroAddress();



PermissionlessNodeRegistry.sol#437
Severity: Low
437     error ZeroAddress();



PermissionlessNodeRegistry.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionlessNodeRegistry.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionlessNodeRegistry.sol#439
Severity: Low
439     error CallerNotManager();



PermissionlessNodeRegistry.sol#439
Severity: Low
439     error CallerNotManager();



PermissionlessNodeRegistry.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionlessNodeRegistry.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionlessNodeRegistry.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionlessNodeRegistry.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionlessNodeRegistry.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionlessNodeRegistry.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionlessNodeRegistry.sol#443
Severity: Low
443     error TransferFailed();



PermissionlessNodeRegistry.sol#443
Severity: Low
443     error TransferFailed();



PermissionlessNodeRegistry.sol#637
Severity: Low
637         bytes[] calldata _preDepositSignature,



PermissionlessNodeRegistry.sol#638
Severity: Low
638         uint256 _operatorId,



PermissionlessNodeRegistry.sol#639
Severity: Low
639         uint256 _operatorTotalKeys



PermissionlessNodeRegistry.sol#652
Severity: Low
652     error NotEnoughRewardToWithdraw();



PermissionlessNodeRegistry.sol#652
Severity: Low
652     error NotEnoughRewardToWithdraw();



PermissionlessNodeRegistry.sol#653
Severity: Low
653     error ETHTransferFailed(address recipient, uint256 amount);



PermissionlessNodeRegistry.sol#653
Severity: Low
653     error ETHTransferFailed(address recipient, uint256 amount);



PermissionlessNodeRegistry.sol#653
Severity: Low
653     error ETHTransferFailed(address recipient, uint256 amount);



PermissionlessNodeRegistry.sol#666
Severity: Low
666     error InvalidAmountProvided();



PermissionlessNodeRegistry.sol#666
Severity: Low
666     error InvalidAmountProvided();



PermissionlessNodeRegistry.sol#667
Severity: Low
667     error TransferFailed();



PermissionlessNodeRegistry.sol#667
Severity: Low
667     error TransferFailed();



PermissionlessNodeRegistry.sol#668
Severity: Low
668     error InSufficientBalance();



PermissionlessNodeRegistry.sol#668
Severity: Low
668     error InSufficientBalance();



PermissionlessNodeRegistry.sol#684
Severity: Low
684     error InvalidRewardAmount();



PermissionlessNodeRegistry.sol#684
Severity: Low
684     error InvalidRewardAmount();



PermissionlessNodeRegistry.sol#685
Severity: Low
685     error NotEnoughRewardToDistribute();



PermissionlessNodeRegistry.sol#685
Severity: Low
685     error NotEnoughRewardToDistribute();



PermissionlessNodeRegistry.sol#686
Severity: Low
686     error CallerNotNodeRegistryContract();



PermissionlessNodeRegistry.sol#686
Severity: Low
686     error CallerNotNodeRegistryContract();



PermissionlessNodeRegistry.sol#726
Severity: Low
726     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



PermissionlessNodeRegistry.sol#726
Severity: Low
726     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



PermissionlessNodeRegistry.sol#727
Severity: Low
727     error InvalidPoolId();



PermissionlessNodeRegistry.sol#727
Severity: Low
727     error InvalidPoolId();



PermissionlessNodeRegistry.sol#728
Severity: Low
728     error InvalidPoolLimit();



PermissionlessNodeRegistry.sol#728
Severity: Low
728     error InvalidPoolLimit();



PermissionlessNodeRegistry.sol#729
Severity: Low
729     error SDTransferFailed();



PermissionlessNodeRegistry.sol#729
Severity: Low
729     error SDTransferFailed();



PermissionlessNodeRegistry.sol#730
Severity: Low
730     error NoStateChange();



PermissionlessNodeRegistry.sol#730
Severity: Low
730     error NoStateChange();



PermissionlessNodeRegistry.sol#790
Severity: Low
790     error TransferFailed();



PermissionlessNodeRegistry.sol#790
Severity: Low
790     error TransferFailed();



PermissionlessNodeRegistry.sol#791
Severity: Low
791     error InvalidBondEthValue();



PermissionlessNodeRegistry.sol#791
Severity: Low
791     error InvalidBondEthValue();



PermissionlessNodeRegistry.sol#792
Severity: Low
792     error InSufficientBalance();



PermissionlessNodeRegistry.sol#792
Severity: Low
792     error InSufficientBalance();



PermissionlessNodeRegistry.sol#793
Severity: Low
793     error CooldownNotComplete();



PermissionlessNodeRegistry.sol#793
Severity: Low
793     error CooldownNotComplete();



PermissionlessNodeRegistry.sol#794
Severity: Low
794     error NoChangeInState();



PermissionlessNodeRegistry.sol#794
Severity: Low
794     error NoChangeInState();



PermissionlessNodeRegistry.sol#829
Severity: Low
829         string calldata _operatorName,



PermissionlessNodeRegistry.sol#830
Severity: Low
830         address payable _operatorRewardAddress



PermissionlessNodeRegistry.sol#831
Severity: Low
831     ) external returns (address mevFeeRecipientAddress);



PermissionlessNodeRegistry.sol#835
Severity: Low
835         bytes[] calldata _preDepositSignature,



PermissionlessNodeRegistry.sol#836
Severity: Low
836         bytes[] calldata _depositSignature



PermissionlessNodeRegistry.sol#937
Severity: Low
937     function sendValue(address payable recipient, uint256 amount) internal {



PermissionlessNodeRegistry.sol#937
Severity: Low
937     function sendValue(address payable recipient, uint256 amount) internal {



PermissionlessNodeRegistry.sol#938
Severity: Low
938         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessNodeRegistry.sol#938
Severity: Low
938         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessNodeRegistry.sol#938
Severity: Low
938         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessNodeRegistry.sol#938
Severity: Low
938         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessNodeRegistry.sol#940
Severity: Low
940         (bool success, ) = recipient.call{value: amount}("");



PermissionlessNodeRegistry.sol#940
Severity: Low
940         (bool success, ) = recipient.call{value: amount}("");



PermissionlessNodeRegistry.sol#940
Severity: Low
940         (bool success, ) = recipient.call{value: amount}("");



PermissionlessNodeRegistry.sol#2352
Severity: Low
2352         string calldata _operatorName,



PermissionlessNodeRegistry.sol#2353
Severity: Low
2353         address payable _operatorRewardAddress



PermissionlessNodeRegistry.sol#2354
Severity: Low
2354     ) external override whenNotPaused returns (address feeRecipientAddress) {



PermissionlessNodeRegistry.sol#2354
Severity: Low
2354     ) external override whenNotPaused returns (address feeRecipientAddress) {



PermissionlessNodeRegistry.sol#2355
Severity: Low
2355         address poolUtils = staderConfig.getPoolUtils();



PermissionlessNodeRegistry.sol#2356
Severity: Low
2356         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionlessPool()) {



PermissionlessNodeRegistry.sol#2356
Severity: Low
2356         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionlessPool()) {



PermissionlessNodeRegistry.sol#2356
Severity: Low
2356         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionlessPool()) {



PermissionlessNodeRegistry.sol#2356
Severity: Low
2356         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionlessPool()) {



PermissionlessNodeRegistry.sol#2356
Severity: Low
2356         if (IPoolUtils(poolUtils).poolAddressById(POOL_ID) != staderConfig.getPermissionlessPool()) {



PermissionlessNodeRegistry.sol#2357
Severity: Low
2357             revert DuplicatePoolIDOrPoolNotAdded();



PermissionlessNodeRegistry.sol#2357
Severity: Low
2357             revert DuplicatePoolIDOrPoolNotAdded();



```

### PermissionlessPool.sol

```

PermissionlessPool.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



PermissionlessPool.sol#393
Severity: Low
393     function onlyValidKeys(



PermissionlessPool.sol#695
Severity: Low
695     function deposit(



PermissionlessPool.sol#806
Severity: Low
806     function onboardNodeOperator(



PermissionlessPool.sol#812
Severity: Low
812     function addValidatorKeys(



PermissionlessPool.sol#830
Severity: Low
830     function updateOperatorDetails(string calldata _operatorName, address payable _rewardAddress) external;



PermissionlessPool.sol#1213
Severity: Low
1213     function sendValue(address payable recipient, uint256 amount) internal {



PermissionlessPool.sol#2377
Severity: Low
2377     constructor() {



PermissionlessPool.sol#6
Severity: Low
6     error InvalidLimits();



PermissionlessPool.sol#6
Severity: Low
6     error InvalidLimits();



PermissionlessPool.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionlessPool.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PermissionlessPool.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionlessPool.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PermissionlessPool.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionlessPool.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PermissionlessPool.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionlessPool.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PermissionlessPool.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionlessPool.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PermissionlessPool.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionlessPool.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PermissionlessPool.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionlessPool.sol#198
Severity: Low
198     error maxKeyLimitReached();



PermissionlessPool.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionlessPool.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PermissionlessPool.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionlessPool.sol#200
Severity: Low
200     error InvalidKeyCount();



PermissionlessPool.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionlessPool.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PermissionlessPool.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionlessPool.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PermissionlessPool.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionlessPool.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PermissionlessPool.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionlessPool.sol#204
Severity: Low
204     error PageNumberIsZero();



PermissionlessPool.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionlessPool.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PermissionlessPool.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionlessPool.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PermissionlessPool.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionlessPool.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PermissionlessPool.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionlessPool.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PermissionlessPool.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionlessPool.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PermissionlessPool.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



PermissionlessPool.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



PermissionlessPool.sol#240
Severity: Low
240             bytes calldata pubkey,



PermissionlessPool.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionlessPool.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PermissionlessPool.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionlessPool.sol#242
Severity: Low
242             bytes calldata depositSignature,



PermissionlessPool.sol#243
Severity: Low
243             address withdrawVaultAddress,



PermissionlessPool.sol#244
Severity: Low
244             uint256 operatorId,



PermissionlessPool.sol#245
Severity: Low
245             uint256 depositTime,



PermissionlessPool.sol#246
Severity: Low
246             uint256 withdrawnTime



PermissionlessPool.sol#256
Severity: Low
256             string calldata operatorName,



PermissionlessPool.sol#257
Severity: Low
257             address payable operatorRewardAddress,



PermissionlessPool.sol#258
Severity: Low
258             address operatorAddress



PermissionlessPool.sol#324
Severity: Low
324     error EmptyNameString();



PermissionlessPool.sol#324
Severity: Low
324     error EmptyNameString();



PermissionlessPool.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionlessPool.sol#325
Severity: Low
325     error PoolIdNotPresent();



PermissionlessPool.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionlessPool.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PermissionlessPool.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionlessPool.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PermissionlessPool.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionlessPool.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PermissionlessPool.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionlessPool.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PermissionlessPool.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionlessPool.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PermissionlessPool.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionlessPool.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PermissionlessPool.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionlessPool.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PermissionlessPool.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



PermissionlessPool.sol#396
Severity: Low
396         bytes calldata _depositSignature



PermissionlessPool.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionlessPool.sol#410
Severity: Low
410     error CallerNotOwner();



PermissionlessPool.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionlessPool.sol#411
Severity: Low
411     error AlreadyInitialized();



PermissionlessPool.sol#437
Severity: Low
437     error ZeroAddress();



PermissionlessPool.sol#437
Severity: Low
437     error ZeroAddress();



PermissionlessPool.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionlessPool.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PermissionlessPool.sol#439
Severity: Low
439     error CallerNotManager();



PermissionlessPool.sol#439
Severity: Low
439     error CallerNotManager();



PermissionlessPool.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionlessPool.sol#440
Severity: Low
440     error CallerNotOperator();



PermissionlessPool.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionlessPool.sol#441
Severity: Low
441     error CallerNotStaderContract();



PermissionlessPool.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionlessPool.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PermissionlessPool.sol#443
Severity: Low
443     error TransferFailed();



PermissionlessPool.sol#443
Severity: Low
443     error TransferFailed();



PermissionlessPool.sol#636
Severity: Low
636     error UnsupportedOperation();



PermissionlessPool.sol#636
Severity: Low
636     error UnsupportedOperation();



PermissionlessPool.sol#637
Severity: Low
637     error InvalidCommission();



PermissionlessPool.sol#637
Severity: Low
637     error InvalidCommission();



PermissionlessPool.sol#638
Severity: Low
638     error CouldNotDetermineExcessETH();



PermissionlessPool.sol#638
Severity: Low
638     error CouldNotDetermineExcessETH();



PermissionlessPool.sol#697
Severity: Low
697         bytes calldata withdrawal_credentials,



PermissionlessPool.sol#698
Severity: Low
698         bytes calldata signature,



PermissionlessPool.sol#698
Severity: Low
698         bytes calldata signature,



PermissionlessPool.sol#699
Severity: Low
699         bytes32 deposit_data_root



PermissionlessPool.sol#713
Severity: Low
713     error InvalidDepositAmount();



PermissionlessPool.sol#713
Severity: Low
713     error InvalidDepositAmount();



PermissionlessPool.sol#714
Severity: Low
714     error UnsupportedOperation();



PermissionlessPool.sol#714
Severity: Low
714     error UnsupportedOperation();



PermissionlessPool.sol#715
Severity: Low
715     error InsufficientBalance();



PermissionlessPool.sol#715
Severity: Low
715     error InsufficientBalance();



PermissionlessPool.sol#716
Severity: Low
716     error TransferFailed();



PermissionlessPool.sol#716
Severity: Low
716     error TransferFailed();



PermissionlessPool.sol#717
Severity: Low
717     error PoolIdDoesNotExit();



PermissionlessPool.sol#717
Severity: Low
717     error PoolIdDoesNotExit();



PermissionlessPool.sol#718
Severity: Low
718     error CooldownNotComplete();



PermissionlessPool.sol#718
Severity: Low
718     error CooldownNotComplete();



PermissionlessPool.sol#719
Severity: Low
719     error UnsupportedOperationInSafeMode();



PermissionlessPool.sol#719
Severity: Low
719     error UnsupportedOperationInSafeMode();



PermissionlessPool.sol#769
Severity: Low
769     error TransferFailed();



PermissionlessPool.sol#769
Severity: Low
769     error TransferFailed();



PermissionlessPool.sol#770
Severity: Low
770     error InvalidBondEthValue();



PermissionlessPool.sol#770
Severity: Low
770     error InvalidBondEthValue();



PermissionlessPool.sol#771
Severity: Low
771     error InSufficientBalance();



PermissionlessPool.sol#771
Severity: Low
771     error InSufficientBalance();



PermissionlessPool.sol#772
Severity: Low
772     error CooldownNotComplete();



PermissionlessPool.sol#772
Severity: Low
772     error CooldownNotComplete();



PermissionlessPool.sol#773
Severity: Low
773     error NoChangeInState();



PermissionlessPool.sol#773
Severity: Low
773     error NoChangeInState();



PermissionlessPool.sol#808
Severity: Low
808         string calldata _operatorName,



PermissionlessPool.sol#809
Severity: Low
809         address payable _operatorRewardAddress



PermissionlessPool.sol#810
Severity: Low
810     ) external returns (address mevFeeRecipientAddress);



PermissionlessPool.sol#814
Severity: Low
814         bytes[] calldata _preDepositSignature,



PermissionlessPool.sol#815
Severity: Low
815         bytes[] calldata _depositSignature



PermissionlessPool.sol#1213
Severity: Low
1213     function sendValue(address payable recipient, uint256 amount) internal {



PermissionlessPool.sol#1213
Severity: Low
1213     function sendValue(address payable recipient, uint256 amount) internal {



PermissionlessPool.sol#1214
Severity: Low
1214         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessPool.sol#1214
Severity: Low
1214         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessPool.sol#1214
Severity: Low
1214         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessPool.sol#1214
Severity: Low
1214         require(address(this).balance >= amount, "Address: insufficient balance");



PermissionlessPool.sol#1216
Severity: Low
1216         (bool success, ) = recipient.call{value: amount}("");



PermissionlessPool.sol#1216
Severity: Low
1216         (bool success, ) = recipient.call{value: amount}("");



PermissionlessPool.sol#1216
Severity: Low
1216         (bool success, ) = recipient.call{value: amount}("");



PermissionlessPool.sol#2393
Severity: Low
2393     receive() external payable {



PermissionlessPool.sol#2394
Severity: Low
2394         revert UnsupportedOperation();



PermissionlessPool.sol#2394
Severity: Low
2394         revert UnsupportedOperation();



```

### PoolSelector.sol

```

PoolSelector.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



PoolSelector.sol#393
Severity: Low
393     function onlyValidKeys(



PoolSelector.sol#1221
Severity: Low
1221     function sendValue(address payable recipient, uint256 amount) internal {



PoolSelector.sol#2304
Severity: Low
2304     constructor() {



PoolSelector.sol#6
Severity: Low
6     error InvalidLimits();



PoolSelector.sol#6
Severity: Low
6     error InvalidLimits();



PoolSelector.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PoolSelector.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PoolSelector.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PoolSelector.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PoolSelector.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PoolSelector.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PoolSelector.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PoolSelector.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PoolSelector.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PoolSelector.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PoolSelector.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PoolSelector.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PoolSelector.sol#198
Severity: Low
198     error maxKeyLimitReached();



PoolSelector.sol#198
Severity: Low
198     error maxKeyLimitReached();



PoolSelector.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PoolSelector.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PoolSelector.sol#200
Severity: Low
200     error InvalidKeyCount();



PoolSelector.sol#200
Severity: Low
200     error InvalidKeyCount();



PoolSelector.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PoolSelector.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PoolSelector.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PoolSelector.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PoolSelector.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PoolSelector.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PoolSelector.sol#204
Severity: Low
204     error PageNumberIsZero();



PoolSelector.sol#204
Severity: Low
204     error PageNumberIsZero();



PoolSelector.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PoolSelector.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PoolSelector.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PoolSelector.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PoolSelector.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PoolSelector.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PoolSelector.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PoolSelector.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PoolSelector.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PoolSelector.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PoolSelector.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



PoolSelector.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



PoolSelector.sol#240
Severity: Low
240             bytes calldata pubkey,



PoolSelector.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PoolSelector.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PoolSelector.sol#242
Severity: Low
242             bytes calldata depositSignature,



PoolSelector.sol#242
Severity: Low
242             bytes calldata depositSignature,



PoolSelector.sol#243
Severity: Low
243             address withdrawVaultAddress,



PoolSelector.sol#244
Severity: Low
244             uint256 operatorId,



PoolSelector.sol#245
Severity: Low
245             uint256 depositTime,



PoolSelector.sol#246
Severity: Low
246             uint256 withdrawnTime



PoolSelector.sol#256
Severity: Low
256             string calldata operatorName,



PoolSelector.sol#257
Severity: Low
257             address payable operatorRewardAddress,



PoolSelector.sol#258
Severity: Low
258             address operatorAddress



PoolSelector.sol#324
Severity: Low
324     error EmptyNameString();



PoolSelector.sol#324
Severity: Low
324     error EmptyNameString();



PoolSelector.sol#325
Severity: Low
325     error PoolIdNotPresent();



PoolSelector.sol#325
Severity: Low
325     error PoolIdNotPresent();



PoolSelector.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PoolSelector.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PoolSelector.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PoolSelector.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PoolSelector.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PoolSelector.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PoolSelector.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PoolSelector.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PoolSelector.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PoolSelector.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PoolSelector.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PoolSelector.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PoolSelector.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PoolSelector.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PoolSelector.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



PoolSelector.sol#396
Severity: Low
396         bytes calldata _depositSignature



PoolSelector.sol#410
Severity: Low
410     error CallerNotOwner();



PoolSelector.sol#410
Severity: Low
410     error CallerNotOwner();



PoolSelector.sol#411
Severity: Low
411     error AlreadyInitialized();



PoolSelector.sol#411
Severity: Low
411     error AlreadyInitialized();



PoolSelector.sol#437
Severity: Low
437     error ZeroAddress();



PoolSelector.sol#437
Severity: Low
437     error ZeroAddress();



PoolSelector.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PoolSelector.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PoolSelector.sol#439
Severity: Low
439     error CallerNotManager();



PoolSelector.sol#439
Severity: Low
439     error CallerNotManager();



PoolSelector.sol#440
Severity: Low
440     error CallerNotOperator();



PoolSelector.sol#440
Severity: Low
440     error CallerNotOperator();



PoolSelector.sol#441
Severity: Low
441     error CallerNotStaderContract();



PoolSelector.sol#441
Severity: Low
441     error CallerNotStaderContract();



PoolSelector.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PoolSelector.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PoolSelector.sol#443
Severity: Low
443     error TransferFailed();



PoolSelector.sol#443
Severity: Low
443     error TransferFailed();



PoolSelector.sol#604
Severity: Low
604     error InvalidTargetWeight();



PoolSelector.sol#604
Severity: Low
604     error InvalidTargetWeight();



PoolSelector.sol#605
Severity: Low
605     error InvalidNewTargetInput();



PoolSelector.sol#605
Severity: Low
605     error InvalidNewTargetInput();



PoolSelector.sol#606
Severity: Low
606     error InvalidSumOfPoolWeights();



PoolSelector.sol#606
Severity: Low
606     error InvalidSumOfPoolWeights();



PoolSelector.sol#1221
Severity: Low
1221     function sendValue(address payable recipient, uint256 amount) internal {



PoolSelector.sol#1221
Severity: Low
1221     function sendValue(address payable recipient, uint256 amount) internal {



PoolSelector.sol#1222
Severity: Low
1222         require(address(this).balance >= amount, "Address: insufficient balance");



PoolSelector.sol#1222
Severity: Low
1222         require(address(this).balance >= amount, "Address: insufficient balance");



PoolSelector.sol#1222
Severity: Low
1222         require(address(this).balance >= amount, "Address: insufficient balance");



PoolSelector.sol#1222
Severity: Low
1222         require(address(this).balance >= amount, "Address: insufficient balance");



PoolSelector.sol#1224
Severity: Low
1224         (bool success, ) = recipient.call{value: amount}("");



PoolSelector.sol#1224
Severity: Low
1224         (bool success, ) = recipient.call{value: amount}("");



PoolSelector.sol#1224
Severity: Low
1224         (bool success, ) = recipient.call{value: amount}("");



```

### PoolUtils.sol

```

PoolUtils.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



PoolUtils.sol#393
Severity: Low
393     function onlyValidKeys(



PoolUtils.sol#798
Severity: Low
798     function sendValue(address payable recipient, uint256 amount) internal {



PoolUtils.sol#1878
Severity: Low
1878     constructor() {



PoolUtils.sol#2082
Severity: Low
2082     function onlyValidKeys(



PoolUtils.sol#6
Severity: Low
6     error InvalidLimits();



PoolUtils.sol#6
Severity: Low
6     error InvalidLimits();



PoolUtils.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PoolUtils.sol#7
Severity: Low
7     error InvalidMinDepositValue();



PoolUtils.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PoolUtils.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



PoolUtils.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PoolUtils.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



PoolUtils.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PoolUtils.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



PoolUtils.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PoolUtils.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



PoolUtils.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PoolUtils.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



PoolUtils.sol#198
Severity: Low
198     error maxKeyLimitReached();



PoolUtils.sol#198
Severity: Low
198     error maxKeyLimitReached();



PoolUtils.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PoolUtils.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



PoolUtils.sol#200
Severity: Low
200     error InvalidKeyCount();



PoolUtils.sol#200
Severity: Low
200     error InvalidKeyCount();



PoolUtils.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PoolUtils.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



PoolUtils.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PoolUtils.sol#202
Severity: Low
202     error OperatorIsDeactivate();



PoolUtils.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PoolUtils.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



PoolUtils.sol#204
Severity: Low
204     error PageNumberIsZero();



PoolUtils.sol#204
Severity: Low
204     error PageNumberIsZero();



PoolUtils.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PoolUtils.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



PoolUtils.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PoolUtils.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



PoolUtils.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PoolUtils.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



PoolUtils.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PoolUtils.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



PoolUtils.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PoolUtils.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



PoolUtils.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



PoolUtils.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



PoolUtils.sol#240
Severity: Low
240             bytes calldata pubkey,



PoolUtils.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PoolUtils.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



PoolUtils.sol#242
Severity: Low
242             bytes calldata depositSignature,



PoolUtils.sol#242
Severity: Low
242             bytes calldata depositSignature,



PoolUtils.sol#243
Severity: Low
243             address withdrawVaultAddress,



PoolUtils.sol#244
Severity: Low
244             uint256 operatorId,



PoolUtils.sol#245
Severity: Low
245             uint256 depositTime,



PoolUtils.sol#246
Severity: Low
246             uint256 withdrawnTime



PoolUtils.sol#256
Severity: Low
256             string calldata operatorName,



PoolUtils.sol#257
Severity: Low
257             address payable operatorRewardAddress,



PoolUtils.sol#258
Severity: Low
258             address operatorAddress



PoolUtils.sol#324
Severity: Low
324     error EmptyNameString();



PoolUtils.sol#324
Severity: Low
324     error EmptyNameString();



PoolUtils.sol#325
Severity: Low
325     error PoolIdNotPresent();



PoolUtils.sol#325
Severity: Low
325     error PoolIdNotPresent();



PoolUtils.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PoolUtils.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



PoolUtils.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PoolUtils.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



PoolUtils.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PoolUtils.sol#328
Severity: Low
328     error NameCrossedMaxLength();



PoolUtils.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PoolUtils.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



PoolUtils.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PoolUtils.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



PoolUtils.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PoolUtils.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



PoolUtils.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PoolUtils.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



PoolUtils.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



PoolUtils.sol#396
Severity: Low
396         bytes calldata _depositSignature



PoolUtils.sol#410
Severity: Low
410     error CallerNotOwner();



PoolUtils.sol#410
Severity: Low
410     error CallerNotOwner();



PoolUtils.sol#411
Severity: Low
411     error AlreadyInitialized();



PoolUtils.sol#411
Severity: Low
411     error AlreadyInitialized();



PoolUtils.sol#437
Severity: Low
437     error ZeroAddress();



PoolUtils.sol#437
Severity: Low
437     error ZeroAddress();



PoolUtils.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PoolUtils.sol#438
Severity: Low
438     error InvalidPubkeyLength();



PoolUtils.sol#439
Severity: Low
439     error CallerNotManager();



PoolUtils.sol#439
Severity: Low
439     error CallerNotManager();



PoolUtils.sol#440
Severity: Low
440     error CallerNotOperator();



PoolUtils.sol#440
Severity: Low
440     error CallerNotOperator();



PoolUtils.sol#441
Severity: Low
441     error CallerNotStaderContract();



PoolUtils.sol#441
Severity: Low
441     error CallerNotStaderContract();



PoolUtils.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PoolUtils.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



PoolUtils.sol#443
Severity: Low
443     error TransferFailed();



PoolUtils.sol#443
Severity: Low
443     error TransferFailed();



PoolUtils.sol#604
Severity: Low
604     error UnsupportedOperation();



PoolUtils.sol#604
Severity: Low
604     error UnsupportedOperation();



PoolUtils.sol#605
Severity: Low
605     error InvalidCommission();



PoolUtils.sol#605
Severity: Low
605     error InvalidCommission();



PoolUtils.sol#606
Severity: Low
606     error CouldNotDetermineExcessETH();



PoolUtils.sol#606
Severity: Low
606     error CouldNotDetermineExcessETH();



PoolUtils.sol#798
Severity: Low
798     function sendValue(address payable recipient, uint256 amount) internal {



PoolUtils.sol#798
Severity: Low
798     function sendValue(address payable recipient, uint256 amount) internal {



PoolUtils.sol#799
Severity: Low
799         require(address(this).balance >= amount, "Address: insufficient balance");



PoolUtils.sol#799
Severity: Low
799         require(address(this).balance >= amount, "Address: insufficient balance");



PoolUtils.sol#799
Severity: Low
799         require(address(this).balance >= amount, "Address: insufficient balance");



PoolUtils.sol#799
Severity: Low
799         require(address(this).balance >= amount, "Address: insufficient balance");



PoolUtils.sol#801
Severity: Low
801         (bool success, ) = recipient.call{value: amount}("");



PoolUtils.sol#801
Severity: Low
801         (bool success, ) = recipient.call{value: amount}("");



PoolUtils.sol#801
Severity: Low
801         (bool success, ) = recipient.call{value: amount}("");



PoolUtils.sol#2084
Severity: Low
2084         bytes calldata _preDepositSignature,



PoolUtils.sol#2085
Severity: Low
2085         bytes calldata _depositSignature



PoolUtils.sol#2087
Severity: Low
2087         if (_pubkey.length != PUBKEY_LENGTH) {



PoolUtils.sol#2088
Severity: Low
2088             revert InvalidLengthOfPubkey();



PoolUtils.sol#2088
Severity: Low
2088             revert InvalidLengthOfPubkey();



```

### SDCollateral.sol

```

SDCollateral.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



SDCollateral.sol#393
Severity: Low
393     function onlyValidKeys(



SDCollateral.sol#800
Severity: Low
800     function claim(



SDCollateral.sol#1496
Severity: Low
1496     function sendValue(address payable recipient, uint256 amount) internal {



SDCollateral.sol#2731
Severity: Low
2731     constructor() {



SDCollateral.sol#6
Severity: Low
6     error InvalidLimits();



SDCollateral.sol#6
Severity: Low
6     error InvalidLimits();



SDCollateral.sol#7
Severity: Low
7     error InvalidMinDepositValue();



SDCollateral.sol#7
Severity: Low
7     error InvalidMinDepositValue();



SDCollateral.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



SDCollateral.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



SDCollateral.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



SDCollateral.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



SDCollateral.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



SDCollateral.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



SDCollateral.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



SDCollateral.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



SDCollateral.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



SDCollateral.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



SDCollateral.sol#198
Severity: Low
198     error maxKeyLimitReached();



SDCollateral.sol#198
Severity: Low
198     error maxKeyLimitReached();



SDCollateral.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



SDCollateral.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



SDCollateral.sol#200
Severity: Low
200     error InvalidKeyCount();



SDCollateral.sol#200
Severity: Low
200     error InvalidKeyCount();



SDCollateral.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



SDCollateral.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



SDCollateral.sol#202
Severity: Low
202     error OperatorIsDeactivate();



SDCollateral.sol#202
Severity: Low
202     error OperatorIsDeactivate();



SDCollateral.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



SDCollateral.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



SDCollateral.sol#204
Severity: Low
204     error PageNumberIsZero();



SDCollateral.sol#204
Severity: Low
204     error PageNumberIsZero();



SDCollateral.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



SDCollateral.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



SDCollateral.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



SDCollateral.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



SDCollateral.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



SDCollateral.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



SDCollateral.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



SDCollateral.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



SDCollateral.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



SDCollateral.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



SDCollateral.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



SDCollateral.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



SDCollateral.sol#240
Severity: Low
240             bytes calldata pubkey,



SDCollateral.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



SDCollateral.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



SDCollateral.sol#242
Severity: Low
242             bytes calldata depositSignature,



SDCollateral.sol#242
Severity: Low
242             bytes calldata depositSignature,



SDCollateral.sol#243
Severity: Low
243             address withdrawVaultAddress,



SDCollateral.sol#244
Severity: Low
244             uint256 operatorId,



SDCollateral.sol#245
Severity: Low
245             uint256 depositTime,



SDCollateral.sol#246
Severity: Low
246             uint256 withdrawnTime



SDCollateral.sol#256
Severity: Low
256             string calldata operatorName,



SDCollateral.sol#257
Severity: Low
257             address payable operatorRewardAddress,



SDCollateral.sol#258
Severity: Low
258             address operatorAddress



SDCollateral.sol#324
Severity: Low
324     error EmptyNameString();



SDCollateral.sol#324
Severity: Low
324     error EmptyNameString();



SDCollateral.sol#325
Severity: Low
325     error PoolIdNotPresent();



SDCollateral.sol#325
Severity: Low
325     error PoolIdNotPresent();



SDCollateral.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



SDCollateral.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



SDCollateral.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



SDCollateral.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



SDCollateral.sol#328
Severity: Low
328     error NameCrossedMaxLength();



SDCollateral.sol#328
Severity: Low
328     error NameCrossedMaxLength();



SDCollateral.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



SDCollateral.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



SDCollateral.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



SDCollateral.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



SDCollateral.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



SDCollateral.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



SDCollateral.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



SDCollateral.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



SDCollateral.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



SDCollateral.sol#396
Severity: Low
396         bytes calldata _depositSignature



SDCollateral.sol#410
Severity: Low
410     error CallerNotOwner();



SDCollateral.sol#410
Severity: Low
410     error CallerNotOwner();



SDCollateral.sol#411
Severity: Low
411     error AlreadyInitialized();



SDCollateral.sol#411
Severity: Low
411     error AlreadyInitialized();



SDCollateral.sol#437
Severity: Low
437     error ZeroAddress();



SDCollateral.sol#437
Severity: Low
437     error ZeroAddress();



SDCollateral.sol#438
Severity: Low
438     error InvalidPubkeyLength();



SDCollateral.sol#438
Severity: Low
438     error InvalidPubkeyLength();



SDCollateral.sol#439
Severity: Low
439     error CallerNotManager();



SDCollateral.sol#439
Severity: Low
439     error CallerNotManager();



SDCollateral.sol#440
Severity: Low
440     error CallerNotOperator();



SDCollateral.sol#440
Severity: Low
440     error CallerNotOperator();



SDCollateral.sol#441
Severity: Low
441     error CallerNotStaderContract();



SDCollateral.sol#441
Severity: Low
441     error CallerNotStaderContract();



SDCollateral.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



SDCollateral.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



SDCollateral.sol#443
Severity: Low
443     error TransferFailed();



SDCollateral.sol#443
Severity: Low
443     error TransferFailed();



SDCollateral.sol#616
Severity: Low
616     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



SDCollateral.sol#616
Severity: Low
616     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



SDCollateral.sol#617
Severity: Low
617     error InvalidPoolId();



SDCollateral.sol#617
Severity: Low
617     error InvalidPoolId();



SDCollateral.sol#618
Severity: Low
618     error InvalidPoolLimit();



SDCollateral.sol#618
Severity: Low
618     error InvalidPoolLimit();



SDCollateral.sol#619
Severity: Low
619     error SDTransferFailed();



SDCollateral.sol#619
Severity: Low
619     error SDTransferFailed();



SDCollateral.sol#620
Severity: Low
620     error NoStateChange();



SDCollateral.sol#620
Severity: Low
620     error NoStateChange();



SDCollateral.sol#680
Severity: Low
680     error InSufficientETH();



SDCollateral.sol#680
Severity: Low
680     error InSufficientETH();



SDCollateral.sol#681
Severity: Low
681     error ETHWithdrawFailed();



SDCollateral.sol#681
Severity: Low
681     error ETHWithdrawFailed();



SDCollateral.sol#682
Severity: Low
682     error AuctionEnded();



SDCollateral.sol#682
Severity: Low
682     error AuctionEnded();



SDCollateral.sol#683
Severity: Low
683     error AuctionNotEnded();



SDCollateral.sol#683
Severity: Low
683     error AuctionNotEnded();



SDCollateral.sol#684
Severity: Low
684     error ShortDuration();



SDCollateral.sol#684
Severity: Low
684     error ShortDuration();



SDCollateral.sol#685
Severity: Low
685     error notQualified();



SDCollateral.sol#685
Severity: Low
685     error notQualified();



SDCollateral.sol#686
Severity: Low
686     error AlreadyClaimed();



SDCollateral.sol#686
Severity: Low
686     error AlreadyClaimed();



SDCollateral.sol#687
Severity: Low
687     error NoBidPlaced();



SDCollateral.sol#687
Severity: Low
687     error NoBidPlaced();



SDCollateral.sol#688
Severity: Low
688     error BidWasSuccessful();



SDCollateral.sol#688
Severity: Low
688     error BidWasSuccessful();



SDCollateral.sol#689
Severity: Low
689     error InSufficientBid();



SDCollateral.sol#689
Severity: Low
689     error InSufficientBid();



SDCollateral.sol#690
Severity: Low
690     error LotWasAuctioned();



SDCollateral.sol#690
Severity: Low
690     error LotWasAuctioned();



SDCollateral.sol#691
Severity: Low
691     error SDTransferFailed();



SDCollateral.sol#691
Severity: Low
691     error SDTransferFailed();



SDCollateral.sol#770
Severity: Low
770     error ETHTransferFailed(address recipient, uint256 amount);



SDCollateral.sol#770
Severity: Low
770     error ETHTransferFailed(address recipient, uint256 amount);



SDCollateral.sol#770
Severity: Low
770     error ETHTransferFailed(address recipient, uint256 amount);



SDCollateral.sol#771
Severity: Low
771     error SDTransferFailed();



SDCollateral.sol#771
Severity: Low
771     error SDTransferFailed();



SDCollateral.sol#772
Severity: Low
772     error RewardAlreadyHandled();



SDCollateral.sol#772
Severity: Low
772     error RewardAlreadyHandled();



SDCollateral.sol#773
Severity: Low
773     error RewardAlreadyClaimed(address operator, uint256 cycle);



SDCollateral.sol#773
Severity: Low
773     error RewardAlreadyClaimed(address operator, uint256 cycle);



SDCollateral.sol#773
Severity: Low
773     error RewardAlreadyClaimed(address operator, uint256 cycle);



SDCollateral.sol#774
Severity: Low
774     error InsufficientETHRewards();



SDCollateral.sol#774
Severity: Low
774     error InsufficientETHRewards();



SDCollateral.sol#775
Severity: Low
775     error InsufficientSDRewards();



SDCollateral.sol#775
Severity: Low
775     error InsufficientSDRewards();



SDCollateral.sol#776
Severity: Low
776     error InvalidAmount();



SDCollateral.sol#776
Severity: Low
776     error InvalidAmount();



SDCollateral.sol#777
Severity: Low
777     error InvalidProof(uint256 cycle, address operator);



SDCollateral.sol#777
Severity: Low
777     error InvalidProof(uint256 cycle, address operator);



SDCollateral.sol#777
Severity: Low
777     error InvalidProof(uint256 cycle, address operator);



SDCollateral.sol#778
Severity: Low
778     error InvalidCycleIndex();



SDCollateral.sol#778
Severity: Low
778     error InvalidCycleIndex();



SDCollateral.sol#779
Severity: Low
779     error FutureCycleIndex();



SDCollateral.sol#779
Severity: Low
779     error FutureCycleIndex();



SDCollateral.sol#802
Severity: Low
802         uint256[] calldata _amountSD,



SDCollateral.sol#803
Severity: Low
803         uint256[] calldata _amountETH,



SDCollateral.sol#803
Severity: Low
803         uint256[] calldata _amountETH,



SDCollateral.sol#804
Severity: Low
804         bytes32[][] calldata _merkleProof



SDCollateral.sol#902
Severity: Low
902     error InvalidUpdate();



SDCollateral.sol#902
Severity: Low
902     error InvalidUpdate();



SDCollateral.sol#903
Severity: Low
903     error NodeAlreadyTrusted();



SDCollateral.sol#903
Severity: Low
903     error NodeAlreadyTrusted();



SDCollateral.sol#904
Severity: Low
904     error NodeNotTrusted();



SDCollateral.sol#904
Severity: Low
904     error NodeNotTrusted();



SDCollateral.sol#905
Severity: Low
905     error ZeroFrequency();



SDCollateral.sol#905
Severity: Low
905     error ZeroFrequency();



SDCollateral.sol#906
Severity: Low
906     error FrequencyUnchanged();



SDCollateral.sol#906
Severity: Low
906     error FrequencyUnchanged();



SDCollateral.sol#907
Severity: Low
907     error DuplicateSubmissionFromNode();



SDCollateral.sol#907
Severity: Low
907     error DuplicateSubmissionFromNode();



SDCollateral.sol#908
Severity: Low
908     error ReportingFutureBlockData();



SDCollateral.sol#908
Severity: Low
908     error ReportingFutureBlockData();



SDCollateral.sol#909
Severity: Low
909     error InvalidMerkleRootIndex();



SDCollateral.sol#909
Severity: Low
909     error InvalidMerkleRootIndex();



SDCollateral.sol#910
Severity: Low
910     error ReportingPreviousCycleData();



SDCollateral.sol#910
Severity: Low
910     error ReportingPreviousCycleData();



SDCollateral.sol#911
Severity: Low
911     error InvalidMAPDIndex();



SDCollateral.sol#911
Severity: Low
911     error InvalidMAPDIndex();



SDCollateral.sol#912
Severity: Low
912     error PageNumberAlreadyReported();



SDCollateral.sol#912
Severity: Low
912     error PageNumberAlreadyReported();



SDCollateral.sol#913
Severity: Low
913     error NotATrustedNode();



SDCollateral.sol#913
Severity: Low
913     error NotATrustedNode();



SDCollateral.sol#914
Severity: Low
914     error InvalidERDataSource();



SDCollateral.sol#914
Severity: Low
914     error InvalidERDataSource();



SDCollateral.sol#915
Severity: Low
915     error InspectionModeActive();



SDCollateral.sol#915
Severity: Low
915     error InspectionModeActive();



SDCollateral.sol#916
Severity: Low
916     error UpdateFrequencyNotSet();



SDCollateral.sol#916
Severity: Low
916     error UpdateFrequencyNotSet();



SDCollateral.sol#917
Severity: Low
917     error InvalidReportingBlock();



SDCollateral.sol#917
Severity: Low
917     error InvalidReportingBlock();



SDCollateral.sol#918
Severity: Low
918     error ERChangeLimitCrossed();



SDCollateral.sol#918
Severity: Low
918     error ERChangeLimitCrossed();



SDCollateral.sol#919
Severity: Low
919     error ERChangeLimitNotCrossed();



SDCollateral.sol#919
Severity: Low
919     error ERChangeLimitNotCrossed();



SDCollateral.sol#920
Severity: Low
920     error ERPermissibleChangeOutofBounds();



SDCollateral.sol#920
Severity: Low
920     error ERPermissibleChangeOutofBounds();



SDCollateral.sol#921
Severity: Low
921     error InsufficientTrustedNodes();



SDCollateral.sol#921
Severity: Low
921     error InsufficientTrustedNodes();



SDCollateral.sol#922
Severity: Low
922     error CooldownNotComplete();



SDCollateral.sol#922
Severity: Low
922     error CooldownNotComplete();



SDCollateral.sol#1496
Severity: Low
1496     function sendValue(address payable recipient, uint256 amount) internal {



SDCollateral.sol#1496
Severity: Low
1496     function sendValue(address payable recipient, uint256 amount) internal {



SDCollateral.sol#1497
Severity: Low
1497         require(address(this).balance >= amount, "Address: insufficient balance");



SDCollateral.sol#1497
Severity: Low
1497         require(address(this).balance >= amount, "Address: insufficient balance");



SDCollateral.sol#1497
Severity: Low
1497         require(address(this).balance >= amount, "Address: insufficient balance");



SDCollateral.sol#1497
Severity: Low
1497         require(address(this).balance >= amount, "Address: insufficient balance");



SDCollateral.sol#1499
Severity: Low
1499         (bool success, ) = recipient.call{value: amount}("");



SDCollateral.sol#1499
Severity: Low
1499         (bool success, ) = recipient.call{value: amount}("");



SDCollateral.sol#1499
Severity: Low
1499         (bool success, ) = recipient.call{value: amount}("");



```

### SocializingPool.sol

```

SocializingPool.sol#229
Severity: Low
229     function markValidatorReadyToDeposit(



SocializingPool.sol#394
Severity: Low
394     function onlyValidKeys(



SocializingPool.sol#656
Severity: Low
656     function claim(



SocializingPool.sol#794
Severity: Low
794     function onboardNodeOperator(



SocializingPool.sol#800
Severity: Low
800     function addValidatorKeys(



SocializingPool.sol#818
Severity: Low
818     function updateOperatorDetails(string calldata _operatorName, address payable _rewardAddress) external;



SocializingPool.sol#977
Severity: Low
977     function sendValue(address payable recipient, uint256 amount) internal {



SocializingPool.sol#2331
Severity: Low
2331     function multiProofVerifyCalldata(



SocializingPool.sol#2546
Severity: Low
2546     constructor() {



SocializingPool.sol#7
Severity: Low
7     error InvalidLimits();



SocializingPool.sol#7
Severity: Low
7     error InvalidLimits();



SocializingPool.sol#8
Severity: Low
8     error InvalidMinDepositValue();



SocializingPool.sol#8
Severity: Low
8     error InvalidMinDepositValue();



SocializingPool.sol#9
Severity: Low
9     error InvalidMaxDepositValue();



SocializingPool.sol#9
Severity: Low
9     error InvalidMaxDepositValue();



SocializingPool.sol#10
Severity: Low
10     error InvalidMinWithdrawValue();



SocializingPool.sol#10
Severity: Low
10     error InvalidMinWithdrawValue();



SocializingPool.sol#11
Severity: Low
11     error InvalidMaxWithdrawValue();



SocializingPool.sol#11
Severity: Low
11     error InvalidMaxWithdrawValue();



SocializingPool.sol#197
Severity: Low
197     error DuplicatePoolIDOrPoolNotAdded();



SocializingPool.sol#197
Severity: Low
197     error DuplicatePoolIDOrPoolNotAdded();



SocializingPool.sol#198
Severity: Low
198     error OperatorAlreadyOnBoardedInProtocol();



SocializingPool.sol#198
Severity: Low
198     error OperatorAlreadyOnBoardedInProtocol();



SocializingPool.sol#199
Severity: Low
199     error maxKeyLimitReached();



SocializingPool.sol#199
Severity: Low
199     error maxKeyLimitReached();



SocializingPool.sol#200
Severity: Low
200     error OperatorNotOnBoarded();



SocializingPool.sol#200
Severity: Low
200     error OperatorNotOnBoarded();



SocializingPool.sol#201
Severity: Low
201     error InvalidKeyCount();



SocializingPool.sol#201
Severity: Low
201     error InvalidKeyCount();



SocializingPool.sol#202
Severity: Low
202     error InvalidStartAndEndIndex();



SocializingPool.sol#202
Severity: Low
202     error InvalidStartAndEndIndex();



SocializingPool.sol#203
Severity: Low
203     error OperatorIsDeactivate();



SocializingPool.sol#203
Severity: Low
203     error OperatorIsDeactivate();



SocializingPool.sol#204
Severity: Low
204     error MisMatchingInputKeysSize();



SocializingPool.sol#204
Severity: Low
204     error MisMatchingInputKeysSize();



SocializingPool.sol#205
Severity: Low
205     error PageNumberIsZero();



SocializingPool.sol#205
Severity: Low
205     error PageNumberIsZero();



SocializingPool.sol#206
Severity: Low
206     error UNEXPECTED_STATUS();



SocializingPool.sol#206
Severity: Low
206     error UNEXPECTED_STATUS();



SocializingPool.sol#207
Severity: Low
207     error PubkeyAlreadyExist();



SocializingPool.sol#207
Severity: Low
207     error PubkeyAlreadyExist();



SocializingPool.sol#208
Severity: Low
208     error NotEnoughSDCollateral();



SocializingPool.sol#208
Severity: Low
208     error NotEnoughSDCollateral();



SocializingPool.sol#209
Severity: Low
209     error TooManyVerifiedKeysReported();



SocializingPool.sol#209
Severity: Low
209     error TooManyVerifiedKeysReported();



SocializingPool.sol#210
Severity: Low
210     error TooManyWithdrawnKeysReported();



SocializingPool.sol#210
Severity: Low
210     error TooManyWithdrawnKeysReported();



SocializingPool.sol#231
Severity: Low
231         bytes[] calldata _frontRunPubkey,



SocializingPool.sol#232
Severity: Low
232         bytes[] calldata _invalidSignaturePubkey



SocializingPool.sol#241
Severity: Low
241             bytes calldata pubkey,



SocializingPool.sol#242
Severity: Low
242             bytes calldata preDepositSignature,



SocializingPool.sol#242
Severity: Low
242             bytes calldata preDepositSignature,



SocializingPool.sol#243
Severity: Low
243             bytes calldata depositSignature,



SocializingPool.sol#243
Severity: Low
243             bytes calldata depositSignature,



SocializingPool.sol#244
Severity: Low
244             address withdrawVaultAddress,



SocializingPool.sol#245
Severity: Low
245             uint256 operatorId,



SocializingPool.sol#246
Severity: Low
246             uint256 depositTime,



SocializingPool.sol#247
Severity: Low
247             uint256 withdrawnTime



SocializingPool.sol#257
Severity: Low
257             string calldata operatorName,



SocializingPool.sol#258
Severity: Low
258             address payable operatorRewardAddress,



SocializingPool.sol#259
Severity: Low
259             address operatorAddress



SocializingPool.sol#325
Severity: Low
325     error EmptyNameString();



SocializingPool.sol#325
Severity: Low
325     error EmptyNameString();



SocializingPool.sol#326
Severity: Low
326     error PoolIdNotPresent();



SocializingPool.sol#326
Severity: Low
326     error PoolIdNotPresent();



SocializingPool.sol#327
Severity: Low
327     error PubkeyDoesNotExit();



SocializingPool.sol#327
Severity: Low
327     error PubkeyDoesNotExit();



SocializingPool.sol#328
Severity: Low
328     error PubkeyAlreadyExist();



SocializingPool.sol#328
Severity: Low
328     error PubkeyAlreadyExist();



SocializingPool.sol#329
Severity: Low
329     error NameCrossedMaxLength();



SocializingPool.sol#329
Severity: Low
329     error NameCrossedMaxLength();



SocializingPool.sol#330
Severity: Low
330     error InvalidLengthOfPubkey();



SocializingPool.sol#330
Severity: Low
330     error InvalidLengthOfPubkey();



SocializingPool.sol#331
Severity: Low
331     error OperatorIsNotOnboarded();



SocializingPool.sol#331
Severity: Low
331     error OperatorIsNotOnboarded();



SocializingPool.sol#332
Severity: Low
332     error InvalidLengthOfSignature();



SocializingPool.sol#332
Severity: Low
332     error InvalidLengthOfSignature();



SocializingPool.sol#333
Severity: Low
333     error ExistingOrMismatchingPoolId();



SocializingPool.sol#333
Severity: Low
333     error ExistingOrMismatchingPoolId();



SocializingPool.sol#396
Severity: Low
396         bytes calldata _preDepositSignature,



SocializingPool.sol#397
Severity: Low
397         bytes calldata _depositSignature



SocializingPool.sol#411
Severity: Low
411     error CallerNotOwner();



SocializingPool.sol#411
Severity: Low
411     error CallerNotOwner();



SocializingPool.sol#412
Severity: Low
412     error AlreadyInitialized();



SocializingPool.sol#412
Severity: Low
412     error AlreadyInitialized();



SocializingPool.sol#438
Severity: Low
438     error ZeroAddress();



SocializingPool.sol#438
Severity: Low
438     error ZeroAddress();



SocializingPool.sol#439
Severity: Low
439     error InvalidPubkeyLength();



SocializingPool.sol#439
Severity: Low
439     error InvalidPubkeyLength();



SocializingPool.sol#440
Severity: Low
440     error CallerNotManager();



SocializingPool.sol#440
Severity: Low
440     error CallerNotManager();



SocializingPool.sol#441
Severity: Low
441     error CallerNotOperator();



SocializingPool.sol#441
Severity: Low
441     error CallerNotOperator();



SocializingPool.sol#442
Severity: Low
442     error CallerNotStaderContract();



SocializingPool.sol#442
Severity: Low
442     error CallerNotStaderContract();



SocializingPool.sol#443
Severity: Low
443     error CallerNotWithdrawVault();



SocializingPool.sol#443
Severity: Low
443     error CallerNotWithdrawVault();



SocializingPool.sol#444
Severity: Low
444     error TransferFailed();



SocializingPool.sol#444
Severity: Low
444     error TransferFailed();



SocializingPool.sol#626
Severity: Low
626     error ETHTransferFailed(address recipient, uint256 amount);



SocializingPool.sol#626
Severity: Low
626     error ETHTransferFailed(address recipient, uint256 amount);



SocializingPool.sol#626
Severity: Low
626     error ETHTransferFailed(address recipient, uint256 amount);



SocializingPool.sol#627
Severity: Low
627     error SDTransferFailed();



SocializingPool.sol#627
Severity: Low
627     error SDTransferFailed();



SocializingPool.sol#628
Severity: Low
628     error RewardAlreadyHandled();



SocializingPool.sol#628
Severity: Low
628     error RewardAlreadyHandled();



SocializingPool.sol#629
Severity: Low
629     error RewardAlreadyClaimed(address operator, uint256 cycle);



SocializingPool.sol#629
Severity: Low
629     error RewardAlreadyClaimed(address operator, uint256 cycle);



SocializingPool.sol#629
Severity: Low
629     error RewardAlreadyClaimed(address operator, uint256 cycle);



SocializingPool.sol#630
Severity: Low
630     error InsufficientETHRewards();



SocializingPool.sol#630
Severity: Low
630     error InsufficientETHRewards();



SocializingPool.sol#631
Severity: Low
631     error InsufficientSDRewards();



SocializingPool.sol#631
Severity: Low
631     error InsufficientSDRewards();



SocializingPool.sol#632
Severity: Low
632     error InvalidAmount();



SocializingPool.sol#632
Severity: Low
632     error InvalidAmount();



SocializingPool.sol#633
Severity: Low
633     error InvalidProof(uint256 cycle, address operator);



SocializingPool.sol#633
Severity: Low
633     error InvalidProof(uint256 cycle, address operator);



SocializingPool.sol#633
Severity: Low
633     error InvalidProof(uint256 cycle, address operator);



SocializingPool.sol#634
Severity: Low
634     error InvalidCycleIndex();



SocializingPool.sol#634
Severity: Low
634     error InvalidCycleIndex();



SocializingPool.sol#635
Severity: Low
635     error FutureCycleIndex();



SocializingPool.sol#635
Severity: Low
635     error FutureCycleIndex();



SocializingPool.sol#658
Severity: Low
658         uint256[] calldata _amountSD,



SocializingPool.sol#659
Severity: Low
659         uint256[] calldata _amountETH,



SocializingPool.sol#659
Severity: Low
659         uint256[] calldata _amountETH,



SocializingPool.sol#660
Severity: Low
660         bytes32[][] calldata _merkleProof



SocializingPool.sol#701
Severity: Low
701     error InvalidDepositAmount();



SocializingPool.sol#701
Severity: Low
701     error InvalidDepositAmount();



SocializingPool.sol#702
Severity: Low
702     error UnsupportedOperation();



SocializingPool.sol#702
Severity: Low
702     error UnsupportedOperation();



SocializingPool.sol#703
Severity: Low
703     error InsufficientBalance();



SocializingPool.sol#703
Severity: Low
703     error InsufficientBalance();



SocializingPool.sol#704
Severity: Low
704     error TransferFailed();



SocializingPool.sol#704
Severity: Low
704     error TransferFailed();



SocializingPool.sol#705
Severity: Low
705     error PoolIdDoesNotExit();



SocializingPool.sol#705
Severity: Low
705     error PoolIdDoesNotExit();



SocializingPool.sol#706
Severity: Low
706     error CooldownNotComplete();



SocializingPool.sol#706
Severity: Low
706     error CooldownNotComplete();



SocializingPool.sol#707
Severity: Low
707     error UnsupportedOperationInSafeMode();



SocializingPool.sol#707
Severity: Low
707     error UnsupportedOperationInSafeMode();



SocializingPool.sol#757
Severity: Low
757     error TransferFailed();



SocializingPool.sol#757
Severity: Low
757     error TransferFailed();



SocializingPool.sol#758
Severity: Low
758     error InvalidBondEthValue();



SocializingPool.sol#758
Severity: Low
758     error InvalidBondEthValue();



SocializingPool.sol#759
Severity: Low
759     error InSufficientBalance();



SocializingPool.sol#759
Severity: Low
759     error InSufficientBalance();



SocializingPool.sol#760
Severity: Low
760     error CooldownNotComplete();



SocializingPool.sol#760
Severity: Low
760     error CooldownNotComplete();



SocializingPool.sol#761
Severity: Low
761     error NoChangeInState();



SocializingPool.sol#761
Severity: Low
761     error NoChangeInState();



SocializingPool.sol#796
Severity: Low
796         string calldata _operatorName,



SocializingPool.sol#797
Severity: Low
797         address payable _operatorRewardAddress



SocializingPool.sol#798
Severity: Low
798     ) external returns (address mevFeeRecipientAddress);



SocializingPool.sol#802
Severity: Low
802         bytes[] calldata _preDepositSignature,



SocializingPool.sol#803
Severity: Low
803         bytes[] calldata _depositSignature



SocializingPool.sol#977
Severity: Low
977     function sendValue(address payable recipient, uint256 amount) internal {



SocializingPool.sol#977
Severity: Low
977     function sendValue(address payable recipient, uint256 amount) internal {



SocializingPool.sol#978
Severity: Low
978         require(address(this).balance >= amount, "Address: insufficient balance");



SocializingPool.sol#978
Severity: Low
978         require(address(this).balance >= amount, "Address: insufficient balance");



SocializingPool.sol#978
Severity: Low
978         require(address(this).balance >= amount, "Address: insufficient balance");



SocializingPool.sol#978
Severity: Low
978         require(address(this).balance >= amount, "Address: insufficient balance");



SocializingPool.sol#980
Severity: Low
980         (bool success, ) = recipient.call{value: amount}("");



SocializingPool.sol#980
Severity: Low
980         (bool success, ) = recipient.call{value: amount}("");



SocializingPool.sol#980
Severity: Low
980         (bool success, ) = recipient.call{value: amount}("");



SocializingPool.sol#2333
Severity: Low
2333         bool[] calldata proofFlags,



SocializingPool.sol#2334
Severity: Low
2334         bytes32 root,



SocializingPool.sol#2335
Severity: Low
2335         bytes32[] memory leaves



SocializingPool.sol#2336
Severity: Low
2336     ) internal pure returns (bool) {



SocializingPool.sol#2337
Severity: Low
2337         return processMultiProofCalldata(proof, proofFlags, leaves) == root;



SocializingPool.sol#2337
Severity: Low
2337         return processMultiProofCalldata(proof, proofFlags, leaves) == root;



SocializingPool.sol#2337
Severity: Low
2337         return processMultiProofCalldata(proof, proofFlags, leaves) == root;



SocializingPool.sol#2568
Severity: Low
2568     receive() external payable {



SocializingPool.sol#2569
Severity: Low
2569         emit ETHReceived(msg.sender, msg.value);



SocializingPool.sol#2569
Severity: Low
2569         emit ETHReceived(msg.sender, msg.value);



SocializingPool.sol#2569
Severity: Low
2569         emit ETHReceived(msg.sender, msg.value);



```

### StaderConfig.sol

```

StaderConfig.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



StaderConfig.sol#393
Severity: Low
393     function onlyValidKeys(



StaderConfig.sol#750
Severity: Low
750     function sendValue(address payable recipient, uint256 amount) internal {



StaderConfig.sol#1892
Severity: Low
1892     constructor() {



StaderConfig.sol#6
Severity: Low
6     error InvalidLimits();



StaderConfig.sol#6
Severity: Low
6     error InvalidLimits();



StaderConfig.sol#7
Severity: Low
7     error InvalidMinDepositValue();



StaderConfig.sol#7
Severity: Low
7     error InvalidMinDepositValue();



StaderConfig.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



StaderConfig.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



StaderConfig.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



StaderConfig.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



StaderConfig.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



StaderConfig.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



StaderConfig.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



StaderConfig.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



StaderConfig.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



StaderConfig.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



StaderConfig.sol#198
Severity: Low
198     error maxKeyLimitReached();



StaderConfig.sol#198
Severity: Low
198     error maxKeyLimitReached();



StaderConfig.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



StaderConfig.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



StaderConfig.sol#200
Severity: Low
200     error InvalidKeyCount();



StaderConfig.sol#200
Severity: Low
200     error InvalidKeyCount();



StaderConfig.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



StaderConfig.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



StaderConfig.sol#202
Severity: Low
202     error OperatorIsDeactivate();



StaderConfig.sol#202
Severity: Low
202     error OperatorIsDeactivate();



StaderConfig.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



StaderConfig.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



StaderConfig.sol#204
Severity: Low
204     error PageNumberIsZero();



StaderConfig.sol#204
Severity: Low
204     error PageNumberIsZero();



StaderConfig.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



StaderConfig.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



StaderConfig.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



StaderConfig.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



StaderConfig.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



StaderConfig.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



StaderConfig.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



StaderConfig.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



StaderConfig.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



StaderConfig.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



StaderConfig.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



StaderConfig.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



StaderConfig.sol#240
Severity: Low
240             bytes calldata pubkey,



StaderConfig.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



StaderConfig.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



StaderConfig.sol#242
Severity: Low
242             bytes calldata depositSignature,



StaderConfig.sol#242
Severity: Low
242             bytes calldata depositSignature,



StaderConfig.sol#243
Severity: Low
243             address withdrawVaultAddress,



StaderConfig.sol#244
Severity: Low
244             uint256 operatorId,



StaderConfig.sol#245
Severity: Low
245             uint256 depositTime,



StaderConfig.sol#246
Severity: Low
246             uint256 withdrawnTime



StaderConfig.sol#256
Severity: Low
256             string calldata operatorName,



StaderConfig.sol#257
Severity: Low
257             address payable operatorRewardAddress,



StaderConfig.sol#258
Severity: Low
258             address operatorAddress



StaderConfig.sol#324
Severity: Low
324     error EmptyNameString();



StaderConfig.sol#324
Severity: Low
324     error EmptyNameString();



StaderConfig.sol#325
Severity: Low
325     error PoolIdNotPresent();



StaderConfig.sol#325
Severity: Low
325     error PoolIdNotPresent();



StaderConfig.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



StaderConfig.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



StaderConfig.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



StaderConfig.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



StaderConfig.sol#328
Severity: Low
328     error NameCrossedMaxLength();



StaderConfig.sol#328
Severity: Low
328     error NameCrossedMaxLength();



StaderConfig.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



StaderConfig.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



StaderConfig.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



StaderConfig.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



StaderConfig.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



StaderConfig.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



StaderConfig.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



StaderConfig.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



StaderConfig.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



StaderConfig.sol#396
Severity: Low
396         bytes calldata _depositSignature



StaderConfig.sol#410
Severity: Low
410     error CallerNotOwner();



StaderConfig.sol#410
Severity: Low
410     error CallerNotOwner();



StaderConfig.sol#411
Severity: Low
411     error AlreadyInitialized();



StaderConfig.sol#411
Severity: Low
411     error AlreadyInitialized();



StaderConfig.sol#437
Severity: Low
437     error ZeroAddress();



StaderConfig.sol#437
Severity: Low
437     error ZeroAddress();



StaderConfig.sol#438
Severity: Low
438     error InvalidPubkeyLength();



StaderConfig.sol#438
Severity: Low
438     error InvalidPubkeyLength();



StaderConfig.sol#439
Severity: Low
439     error CallerNotManager();



StaderConfig.sol#439
Severity: Low
439     error CallerNotManager();



StaderConfig.sol#440
Severity: Low
440     error CallerNotOperator();



StaderConfig.sol#440
Severity: Low
440     error CallerNotOperator();



StaderConfig.sol#441
Severity: Low
441     error CallerNotStaderContract();



StaderConfig.sol#441
Severity: Low
441     error CallerNotStaderContract();



StaderConfig.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



StaderConfig.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



StaderConfig.sol#443
Severity: Low
443     error TransferFailed();



StaderConfig.sol#443
Severity: Low
443     error TransferFailed();



StaderConfig.sol#750
Severity: Low
750     function sendValue(address payable recipient, uint256 amount) internal {



StaderConfig.sol#750
Severity: Low
750     function sendValue(address payable recipient, uint256 amount) internal {



StaderConfig.sol#751
Severity: Low
751         require(address(this).balance >= amount, "Address: insufficient balance");



StaderConfig.sol#751
Severity: Low
751         require(address(this).balance >= amount, "Address: insufficient balance");



StaderConfig.sol#751
Severity: Low
751         require(address(this).balance >= amount, "Address: insufficient balance");



StaderConfig.sol#751
Severity: Low
751         require(address(this).balance >= amount, "Address: insufficient balance");



StaderConfig.sol#753
Severity: Low
753         (bool success, ) = recipient.call{value: amount}("");



StaderConfig.sol#753
Severity: Low
753         (bool success, ) = recipient.call{value: amount}("");



StaderConfig.sol#753
Severity: Low
753         (bool success, ) = recipient.call{value: amount}("");



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



StaderInsuranceFund.sol#393
Severity: Low
393     function onlyValidKeys(



StaderInsuranceFund.sol#776
Severity: Low
776     function sendValue(address payable recipient, uint256 amount) internal {



StaderInsuranceFund.sol#1934
Severity: Low
1934     constructor() {



StaderInsuranceFund.sol#6
Severity: Low
6     error InvalidLimits();



StaderInsuranceFund.sol#6
Severity: Low
6     error InvalidLimits();



StaderInsuranceFund.sol#7
Severity: Low
7     error InvalidMinDepositValue();



StaderInsuranceFund.sol#7
Severity: Low
7     error InvalidMinDepositValue();



StaderInsuranceFund.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



StaderInsuranceFund.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



StaderInsuranceFund.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



StaderInsuranceFund.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



StaderInsuranceFund.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



StaderInsuranceFund.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



StaderInsuranceFund.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



StaderInsuranceFund.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



StaderInsuranceFund.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



StaderInsuranceFund.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



StaderInsuranceFund.sol#198
Severity: Low
198     error maxKeyLimitReached();



StaderInsuranceFund.sol#198
Severity: Low
198     error maxKeyLimitReached();



StaderInsuranceFund.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



StaderInsuranceFund.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



StaderInsuranceFund.sol#200
Severity: Low
200     error InvalidKeyCount();



StaderInsuranceFund.sol#200
Severity: Low
200     error InvalidKeyCount();



StaderInsuranceFund.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



StaderInsuranceFund.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



StaderInsuranceFund.sol#202
Severity: Low
202     error OperatorIsDeactivate();



StaderInsuranceFund.sol#202
Severity: Low
202     error OperatorIsDeactivate();



StaderInsuranceFund.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



StaderInsuranceFund.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



StaderInsuranceFund.sol#204
Severity: Low
204     error PageNumberIsZero();



StaderInsuranceFund.sol#204
Severity: Low
204     error PageNumberIsZero();



StaderInsuranceFund.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



StaderInsuranceFund.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



StaderInsuranceFund.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



StaderInsuranceFund.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



StaderInsuranceFund.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



StaderInsuranceFund.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



StaderInsuranceFund.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



StaderInsuranceFund.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



StaderInsuranceFund.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



StaderInsuranceFund.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



StaderInsuranceFund.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



StaderInsuranceFund.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



StaderInsuranceFund.sol#240
Severity: Low
240             bytes calldata pubkey,



StaderInsuranceFund.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



StaderInsuranceFund.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



StaderInsuranceFund.sol#242
Severity: Low
242             bytes calldata depositSignature,



StaderInsuranceFund.sol#242
Severity: Low
242             bytes calldata depositSignature,



StaderInsuranceFund.sol#243
Severity: Low
243             address withdrawVaultAddress,



StaderInsuranceFund.sol#244
Severity: Low
244             uint256 operatorId,



StaderInsuranceFund.sol#245
Severity: Low
245             uint256 depositTime,



StaderInsuranceFund.sol#246
Severity: Low
246             uint256 withdrawnTime



StaderInsuranceFund.sol#256
Severity: Low
256             string calldata operatorName,



StaderInsuranceFund.sol#257
Severity: Low
257             address payable operatorRewardAddress,



StaderInsuranceFund.sol#258
Severity: Low
258             address operatorAddress



StaderInsuranceFund.sol#324
Severity: Low
324     error EmptyNameString();



StaderInsuranceFund.sol#324
Severity: Low
324     error EmptyNameString();



StaderInsuranceFund.sol#325
Severity: Low
325     error PoolIdNotPresent();



StaderInsuranceFund.sol#325
Severity: Low
325     error PoolIdNotPresent();



StaderInsuranceFund.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



StaderInsuranceFund.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



StaderInsuranceFund.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



StaderInsuranceFund.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



StaderInsuranceFund.sol#328
Severity: Low
328     error NameCrossedMaxLength();



StaderInsuranceFund.sol#328
Severity: Low
328     error NameCrossedMaxLength();



StaderInsuranceFund.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



StaderInsuranceFund.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



StaderInsuranceFund.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



StaderInsuranceFund.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



StaderInsuranceFund.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



StaderInsuranceFund.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



StaderInsuranceFund.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



StaderInsuranceFund.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



StaderInsuranceFund.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



StaderInsuranceFund.sol#396
Severity: Low
396         bytes calldata _depositSignature



StaderInsuranceFund.sol#410
Severity: Low
410     error CallerNotOwner();



StaderInsuranceFund.sol#410
Severity: Low
410     error CallerNotOwner();



StaderInsuranceFund.sol#411
Severity: Low
411     error AlreadyInitialized();



StaderInsuranceFund.sol#411
Severity: Low
411     error AlreadyInitialized();



StaderInsuranceFund.sol#437
Severity: Low
437     error ZeroAddress();



StaderInsuranceFund.sol#437
Severity: Low
437     error ZeroAddress();



StaderInsuranceFund.sol#438
Severity: Low
438     error InvalidPubkeyLength();



StaderInsuranceFund.sol#438
Severity: Low
438     error InvalidPubkeyLength();



StaderInsuranceFund.sol#439
Severity: Low
439     error CallerNotManager();



StaderInsuranceFund.sol#439
Severity: Low
439     error CallerNotManager();



StaderInsuranceFund.sol#440
Severity: Low
440     error CallerNotOperator();



StaderInsuranceFund.sol#440
Severity: Low
440     error CallerNotOperator();



StaderInsuranceFund.sol#441
Severity: Low
441     error CallerNotStaderContract();



StaderInsuranceFund.sol#441
Severity: Low
441     error CallerNotStaderContract();



StaderInsuranceFund.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



StaderInsuranceFund.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



StaderInsuranceFund.sol#443
Severity: Low
443     error TransferFailed();



StaderInsuranceFund.sol#443
Severity: Low
443     error TransferFailed();



StaderInsuranceFund.sol#612
Severity: Low
612     error InvalidAmountProvided();



StaderInsuranceFund.sol#612
Severity: Low
612     error InvalidAmountProvided();



StaderInsuranceFund.sol#613
Severity: Low
613     error TransferFailed();



StaderInsuranceFund.sol#613
Severity: Low
613     error TransferFailed();



StaderInsuranceFund.sol#614
Severity: Low
614     error InSufficientBalance();



StaderInsuranceFund.sol#614
Severity: Low
614     error InSufficientBalance();



StaderInsuranceFund.sol#776
Severity: Low
776     function sendValue(address payable recipient, uint256 amount) internal {



StaderInsuranceFund.sol#776
Severity: Low
776     function sendValue(address payable recipient, uint256 amount) internal {



StaderInsuranceFund.sol#777
Severity: Low
777         require(address(this).balance >= amount, "Address: insufficient balance");



StaderInsuranceFund.sol#777
Severity: Low
777         require(address(this).balance >= amount, "Address: insufficient balance");



StaderInsuranceFund.sol#777
Severity: Low
777         require(address(this).balance >= amount, "Address: insufficient balance");



StaderInsuranceFund.sol#777
Severity: Low
777         require(address(this).balance >= amount, "Address: insufficient balance");



StaderInsuranceFund.sol#779
Severity: Low
779         (bool success, ) = recipient.call{value: amount}("");



StaderInsuranceFund.sol#779
Severity: Low
779         (bool success, ) = recipient.call{value: amount}("");



StaderInsuranceFund.sol#779
Severity: Low
779         (bool success, ) = recipient.call{value: amount}("");



```

### StaderOracle.sol

```

StaderOracle.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



StaderOracle.sol#393
Severity: Low
393     function onlyValidKeys(



StaderOracle.sol#655
Severity: Low
655     function claim(



StaderOracle.sol#1127
Severity: Low
1127     function sendValue(address payable recipient, uint256 amount) internal {



StaderOracle.sol#2515
Severity: Low
2515     constructor() {



StaderOracle.sol#6
Severity: Low
6     error InvalidLimits();



StaderOracle.sol#6
Severity: Low
6     error InvalidLimits();



StaderOracle.sol#7
Severity: Low
7     error InvalidMinDepositValue();



StaderOracle.sol#7
Severity: Low
7     error InvalidMinDepositValue();



StaderOracle.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



StaderOracle.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



StaderOracle.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



StaderOracle.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



StaderOracle.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



StaderOracle.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



StaderOracle.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



StaderOracle.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



StaderOracle.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



StaderOracle.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



StaderOracle.sol#198
Severity: Low
198     error maxKeyLimitReached();



StaderOracle.sol#198
Severity: Low
198     error maxKeyLimitReached();



StaderOracle.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



StaderOracle.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



StaderOracle.sol#200
Severity: Low
200     error InvalidKeyCount();



StaderOracle.sol#200
Severity: Low
200     error InvalidKeyCount();



StaderOracle.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



StaderOracle.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



StaderOracle.sol#202
Severity: Low
202     error OperatorIsDeactivate();



StaderOracle.sol#202
Severity: Low
202     error OperatorIsDeactivate();



StaderOracle.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



StaderOracle.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



StaderOracle.sol#204
Severity: Low
204     error PageNumberIsZero();



StaderOracle.sol#204
Severity: Low
204     error PageNumberIsZero();



StaderOracle.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



StaderOracle.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



StaderOracle.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



StaderOracle.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



StaderOracle.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



StaderOracle.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



StaderOracle.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



StaderOracle.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



StaderOracle.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



StaderOracle.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



StaderOracle.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



StaderOracle.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



StaderOracle.sol#240
Severity: Low
240             bytes calldata pubkey,



StaderOracle.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



StaderOracle.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



StaderOracle.sol#242
Severity: Low
242             bytes calldata depositSignature,



StaderOracle.sol#242
Severity: Low
242             bytes calldata depositSignature,



StaderOracle.sol#243
Severity: Low
243             address withdrawVaultAddress,



StaderOracle.sol#244
Severity: Low
244             uint256 operatorId,



StaderOracle.sol#245
Severity: Low
245             uint256 depositTime,



StaderOracle.sol#246
Severity: Low
246             uint256 withdrawnTime



StaderOracle.sol#256
Severity: Low
256             string calldata operatorName,



StaderOracle.sol#257
Severity: Low
257             address payable operatorRewardAddress,



StaderOracle.sol#258
Severity: Low
258             address operatorAddress



StaderOracle.sol#324
Severity: Low
324     error EmptyNameString();



StaderOracle.sol#324
Severity: Low
324     error EmptyNameString();



StaderOracle.sol#325
Severity: Low
325     error PoolIdNotPresent();



StaderOracle.sol#325
Severity: Low
325     error PoolIdNotPresent();



StaderOracle.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



StaderOracle.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



StaderOracle.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



StaderOracle.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



StaderOracle.sol#328
Severity: Low
328     error NameCrossedMaxLength();



StaderOracle.sol#328
Severity: Low
328     error NameCrossedMaxLength();



StaderOracle.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



StaderOracle.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



StaderOracle.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



StaderOracle.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



StaderOracle.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



StaderOracle.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



StaderOracle.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



StaderOracle.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



StaderOracle.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



StaderOracle.sol#396
Severity: Low
396         bytes calldata _depositSignature



StaderOracle.sol#410
Severity: Low
410     error CallerNotOwner();



StaderOracle.sol#410
Severity: Low
410     error CallerNotOwner();



StaderOracle.sol#411
Severity: Low
411     error AlreadyInitialized();



StaderOracle.sol#411
Severity: Low
411     error AlreadyInitialized();



StaderOracle.sol#437
Severity: Low
437     error ZeroAddress();



StaderOracle.sol#437
Severity: Low
437     error ZeroAddress();



StaderOracle.sol#438
Severity: Low
438     error InvalidPubkeyLength();



StaderOracle.sol#438
Severity: Low
438     error InvalidPubkeyLength();



StaderOracle.sol#439
Severity: Low
439     error CallerNotManager();



StaderOracle.sol#439
Severity: Low
439     error CallerNotManager();



StaderOracle.sol#440
Severity: Low
440     error CallerNotOperator();



StaderOracle.sol#440
Severity: Low
440     error CallerNotOperator();



StaderOracle.sol#441
Severity: Low
441     error CallerNotStaderContract();



StaderOracle.sol#441
Severity: Low
441     error CallerNotStaderContract();



StaderOracle.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



StaderOracle.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



StaderOracle.sol#443
Severity: Low
443     error TransferFailed();



StaderOracle.sol#443
Severity: Low
443     error TransferFailed();



StaderOracle.sol#625
Severity: Low
625     error ETHTransferFailed(address recipient, uint256 amount);



StaderOracle.sol#625
Severity: Low
625     error ETHTransferFailed(address recipient, uint256 amount);



StaderOracle.sol#625
Severity: Low
625     error ETHTransferFailed(address recipient, uint256 amount);



StaderOracle.sol#626
Severity: Low
626     error SDTransferFailed();



StaderOracle.sol#626
Severity: Low
626     error SDTransferFailed();



StaderOracle.sol#627
Severity: Low
627     error RewardAlreadyHandled();



StaderOracle.sol#627
Severity: Low
627     error RewardAlreadyHandled();



StaderOracle.sol#628
Severity: Low
628     error RewardAlreadyClaimed(address operator, uint256 cycle);



StaderOracle.sol#628
Severity: Low
628     error RewardAlreadyClaimed(address operator, uint256 cycle);



StaderOracle.sol#628
Severity: Low
628     error RewardAlreadyClaimed(address operator, uint256 cycle);



StaderOracle.sol#629
Severity: Low
629     error InsufficientETHRewards();



StaderOracle.sol#629
Severity: Low
629     error InsufficientETHRewards();



StaderOracle.sol#630
Severity: Low
630     error InsufficientSDRewards();



StaderOracle.sol#630
Severity: Low
630     error InsufficientSDRewards();



StaderOracle.sol#631
Severity: Low
631     error InvalidAmount();



StaderOracle.sol#631
Severity: Low
631     error InvalidAmount();



StaderOracle.sol#632
Severity: Low
632     error InvalidProof(uint256 cycle, address operator);



StaderOracle.sol#632
Severity: Low
632     error InvalidProof(uint256 cycle, address operator);



StaderOracle.sol#632
Severity: Low
632     error InvalidProof(uint256 cycle, address operator);



StaderOracle.sol#633
Severity: Low
633     error InvalidCycleIndex();



StaderOracle.sol#633
Severity: Low
633     error InvalidCycleIndex();



StaderOracle.sol#634
Severity: Low
634     error FutureCycleIndex();



StaderOracle.sol#634
Severity: Low
634     error FutureCycleIndex();



StaderOracle.sol#657
Severity: Low
657         uint256[] calldata _amountSD,



StaderOracle.sol#658
Severity: Low
658         uint256[] calldata _amountETH,



StaderOracle.sol#658
Severity: Low
658         uint256[] calldata _amountETH,



StaderOracle.sol#659
Severity: Low
659         bytes32[][] calldata _merkleProof



StaderOracle.sol#757
Severity: Low
757     error InvalidUpdate();



StaderOracle.sol#757
Severity: Low
757     error InvalidUpdate();



StaderOracle.sol#758
Severity: Low
758     error NodeAlreadyTrusted();



StaderOracle.sol#758
Severity: Low
758     error NodeAlreadyTrusted();



StaderOracle.sol#759
Severity: Low
759     error NodeNotTrusted();



StaderOracle.sol#759
Severity: Low
759     error NodeNotTrusted();



StaderOracle.sol#760
Severity: Low
760     error ZeroFrequency();



StaderOracle.sol#760
Severity: Low
760     error ZeroFrequency();



StaderOracle.sol#761
Severity: Low
761     error FrequencyUnchanged();



StaderOracle.sol#761
Severity: Low
761     error FrequencyUnchanged();



StaderOracle.sol#762
Severity: Low
762     error DuplicateSubmissionFromNode();



StaderOracle.sol#762
Severity: Low
762     error DuplicateSubmissionFromNode();



StaderOracle.sol#763
Severity: Low
763     error ReportingFutureBlockData();



StaderOracle.sol#763
Severity: Low
763     error ReportingFutureBlockData();



StaderOracle.sol#764
Severity: Low
764     error InvalidMerkleRootIndex();



StaderOracle.sol#764
Severity: Low
764     error InvalidMerkleRootIndex();



StaderOracle.sol#765
Severity: Low
765     error ReportingPreviousCycleData();



StaderOracle.sol#765
Severity: Low
765     error ReportingPreviousCycleData();



StaderOracle.sol#766
Severity: Low
766     error InvalidMAPDIndex();



StaderOracle.sol#766
Severity: Low
766     error InvalidMAPDIndex();



StaderOracle.sol#767
Severity: Low
767     error PageNumberAlreadyReported();



StaderOracle.sol#767
Severity: Low
767     error PageNumberAlreadyReported();



StaderOracle.sol#768
Severity: Low
768     error NotATrustedNode();



StaderOracle.sol#768
Severity: Low
768     error NotATrustedNode();



StaderOracle.sol#769
Severity: Low
769     error InvalidERDataSource();



StaderOracle.sol#769
Severity: Low
769     error InvalidERDataSource();



StaderOracle.sol#770
Severity: Low
770     error InspectionModeActive();



StaderOracle.sol#770
Severity: Low
770     error InspectionModeActive();



StaderOracle.sol#771
Severity: Low
771     error UpdateFrequencyNotSet();



StaderOracle.sol#771
Severity: Low
771     error UpdateFrequencyNotSet();



StaderOracle.sol#772
Severity: Low
772     error InvalidReportingBlock();



StaderOracle.sol#772
Severity: Low
772     error InvalidReportingBlock();



StaderOracle.sol#773
Severity: Low
773     error ERChangeLimitCrossed();



StaderOracle.sol#773
Severity: Low
773     error ERChangeLimitCrossed();



StaderOracle.sol#774
Severity: Low
774     error ERChangeLimitNotCrossed();



StaderOracle.sol#774
Severity: Low
774     error ERChangeLimitNotCrossed();



StaderOracle.sol#775
Severity: Low
775     error ERPermissibleChangeOutofBounds();



StaderOracle.sol#775
Severity: Low
775     error ERPermissibleChangeOutofBounds();



StaderOracle.sol#776
Severity: Low
776     error InsufficientTrustedNodes();



StaderOracle.sol#776
Severity: Low
776     error InsufficientTrustedNodes();



StaderOracle.sol#777
Severity: Low
777     error CooldownNotComplete();



StaderOracle.sol#777
Severity: Low
777     error CooldownNotComplete();



StaderOracle.sol#981
Severity: Low
981     error InvalidDepositAmount();



StaderOracle.sol#981
Severity: Low
981     error InvalidDepositAmount();



StaderOracle.sol#982
Severity: Low
982     error UnsupportedOperation();



StaderOracle.sol#982
Severity: Low
982     error UnsupportedOperation();



StaderOracle.sol#983
Severity: Low
983     error InsufficientBalance();



StaderOracle.sol#983
Severity: Low
983     error InsufficientBalance();



StaderOracle.sol#984
Severity: Low
984     error TransferFailed();



StaderOracle.sol#984
Severity: Low
984     error TransferFailed();



StaderOracle.sol#985
Severity: Low
985     error PoolIdDoesNotExit();



StaderOracle.sol#985
Severity: Low
985     error PoolIdDoesNotExit();



StaderOracle.sol#986
Severity: Low
986     error CooldownNotComplete();



StaderOracle.sol#986
Severity: Low
986     error CooldownNotComplete();



StaderOracle.sol#987
Severity: Low
987     error UnsupportedOperationInSafeMode();



StaderOracle.sol#987
Severity: Low
987     error UnsupportedOperationInSafeMode();



StaderOracle.sol#1127
Severity: Low
1127     function sendValue(address payable recipient, uint256 amount) internal {



StaderOracle.sol#1127
Severity: Low
1127     function sendValue(address payable recipient, uint256 amount) internal {



StaderOracle.sol#1128
Severity: Low
1128         require(address(this).balance >= amount, "Address: insufficient balance");



StaderOracle.sol#1128
Severity: Low
1128         require(address(this).balance >= amount, "Address: insufficient balance");



StaderOracle.sol#1128
Severity: Low
1128         require(address(this).balance >= amount, "Address: insufficient balance");



StaderOracle.sol#1128
Severity: Low
1128         require(address(this).balance >= amount, "Address: insufficient balance");



StaderOracle.sol#1130
Severity: Low
1130         (bool success, ) = recipient.call{value: amount}("");



StaderOracle.sol#1130
Severity: Low
1130         (bool success, ) = recipient.call{value: amount}("");



StaderOracle.sol#1130
Severity: Low
1130         (bool success, ) = recipient.call{value: amount}("");



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#229
Severity: Low
229     function markValidatorReadyToDeposit(



StaderStakePoolsManager.sol#394
Severity: Low
394     function onlyValidKeys(



StaderStakePoolsManager.sol#769
Severity: Low
769     function sendValue(address payable recipient, uint256 amount) internal {



StaderStakePoolsManager.sol#2446
Severity: Low
2446     constructor() {



StaderStakePoolsManager.sol#2588
Severity: Low
2588     function claim(



StaderStakePoolsManager.sol#3632
Severity: Low
3632     constructor() {



StaderStakePoolsManager.sol#7
Severity: Low
7     error InvalidLimits();



StaderStakePoolsManager.sol#7
Severity: Low
7     error InvalidLimits();



StaderStakePoolsManager.sol#8
Severity: Low
8     error InvalidMinDepositValue();



StaderStakePoolsManager.sol#8
Severity: Low
8     error InvalidMinDepositValue();



StaderStakePoolsManager.sol#9
Severity: Low
9     error InvalidMaxDepositValue();



StaderStakePoolsManager.sol#9
Severity: Low
9     error InvalidMaxDepositValue();



StaderStakePoolsManager.sol#10
Severity: Low
10     error InvalidMinWithdrawValue();



StaderStakePoolsManager.sol#10
Severity: Low
10     error InvalidMinWithdrawValue();



StaderStakePoolsManager.sol#11
Severity: Low
11     error InvalidMaxWithdrawValue();



StaderStakePoolsManager.sol#11
Severity: Low
11     error InvalidMaxWithdrawValue();



StaderStakePoolsManager.sol#197
Severity: Low
197     error DuplicatePoolIDOrPoolNotAdded();



StaderStakePoolsManager.sol#197
Severity: Low
197     error DuplicatePoolIDOrPoolNotAdded();



StaderStakePoolsManager.sol#198
Severity: Low
198     error OperatorAlreadyOnBoardedInProtocol();



StaderStakePoolsManager.sol#198
Severity: Low
198     error OperatorAlreadyOnBoardedInProtocol();



StaderStakePoolsManager.sol#199
Severity: Low
199     error maxKeyLimitReached();



StaderStakePoolsManager.sol#199
Severity: Low
199     error maxKeyLimitReached();



StaderStakePoolsManager.sol#200
Severity: Low
200     error OperatorNotOnBoarded();



StaderStakePoolsManager.sol#200
Severity: Low
200     error OperatorNotOnBoarded();



StaderStakePoolsManager.sol#201
Severity: Low
201     error InvalidKeyCount();



StaderStakePoolsManager.sol#201
Severity: Low
201     error InvalidKeyCount();



StaderStakePoolsManager.sol#202
Severity: Low
202     error InvalidStartAndEndIndex();



StaderStakePoolsManager.sol#202
Severity: Low
202     error InvalidStartAndEndIndex();



StaderStakePoolsManager.sol#203
Severity: Low
203     error OperatorIsDeactivate();



StaderStakePoolsManager.sol#203
Severity: Low
203     error OperatorIsDeactivate();



StaderStakePoolsManager.sol#204
Severity: Low
204     error MisMatchingInputKeysSize();



StaderStakePoolsManager.sol#204
Severity: Low
204     error MisMatchingInputKeysSize();



StaderStakePoolsManager.sol#205
Severity: Low
205     error PageNumberIsZero();



StaderStakePoolsManager.sol#205
Severity: Low
205     error PageNumberIsZero();



StaderStakePoolsManager.sol#206
Severity: Low
206     error UNEXPECTED_STATUS();



StaderStakePoolsManager.sol#206
Severity: Low
206     error UNEXPECTED_STATUS();



StaderStakePoolsManager.sol#207
Severity: Low
207     error PubkeyAlreadyExist();



StaderStakePoolsManager.sol#207
Severity: Low
207     error PubkeyAlreadyExist();



StaderStakePoolsManager.sol#208
Severity: Low
208     error NotEnoughSDCollateral();



StaderStakePoolsManager.sol#208
Severity: Low
208     error NotEnoughSDCollateral();



StaderStakePoolsManager.sol#209
Severity: Low
209     error TooManyVerifiedKeysReported();



StaderStakePoolsManager.sol#209
Severity: Low
209     error TooManyVerifiedKeysReported();



StaderStakePoolsManager.sol#210
Severity: Low
210     error TooManyWithdrawnKeysReported();



StaderStakePoolsManager.sol#210
Severity: Low
210     error TooManyWithdrawnKeysReported();



StaderStakePoolsManager.sol#231
Severity: Low
231         bytes[] calldata _frontRunPubkey,



StaderStakePoolsManager.sol#232
Severity: Low
232         bytes[] calldata _invalidSignaturePubkey



StaderStakePoolsManager.sol#241
Severity: Low
241             bytes calldata pubkey,



StaderStakePoolsManager.sol#242
Severity: Low
242             bytes calldata preDepositSignature,



StaderStakePoolsManager.sol#242
Severity: Low
242             bytes calldata preDepositSignature,



StaderStakePoolsManager.sol#243
Severity: Low
243             bytes calldata depositSignature,



StaderStakePoolsManager.sol#243
Severity: Low
243             bytes calldata depositSignature,



StaderStakePoolsManager.sol#244
Severity: Low
244             address withdrawVaultAddress,



StaderStakePoolsManager.sol#245
Severity: Low
245             uint256 operatorId,



StaderStakePoolsManager.sol#246
Severity: Low
246             uint256 depositTime,



StaderStakePoolsManager.sol#247
Severity: Low
247             uint256 withdrawnTime



StaderStakePoolsManager.sol#257
Severity: Low
257             string calldata operatorName,



StaderStakePoolsManager.sol#258
Severity: Low
258             address payable operatorRewardAddress,



StaderStakePoolsManager.sol#259
Severity: Low
259             address operatorAddress



StaderStakePoolsManager.sol#325
Severity: Low
325     error EmptyNameString();



StaderStakePoolsManager.sol#325
Severity: Low
325     error EmptyNameString();



StaderStakePoolsManager.sol#326
Severity: Low
326     error PoolIdNotPresent();



StaderStakePoolsManager.sol#326
Severity: Low
326     error PoolIdNotPresent();



StaderStakePoolsManager.sol#327
Severity: Low
327     error PubkeyDoesNotExit();



StaderStakePoolsManager.sol#327
Severity: Low
327     error PubkeyDoesNotExit();



StaderStakePoolsManager.sol#328
Severity: Low
328     error PubkeyAlreadyExist();



StaderStakePoolsManager.sol#328
Severity: Low
328     error PubkeyAlreadyExist();



StaderStakePoolsManager.sol#329
Severity: Low
329     error NameCrossedMaxLength();



StaderStakePoolsManager.sol#329
Severity: Low
329     error NameCrossedMaxLength();



StaderStakePoolsManager.sol#330
Severity: Low
330     error InvalidLengthOfPubkey();



StaderStakePoolsManager.sol#330
Severity: Low
330     error InvalidLengthOfPubkey();



StaderStakePoolsManager.sol#331
Severity: Low
331     error OperatorIsNotOnboarded();



StaderStakePoolsManager.sol#331
Severity: Low
331     error OperatorIsNotOnboarded();



StaderStakePoolsManager.sol#332
Severity: Low
332     error InvalidLengthOfSignature();



StaderStakePoolsManager.sol#332
Severity: Low
332     error InvalidLengthOfSignature();



StaderStakePoolsManager.sol#333
Severity: Low
333     error ExistingOrMismatchingPoolId();



StaderStakePoolsManager.sol#333
Severity: Low
333     error ExistingOrMismatchingPoolId();



StaderStakePoolsManager.sol#396
Severity: Low
396         bytes calldata _preDepositSignature,



StaderStakePoolsManager.sol#397
Severity: Low
397         bytes calldata _depositSignature



StaderStakePoolsManager.sol#411
Severity: Low
411     error CallerNotOwner();



StaderStakePoolsManager.sol#411
Severity: Low
411     error CallerNotOwner();



StaderStakePoolsManager.sol#412
Severity: Low
412     error AlreadyInitialized();



StaderStakePoolsManager.sol#412
Severity: Low
412     error AlreadyInitialized();



StaderStakePoolsManager.sol#438
Severity: Low
438     error ZeroAddress();



StaderStakePoolsManager.sol#438
Severity: Low
438     error ZeroAddress();



StaderStakePoolsManager.sol#439
Severity: Low
439     error InvalidPubkeyLength();



StaderStakePoolsManager.sol#439
Severity: Low
439     error InvalidPubkeyLength();



StaderStakePoolsManager.sol#440
Severity: Low
440     error CallerNotManager();



StaderStakePoolsManager.sol#440
Severity: Low
440     error CallerNotManager();



StaderStakePoolsManager.sol#441
Severity: Low
441     error CallerNotOperator();



StaderStakePoolsManager.sol#441
Severity: Low
441     error CallerNotOperator();



StaderStakePoolsManager.sol#442
Severity: Low
442     error CallerNotStaderContract();



StaderStakePoolsManager.sol#442
Severity: Low
442     error CallerNotStaderContract();



StaderStakePoolsManager.sol#443
Severity: Low
443     error CallerNotWithdrawVault();



StaderStakePoolsManager.sol#443
Severity: Low
443     error CallerNotWithdrawVault();



StaderStakePoolsManager.sol#444
Severity: Low
444     error TransferFailed();



StaderStakePoolsManager.sol#444
Severity: Low
444     error TransferFailed();



StaderStakePoolsManager.sol#769
Severity: Low
769     function sendValue(address payable recipient, uint256 amount) internal {



StaderStakePoolsManager.sol#769
Severity: Low
769     function sendValue(address payable recipient, uint256 amount) internal {



StaderStakePoolsManager.sol#770
Severity: Low
770         require(address(this).balance >= amount, "Address: insufficient balance");



StaderStakePoolsManager.sol#770
Severity: Low
770         require(address(this).balance >= amount, "Address: insufficient balance");



StaderStakePoolsManager.sol#770
Severity: Low
770         require(address(this).balance >= amount, "Address: insufficient balance");



StaderStakePoolsManager.sol#770
Severity: Low
770         require(address(this).balance >= amount, "Address: insufficient balance");



StaderStakePoolsManager.sol#772
Severity: Low
772         (bool success, ) = recipient.call{value: amount}("");



StaderStakePoolsManager.sol#772
Severity: Low
772         (bool success, ) = recipient.call{value: amount}("");



StaderStakePoolsManager.sol#772
Severity: Low
772         (bool success, ) = recipient.call{value: amount}("");



StaderStakePoolsManager.sol#2515
Severity: Low
2515     error InvalidTargetWeight();



StaderStakePoolsManager.sol#2515
Severity: Low
2515     error InvalidTargetWeight();



StaderStakePoolsManager.sol#2516
Severity: Low
2516     error InvalidNewTargetInput();



StaderStakePoolsManager.sol#2516
Severity: Low
2516     error InvalidNewTargetInput();



StaderStakePoolsManager.sol#2517
Severity: Low
2517     error InvalidSumOfPoolWeights();



StaderStakePoolsManager.sol#2517
Severity: Low
2517     error InvalidSumOfPoolWeights();



StaderStakePoolsManager.sol#2558
Severity: Low
2558     error ETHTransferFailed(address recipient, uint256 amount);



StaderStakePoolsManager.sol#2558
Severity: Low
2558     error ETHTransferFailed(address recipient, uint256 amount);



StaderStakePoolsManager.sol#2558
Severity: Low
2558     error ETHTransferFailed(address recipient, uint256 amount);



StaderStakePoolsManager.sol#2559
Severity: Low
2559     error SDTransferFailed();



StaderStakePoolsManager.sol#2559
Severity: Low
2559     error SDTransferFailed();



StaderStakePoolsManager.sol#2560
Severity: Low
2560     error RewardAlreadyHandled();



StaderStakePoolsManager.sol#2560
Severity: Low
2560     error RewardAlreadyHandled();



StaderStakePoolsManager.sol#2561
Severity: Low
2561     error RewardAlreadyClaimed(address operator, uint256 cycle);



StaderStakePoolsManager.sol#2561
Severity: Low
2561     error RewardAlreadyClaimed(address operator, uint256 cycle);



StaderStakePoolsManager.sol#2561
Severity: Low
2561     error RewardAlreadyClaimed(address operator, uint256 cycle);



StaderStakePoolsManager.sol#2562
Severity: Low
2562     error InsufficientETHRewards();



StaderStakePoolsManager.sol#2562
Severity: Low
2562     error InsufficientETHRewards();



StaderStakePoolsManager.sol#2563
Severity: Low
2563     error InsufficientSDRewards();



StaderStakePoolsManager.sol#2563
Severity: Low
2563     error InsufficientSDRewards();



StaderStakePoolsManager.sol#2564
Severity: Low
2564     error InvalidAmount();



StaderStakePoolsManager.sol#2564
Severity: Low
2564     error InvalidAmount();



StaderStakePoolsManager.sol#2565
Severity: Low
2565     error InvalidProof(uint256 cycle, address operator);



StaderStakePoolsManager.sol#2565
Severity: Low
2565     error InvalidProof(uint256 cycle, address operator);



StaderStakePoolsManager.sol#2565
Severity: Low
2565     error InvalidProof(uint256 cycle, address operator);



StaderStakePoolsManager.sol#2566
Severity: Low
2566     error InvalidCycleIndex();



StaderStakePoolsManager.sol#2566
Severity: Low
2566     error InvalidCycleIndex();



StaderStakePoolsManager.sol#2567
Severity: Low
2567     error FutureCycleIndex();



StaderStakePoolsManager.sol#2567
Severity: Low
2567     error FutureCycleIndex();



StaderStakePoolsManager.sol#2590
Severity: Low
2590         uint256[] calldata _amountSD,



StaderStakePoolsManager.sol#2591
Severity: Low
2591         uint256[] calldata _amountETH,



StaderStakePoolsManager.sol#2591
Severity: Low
2591         uint256[] calldata _amountETH,



StaderStakePoolsManager.sol#2592
Severity: Low
2592         bytes32[][] calldata _merkleProof



StaderStakePoolsManager.sol#2690
Severity: Low
2690     error InvalidUpdate();



StaderStakePoolsManager.sol#2690
Severity: Low
2690     error InvalidUpdate();



StaderStakePoolsManager.sol#2691
Severity: Low
2691     error NodeAlreadyTrusted();



StaderStakePoolsManager.sol#2691
Severity: Low
2691     error NodeAlreadyTrusted();



StaderStakePoolsManager.sol#2692
Severity: Low
2692     error NodeNotTrusted();



StaderStakePoolsManager.sol#2692
Severity: Low
2692     error NodeNotTrusted();



StaderStakePoolsManager.sol#2693
Severity: Low
2693     error ZeroFrequency();



StaderStakePoolsManager.sol#2693
Severity: Low
2693     error ZeroFrequency();



StaderStakePoolsManager.sol#2694
Severity: Low
2694     error FrequencyUnchanged();



StaderStakePoolsManager.sol#2694
Severity: Low
2694     error FrequencyUnchanged();



StaderStakePoolsManager.sol#2695
Severity: Low
2695     error DuplicateSubmissionFromNode();



StaderStakePoolsManager.sol#2695
Severity: Low
2695     error DuplicateSubmissionFromNode();



StaderStakePoolsManager.sol#2696
Severity: Low
2696     error ReportingFutureBlockData();



StaderStakePoolsManager.sol#2696
Severity: Low
2696     error ReportingFutureBlockData();



StaderStakePoolsManager.sol#2697
Severity: Low
2697     error InvalidMerkleRootIndex();



StaderStakePoolsManager.sol#2697
Severity: Low
2697     error InvalidMerkleRootIndex();



StaderStakePoolsManager.sol#2698
Severity: Low
2698     error ReportingPreviousCycleData();



StaderStakePoolsManager.sol#2698
Severity: Low
2698     error ReportingPreviousCycleData();



StaderStakePoolsManager.sol#2699
Severity: Low
2699     error InvalidMAPDIndex();



StaderStakePoolsManager.sol#2699
Severity: Low
2699     error InvalidMAPDIndex();



StaderStakePoolsManager.sol#2700
Severity: Low
2700     error PageNumberAlreadyReported();



StaderStakePoolsManager.sol#2700
Severity: Low
2700     error PageNumberAlreadyReported();



StaderStakePoolsManager.sol#2701
Severity: Low
2701     error NotATrustedNode();



StaderStakePoolsManager.sol#2701
Severity: Low
2701     error NotATrustedNode();



StaderStakePoolsManager.sol#2702
Severity: Low
2702     error InvalidERDataSource();



StaderStakePoolsManager.sol#2702
Severity: Low
2702     error InvalidERDataSource();



StaderStakePoolsManager.sol#2703
Severity: Low
2703     error InspectionModeActive();



StaderStakePoolsManager.sol#2703
Severity: Low
2703     error InspectionModeActive();



StaderStakePoolsManager.sol#2704
Severity: Low
2704     error UpdateFrequencyNotSet();



StaderStakePoolsManager.sol#2704
Severity: Low
2704     error UpdateFrequencyNotSet();



StaderStakePoolsManager.sol#2705
Severity: Low
2705     error InvalidReportingBlock();



StaderStakePoolsManager.sol#2705
Severity: Low
2705     error InvalidReportingBlock();



StaderStakePoolsManager.sol#2706
Severity: Low
2706     error ERChangeLimitCrossed();



StaderStakePoolsManager.sol#2706
Severity: Low
2706     error ERChangeLimitCrossed();



StaderStakePoolsManager.sol#2707
Severity: Low
2707     error ERChangeLimitNotCrossed();



StaderStakePoolsManager.sol#2707
Severity: Low
2707     error ERChangeLimitNotCrossed();



StaderStakePoolsManager.sol#2708
Severity: Low
2708     error ERPermissibleChangeOutofBounds();



StaderStakePoolsManager.sol#2708
Severity: Low
2708     error ERPermissibleChangeOutofBounds();



StaderStakePoolsManager.sol#2709
Severity: Low
2709     error InsufficientTrustedNodes();



StaderStakePoolsManager.sol#2709
Severity: Low
2709     error InsufficientTrustedNodes();



StaderStakePoolsManager.sol#2710
Severity: Low
2710     error CooldownNotComplete();



StaderStakePoolsManager.sol#2710
Severity: Low
2710     error CooldownNotComplete();



StaderStakePoolsManager.sol#2914
Severity: Low
2914     error UnsupportedOperation();



StaderStakePoolsManager.sol#2914
Severity: Low
2914     error UnsupportedOperation();



StaderStakePoolsManager.sol#2915
Severity: Low
2915     error InvalidCommission();



StaderStakePoolsManager.sol#2915
Severity: Low
2915     error InvalidCommission();



StaderStakePoolsManager.sol#2916
Severity: Low
2916     error CouldNotDetermineExcessETH();



StaderStakePoolsManager.sol#2916
Severity: Low
2916     error CouldNotDetermineExcessETH();



StaderStakePoolsManager.sol#2962
Severity: Low
2962     error ETHTransferFailed();



StaderStakePoolsManager.sol#2962
Severity: Low
2962     error ETHTransferFailed();



StaderStakePoolsManager.sol#2963
Severity: Low
2963     error UnsupportedOperationInSafeMode();



StaderStakePoolsManager.sol#2963
Severity: Low
2963     error UnsupportedOperationInSafeMode();



StaderStakePoolsManager.sol#2964
Severity: Low
2964     error InSufficientBalance();



StaderStakePoolsManager.sol#2964
Severity: Low
2964     error InSufficientBalance();



StaderStakePoolsManager.sol#2965
Severity: Low
2965     error ProtocolNotHealthy();



StaderStakePoolsManager.sol#2965
Severity: Low
2965     error ProtocolNotHealthy();



StaderStakePoolsManager.sol#2966
Severity: Low
2966     error InvalidWithdrawAmount();



StaderStakePoolsManager.sol#2966
Severity: Low
2966     error InvalidWithdrawAmount();



StaderStakePoolsManager.sol#2967
Severity: Low
2967     error requestIdNotFinalized(uint256 _requestId);



StaderStakePoolsManager.sol#2967
Severity: Low
2967     error requestIdNotFinalized(uint256 _requestId);



StaderStakePoolsManager.sol#2968
Severity: Low
2968     error RequestAlreadyRedeemed(uint256 _requestId);



StaderStakePoolsManager.sol#2968
Severity: Low
2968     error RequestAlreadyRedeemed(uint256 _requestId);



StaderStakePoolsManager.sol#2969
Severity: Low
2969     error MaxLimitOnWithdrawRequestCountReached();



StaderStakePoolsManager.sol#2969
Severity: Low
2969     error MaxLimitOnWithdrawRequestCountReached();



StaderStakePoolsManager.sol#2970
Severity: Low
2970     error CannotFindRequestId();



StaderStakePoolsManager.sol#2970
Severity: Low
2970     error CannotFindRequestId();



StaderStakePoolsManager.sol#2971
Severity: Low
2971     error CallerNotAuthorizedToRedeem();



StaderStakePoolsManager.sol#2971
Severity: Low
2971     error CallerNotAuthorizedToRedeem();



StaderStakePoolsManager.sol#2972
Severity: Low
2972     error ZeroAddressReceived();



StaderStakePoolsManager.sol#2972
Severity: Low
2972     error ZeroAddressReceived();



StaderStakePoolsManager.sol#3009
Severity: Low
3009             address payable owner,



StaderStakePoolsManager.sol#3010
Severity: Low
3010             uint256 ethXAmount,



StaderStakePoolsManager.sol#3011
Severity: Low
3011             uint256 ethExpected,



StaderStakePoolsManager.sol#3012
Severity: Low
3012             uint256 ethFinalized,



StaderStakePoolsManager.sol#3013
Severity: Low
3013             uint256 requestTime



StaderStakePoolsManager.sol#3031
Severity: Low
3031     error InvalidDepositAmount();



StaderStakePoolsManager.sol#3031
Severity: Low
3031     error InvalidDepositAmount();



StaderStakePoolsManager.sol#3032
Severity: Low
3032     error UnsupportedOperation();



StaderStakePoolsManager.sol#3032
Severity: Low
3032     error UnsupportedOperation();



StaderStakePoolsManager.sol#3033
Severity: Low
3033     error InsufficientBalance();



StaderStakePoolsManager.sol#3033
Severity: Low
3033     error InsufficientBalance();



StaderStakePoolsManager.sol#3034
Severity: Low
3034     error TransferFailed();



StaderStakePoolsManager.sol#3034
Severity: Low
3034     error TransferFailed();



StaderStakePoolsManager.sol#3035
Severity: Low
3035     error PoolIdDoesNotExit();



StaderStakePoolsManager.sol#3035
Severity: Low
3035     error PoolIdDoesNotExit();



StaderStakePoolsManager.sol#3036
Severity: Low
3036     error CooldownNotComplete();



StaderStakePoolsManager.sol#3036
Severity: Low
3036     error CooldownNotComplete();



StaderStakePoolsManager.sol#3037
Severity: Low
3037     error UnsupportedOperationInSafeMode();



StaderStakePoolsManager.sol#3037
Severity: Low
3037     error UnsupportedOperationInSafeMode();



StaderStakePoolsManager.sol#3653
Severity: Low
3653     fallback() external payable {



StaderStakePoolsManager.sol#3654
Severity: Low
3654         revert UnsupportedOperation();



StaderStakePoolsManager.sol#3654
Severity: Low
3654         revert UnsupportedOperation();



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



UserWithdrawalManager.sol#393
Severity: Low
393     function onlyValidKeys(



UserWithdrawalManager.sol#768
Severity: Low
768     function sendValue(address payable recipient, uint256 amount) internal {



UserWithdrawalManager.sol#2445
Severity: Low
2445     constructor() {



UserWithdrawalManager.sol#2565
Severity: Low
2565     function claim(



UserWithdrawalManager.sol#3516
Severity: Low
3516     constructor() {



UserWithdrawalManager.sol#6
Severity: Low
6     error InvalidLimits();



UserWithdrawalManager.sol#6
Severity: Low
6     error InvalidLimits();



UserWithdrawalManager.sol#7
Severity: Low
7     error InvalidMinDepositValue();



UserWithdrawalManager.sol#7
Severity: Low
7     error InvalidMinDepositValue();



UserWithdrawalManager.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



UserWithdrawalManager.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



UserWithdrawalManager.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



UserWithdrawalManager.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



UserWithdrawalManager.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



UserWithdrawalManager.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



UserWithdrawalManager.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



UserWithdrawalManager.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



UserWithdrawalManager.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



UserWithdrawalManager.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



UserWithdrawalManager.sol#198
Severity: Low
198     error maxKeyLimitReached();



UserWithdrawalManager.sol#198
Severity: Low
198     error maxKeyLimitReached();



UserWithdrawalManager.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



UserWithdrawalManager.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



UserWithdrawalManager.sol#200
Severity: Low
200     error InvalidKeyCount();



UserWithdrawalManager.sol#200
Severity: Low
200     error InvalidKeyCount();



UserWithdrawalManager.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



UserWithdrawalManager.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



UserWithdrawalManager.sol#202
Severity: Low
202     error OperatorIsDeactivate();



UserWithdrawalManager.sol#202
Severity: Low
202     error OperatorIsDeactivate();



UserWithdrawalManager.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



UserWithdrawalManager.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



UserWithdrawalManager.sol#204
Severity: Low
204     error PageNumberIsZero();



UserWithdrawalManager.sol#204
Severity: Low
204     error PageNumberIsZero();



UserWithdrawalManager.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



UserWithdrawalManager.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



UserWithdrawalManager.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



UserWithdrawalManager.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



UserWithdrawalManager.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



UserWithdrawalManager.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



UserWithdrawalManager.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



UserWithdrawalManager.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



UserWithdrawalManager.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



UserWithdrawalManager.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



UserWithdrawalManager.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



UserWithdrawalManager.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



UserWithdrawalManager.sol#240
Severity: Low
240             bytes calldata pubkey,



UserWithdrawalManager.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



UserWithdrawalManager.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



UserWithdrawalManager.sol#242
Severity: Low
242             bytes calldata depositSignature,



UserWithdrawalManager.sol#242
Severity: Low
242             bytes calldata depositSignature,



UserWithdrawalManager.sol#243
Severity: Low
243             address withdrawVaultAddress,



UserWithdrawalManager.sol#244
Severity: Low
244             uint256 operatorId,



UserWithdrawalManager.sol#245
Severity: Low
245             uint256 depositTime,



UserWithdrawalManager.sol#246
Severity: Low
246             uint256 withdrawnTime



UserWithdrawalManager.sol#256
Severity: Low
256             string calldata operatorName,



UserWithdrawalManager.sol#257
Severity: Low
257             address payable operatorRewardAddress,



UserWithdrawalManager.sol#258
Severity: Low
258             address operatorAddress



UserWithdrawalManager.sol#324
Severity: Low
324     error EmptyNameString();



UserWithdrawalManager.sol#324
Severity: Low
324     error EmptyNameString();



UserWithdrawalManager.sol#325
Severity: Low
325     error PoolIdNotPresent();



UserWithdrawalManager.sol#325
Severity: Low
325     error PoolIdNotPresent();



UserWithdrawalManager.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



UserWithdrawalManager.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



UserWithdrawalManager.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



UserWithdrawalManager.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



UserWithdrawalManager.sol#328
Severity: Low
328     error NameCrossedMaxLength();



UserWithdrawalManager.sol#328
Severity: Low
328     error NameCrossedMaxLength();



UserWithdrawalManager.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



UserWithdrawalManager.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



UserWithdrawalManager.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



UserWithdrawalManager.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



UserWithdrawalManager.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



UserWithdrawalManager.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



UserWithdrawalManager.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



UserWithdrawalManager.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



UserWithdrawalManager.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



UserWithdrawalManager.sol#396
Severity: Low
396         bytes calldata _depositSignature



UserWithdrawalManager.sol#410
Severity: Low
410     error CallerNotOwner();



UserWithdrawalManager.sol#410
Severity: Low
410     error CallerNotOwner();



UserWithdrawalManager.sol#411
Severity: Low
411     error AlreadyInitialized();



UserWithdrawalManager.sol#411
Severity: Low
411     error AlreadyInitialized();



UserWithdrawalManager.sol#437
Severity: Low
437     error ZeroAddress();



UserWithdrawalManager.sol#437
Severity: Low
437     error ZeroAddress();



UserWithdrawalManager.sol#438
Severity: Low
438     error InvalidPubkeyLength();



UserWithdrawalManager.sol#438
Severity: Low
438     error InvalidPubkeyLength();



UserWithdrawalManager.sol#439
Severity: Low
439     error CallerNotManager();



UserWithdrawalManager.sol#439
Severity: Low
439     error CallerNotManager();



UserWithdrawalManager.sol#440
Severity: Low
440     error CallerNotOperator();



UserWithdrawalManager.sol#440
Severity: Low
440     error CallerNotOperator();



UserWithdrawalManager.sol#441
Severity: Low
441     error CallerNotStaderContract();



UserWithdrawalManager.sol#441
Severity: Low
441     error CallerNotStaderContract();



UserWithdrawalManager.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



UserWithdrawalManager.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



UserWithdrawalManager.sol#443
Severity: Low
443     error TransferFailed();



UserWithdrawalManager.sol#443
Severity: Low
443     error TransferFailed();



UserWithdrawalManager.sol#768
Severity: Low
768     function sendValue(address payable recipient, uint256 amount) internal {



UserWithdrawalManager.sol#768
Severity: Low
768     function sendValue(address payable recipient, uint256 amount) internal {



UserWithdrawalManager.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



UserWithdrawalManager.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



UserWithdrawalManager.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



UserWithdrawalManager.sol#769
Severity: Low
769         require(address(this).balance >= amount, "Address: insufficient balance");



UserWithdrawalManager.sol#771
Severity: Low
771         (bool success, ) = recipient.call{value: amount}("");



UserWithdrawalManager.sol#771
Severity: Low
771         (bool success, ) = recipient.call{value: amount}("");



UserWithdrawalManager.sol#771
Severity: Low
771         (bool success, ) = recipient.call{value: amount}("");



UserWithdrawalManager.sol#2535
Severity: Low
2535     error ETHTransferFailed(address recipient, uint256 amount);



UserWithdrawalManager.sol#2535
Severity: Low
2535     error ETHTransferFailed(address recipient, uint256 amount);



UserWithdrawalManager.sol#2535
Severity: Low
2535     error ETHTransferFailed(address recipient, uint256 amount);



UserWithdrawalManager.sol#2536
Severity: Low
2536     error SDTransferFailed();



UserWithdrawalManager.sol#2536
Severity: Low
2536     error SDTransferFailed();



UserWithdrawalManager.sol#2537
Severity: Low
2537     error RewardAlreadyHandled();



UserWithdrawalManager.sol#2537
Severity: Low
2537     error RewardAlreadyHandled();



UserWithdrawalManager.sol#2538
Severity: Low
2538     error RewardAlreadyClaimed(address operator, uint256 cycle);



UserWithdrawalManager.sol#2538
Severity: Low
2538     error RewardAlreadyClaimed(address operator, uint256 cycle);



UserWithdrawalManager.sol#2538
Severity: Low
2538     error RewardAlreadyClaimed(address operator, uint256 cycle);



UserWithdrawalManager.sol#2539
Severity: Low
2539     error InsufficientETHRewards();



UserWithdrawalManager.sol#2539
Severity: Low
2539     error InsufficientETHRewards();



UserWithdrawalManager.sol#2540
Severity: Low
2540     error InsufficientSDRewards();



UserWithdrawalManager.sol#2540
Severity: Low
2540     error InsufficientSDRewards();



UserWithdrawalManager.sol#2541
Severity: Low
2541     error InvalidAmount();



UserWithdrawalManager.sol#2541
Severity: Low
2541     error InvalidAmount();



UserWithdrawalManager.sol#2542
Severity: Low
2542     error InvalidProof(uint256 cycle, address operator);



UserWithdrawalManager.sol#2542
Severity: Low
2542     error InvalidProof(uint256 cycle, address operator);



UserWithdrawalManager.sol#2542
Severity: Low
2542     error InvalidProof(uint256 cycle, address operator);



UserWithdrawalManager.sol#2543
Severity: Low
2543     error InvalidCycleIndex();



UserWithdrawalManager.sol#2543
Severity: Low
2543     error InvalidCycleIndex();



UserWithdrawalManager.sol#2544
Severity: Low
2544     error FutureCycleIndex();



UserWithdrawalManager.sol#2544
Severity: Low
2544     error FutureCycleIndex();



UserWithdrawalManager.sol#2567
Severity: Low
2567         uint256[] calldata _amountSD,



UserWithdrawalManager.sol#2568
Severity: Low
2568         uint256[] calldata _amountETH,



UserWithdrawalManager.sol#2568
Severity: Low
2568         uint256[] calldata _amountETH,



UserWithdrawalManager.sol#2569
Severity: Low
2569         bytes32[][] calldata _merkleProof



UserWithdrawalManager.sol#2667
Severity: Low
2667     error InvalidUpdate();



UserWithdrawalManager.sol#2667
Severity: Low
2667     error InvalidUpdate();



UserWithdrawalManager.sol#2668
Severity: Low
2668     error NodeAlreadyTrusted();



UserWithdrawalManager.sol#2668
Severity: Low
2668     error NodeAlreadyTrusted();



UserWithdrawalManager.sol#2669
Severity: Low
2669     error NodeNotTrusted();



UserWithdrawalManager.sol#2669
Severity: Low
2669     error NodeNotTrusted();



UserWithdrawalManager.sol#2670
Severity: Low
2670     error ZeroFrequency();



UserWithdrawalManager.sol#2670
Severity: Low
2670     error ZeroFrequency();



UserWithdrawalManager.sol#2671
Severity: Low
2671     error FrequencyUnchanged();



UserWithdrawalManager.sol#2671
Severity: Low
2671     error FrequencyUnchanged();



UserWithdrawalManager.sol#2672
Severity: Low
2672     error DuplicateSubmissionFromNode();



UserWithdrawalManager.sol#2672
Severity: Low
2672     error DuplicateSubmissionFromNode();



UserWithdrawalManager.sol#2673
Severity: Low
2673     error ReportingFutureBlockData();



UserWithdrawalManager.sol#2673
Severity: Low
2673     error ReportingFutureBlockData();



UserWithdrawalManager.sol#2674
Severity: Low
2674     error InvalidMerkleRootIndex();



UserWithdrawalManager.sol#2674
Severity: Low
2674     error InvalidMerkleRootIndex();



UserWithdrawalManager.sol#2675
Severity: Low
2675     error ReportingPreviousCycleData();



UserWithdrawalManager.sol#2675
Severity: Low
2675     error ReportingPreviousCycleData();



UserWithdrawalManager.sol#2676
Severity: Low
2676     error InvalidMAPDIndex();



UserWithdrawalManager.sol#2676
Severity: Low
2676     error InvalidMAPDIndex();



UserWithdrawalManager.sol#2677
Severity: Low
2677     error PageNumberAlreadyReported();



UserWithdrawalManager.sol#2677
Severity: Low
2677     error PageNumberAlreadyReported();



UserWithdrawalManager.sol#2678
Severity: Low
2678     error NotATrustedNode();



UserWithdrawalManager.sol#2678
Severity: Low
2678     error NotATrustedNode();



UserWithdrawalManager.sol#2679
Severity: Low
2679     error InvalidERDataSource();



UserWithdrawalManager.sol#2679
Severity: Low
2679     error InvalidERDataSource();



UserWithdrawalManager.sol#2680
Severity: Low
2680     error InspectionModeActive();



UserWithdrawalManager.sol#2680
Severity: Low
2680     error InspectionModeActive();



UserWithdrawalManager.sol#2681
Severity: Low
2681     error UpdateFrequencyNotSet();



UserWithdrawalManager.sol#2681
Severity: Low
2681     error UpdateFrequencyNotSet();



UserWithdrawalManager.sol#2682
Severity: Low
2682     error InvalidReportingBlock();



UserWithdrawalManager.sol#2682
Severity: Low
2682     error InvalidReportingBlock();



UserWithdrawalManager.sol#2683
Severity: Low
2683     error ERChangeLimitCrossed();



UserWithdrawalManager.sol#2683
Severity: Low
2683     error ERChangeLimitCrossed();



UserWithdrawalManager.sol#2684
Severity: Low
2684     error ERChangeLimitNotCrossed();



UserWithdrawalManager.sol#2684
Severity: Low
2684     error ERChangeLimitNotCrossed();



UserWithdrawalManager.sol#2685
Severity: Low
2685     error ERPermissibleChangeOutofBounds();



UserWithdrawalManager.sol#2685
Severity: Low
2685     error ERPermissibleChangeOutofBounds();



UserWithdrawalManager.sol#2686
Severity: Low
2686     error InsufficientTrustedNodes();



UserWithdrawalManager.sol#2686
Severity: Low
2686     error InsufficientTrustedNodes();



UserWithdrawalManager.sol#2687
Severity: Low
2687     error CooldownNotComplete();



UserWithdrawalManager.sol#2687
Severity: Low
2687     error CooldownNotComplete();



UserWithdrawalManager.sol#2891
Severity: Low
2891     error InvalidDepositAmount();



UserWithdrawalManager.sol#2891
Severity: Low
2891     error InvalidDepositAmount();



UserWithdrawalManager.sol#2892
Severity: Low
2892     error UnsupportedOperation();



UserWithdrawalManager.sol#2892
Severity: Low
2892     error UnsupportedOperation();



UserWithdrawalManager.sol#2893
Severity: Low
2893     error InsufficientBalance();



UserWithdrawalManager.sol#2893
Severity: Low
2893     error InsufficientBalance();



UserWithdrawalManager.sol#2894
Severity: Low
2894     error TransferFailed();



UserWithdrawalManager.sol#2894
Severity: Low
2894     error TransferFailed();



UserWithdrawalManager.sol#2895
Severity: Low
2895     error PoolIdDoesNotExit();



UserWithdrawalManager.sol#2895
Severity: Low
2895     error PoolIdDoesNotExit();



UserWithdrawalManager.sol#2896
Severity: Low
2896     error CooldownNotComplete();



UserWithdrawalManager.sol#2896
Severity: Low
2896     error CooldownNotComplete();



UserWithdrawalManager.sol#2897
Severity: Low
2897     error UnsupportedOperationInSafeMode();



UserWithdrawalManager.sol#2897
Severity: Low
2897     error UnsupportedOperationInSafeMode();



UserWithdrawalManager.sol#2947
Severity: Low
2947     error ETHTransferFailed();



UserWithdrawalManager.sol#2947
Severity: Low
2947     error ETHTransferFailed();



UserWithdrawalManager.sol#2948
Severity: Low
2948     error UnsupportedOperationInSafeMode();



UserWithdrawalManager.sol#2948
Severity: Low
2948     error UnsupportedOperationInSafeMode();



UserWithdrawalManager.sol#2949
Severity: Low
2949     error InSufficientBalance();



UserWithdrawalManager.sol#2949
Severity: Low
2949     error InSufficientBalance();



UserWithdrawalManager.sol#2950
Severity: Low
2950     error ProtocolNotHealthy();



UserWithdrawalManager.sol#2950
Severity: Low
2950     error ProtocolNotHealthy();



UserWithdrawalManager.sol#2951
Severity: Low
2951     error InvalidWithdrawAmount();



UserWithdrawalManager.sol#2951
Severity: Low
2951     error InvalidWithdrawAmount();



UserWithdrawalManager.sol#2952
Severity: Low
2952     error requestIdNotFinalized(uint256 _requestId);



UserWithdrawalManager.sol#2952
Severity: Low
2952     error requestIdNotFinalized(uint256 _requestId);



UserWithdrawalManager.sol#2953
Severity: Low
2953     error RequestAlreadyRedeemed(uint256 _requestId);



UserWithdrawalManager.sol#2953
Severity: Low
2953     error RequestAlreadyRedeemed(uint256 _requestId);



UserWithdrawalManager.sol#2954
Severity: Low
2954     error MaxLimitOnWithdrawRequestCountReached();



UserWithdrawalManager.sol#2954
Severity: Low
2954     error MaxLimitOnWithdrawRequestCountReached();



UserWithdrawalManager.sol#2955
Severity: Low
2955     error CannotFindRequestId();



UserWithdrawalManager.sol#2955
Severity: Low
2955     error CannotFindRequestId();



UserWithdrawalManager.sol#2956
Severity: Low
2956     error CallerNotAuthorizedToRedeem();



UserWithdrawalManager.sol#2956
Severity: Low
2956     error CallerNotAuthorizedToRedeem();



UserWithdrawalManager.sol#2957
Severity: Low
2957     error ZeroAddressReceived();



UserWithdrawalManager.sol#2957
Severity: Low
2957     error ZeroAddressReceived();



UserWithdrawalManager.sol#2994
Severity: Low
2994             address payable owner,



UserWithdrawalManager.sol#2995
Severity: Low
2995             uint256 ethXAmount,



UserWithdrawalManager.sol#2996
Severity: Low
2996             uint256 ethExpected,



UserWithdrawalManager.sol#2997
Severity: Low
2997             uint256 ethFinalized,



UserWithdrawalManager.sol#2998
Severity: Low
2998             uint256 requestTime



UserWithdrawalManager.sol#3534
Severity: Low
3534     receive() external payable {



UserWithdrawalManager.sol#3535
Severity: Low
3535         emit ReceivedETH(msg.value);



UserWithdrawalManager.sol#3535
Severity: Low
3535         emit ReceivedETH(msg.value);



```

### UtilLib.sol

```

UtilLib.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



UtilLib.sol#393
Severity: Low
393     function onlyValidKeys(



UtilLib.sol#6
Severity: Low
6     error InvalidLimits();



UtilLib.sol#6
Severity: Low
6     error InvalidLimits();



UtilLib.sol#7
Severity: Low
7     error InvalidMinDepositValue();



UtilLib.sol#7
Severity: Low
7     error InvalidMinDepositValue();



UtilLib.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



UtilLib.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



UtilLib.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



UtilLib.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



UtilLib.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



UtilLib.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



UtilLib.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



UtilLib.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



UtilLib.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



UtilLib.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



UtilLib.sol#198
Severity: Low
198     error maxKeyLimitReached();



UtilLib.sol#198
Severity: Low
198     error maxKeyLimitReached();



UtilLib.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



UtilLib.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



UtilLib.sol#200
Severity: Low
200     error InvalidKeyCount();



UtilLib.sol#200
Severity: Low
200     error InvalidKeyCount();



UtilLib.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



UtilLib.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



UtilLib.sol#202
Severity: Low
202     error OperatorIsDeactivate();



UtilLib.sol#202
Severity: Low
202     error OperatorIsDeactivate();



UtilLib.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



UtilLib.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



UtilLib.sol#204
Severity: Low
204     error PageNumberIsZero();



UtilLib.sol#204
Severity: Low
204     error PageNumberIsZero();



UtilLib.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



UtilLib.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



UtilLib.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



UtilLib.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



UtilLib.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



UtilLib.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



UtilLib.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



UtilLib.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



UtilLib.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



UtilLib.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



UtilLib.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



UtilLib.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



UtilLib.sol#240
Severity: Low
240             bytes calldata pubkey,



UtilLib.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



UtilLib.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



UtilLib.sol#242
Severity: Low
242             bytes calldata depositSignature,



UtilLib.sol#242
Severity: Low
242             bytes calldata depositSignature,



UtilLib.sol#243
Severity: Low
243             address withdrawVaultAddress,



UtilLib.sol#244
Severity: Low
244             uint256 operatorId,



UtilLib.sol#245
Severity: Low
245             uint256 depositTime,



UtilLib.sol#246
Severity: Low
246             uint256 withdrawnTime



UtilLib.sol#256
Severity: Low
256             string calldata operatorName,



UtilLib.sol#257
Severity: Low
257             address payable operatorRewardAddress,



UtilLib.sol#258
Severity: Low
258             address operatorAddress



UtilLib.sol#324
Severity: Low
324     error EmptyNameString();



UtilLib.sol#324
Severity: Low
324     error EmptyNameString();



UtilLib.sol#325
Severity: Low
325     error PoolIdNotPresent();



UtilLib.sol#325
Severity: Low
325     error PoolIdNotPresent();



UtilLib.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



UtilLib.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



UtilLib.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



UtilLib.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



UtilLib.sol#328
Severity: Low
328     error NameCrossedMaxLength();



UtilLib.sol#328
Severity: Low
328     error NameCrossedMaxLength();



UtilLib.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



UtilLib.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



UtilLib.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



UtilLib.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



UtilLib.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



UtilLib.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



UtilLib.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



UtilLib.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



UtilLib.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



UtilLib.sol#396
Severity: Low
396         bytes calldata _depositSignature



UtilLib.sol#410
Severity: Low
410     error CallerNotOwner();



UtilLib.sol#410
Severity: Low
410     error CallerNotOwner();



UtilLib.sol#411
Severity: Low
411     error AlreadyInitialized();



UtilLib.sol#411
Severity: Low
411     error AlreadyInitialized();



UtilLib.sol#437
Severity: Low
437     error ZeroAddress();



UtilLib.sol#437
Severity: Low
437     error ZeroAddress();



UtilLib.sol#438
Severity: Low
438     error InvalidPubkeyLength();



UtilLib.sol#438
Severity: Low
438     error InvalidPubkeyLength();



UtilLib.sol#439
Severity: Low
439     error CallerNotManager();



UtilLib.sol#439
Severity: Low
439     error CallerNotManager();



UtilLib.sol#440
Severity: Low
440     error CallerNotOperator();



UtilLib.sol#440
Severity: Low
440     error CallerNotOperator();



UtilLib.sol#441
Severity: Low
441     error CallerNotStaderContract();



UtilLib.sol#441
Severity: Low
441     error CallerNotStaderContract();



UtilLib.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



UtilLib.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



UtilLib.sol#443
Severity: Low
443     error TransferFailed();



UtilLib.sol#443
Severity: Low
443     error TransferFailed();



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



ValidatorWithdrawalVault.sol#393
Severity: Low
393     function onlyValidKeys(



ValidatorWithdrawalVault.sol#612
Severity: Low
612     constructor() {}



ValidatorWithdrawalVault.sol#1174
Severity: Low
1174     constructor() {}



ValidatorWithdrawalVault.sol#6
Severity: Low
6     error InvalidLimits();



ValidatorWithdrawalVault.sol#6
Severity: Low
6     error InvalidLimits();



ValidatorWithdrawalVault.sol#7
Severity: Low
7     error InvalidMinDepositValue();



ValidatorWithdrawalVault.sol#7
Severity: Low
7     error InvalidMinDepositValue();



ValidatorWithdrawalVault.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



ValidatorWithdrawalVault.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



ValidatorWithdrawalVault.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



ValidatorWithdrawalVault.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



ValidatorWithdrawalVault.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



ValidatorWithdrawalVault.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



ValidatorWithdrawalVault.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



ValidatorWithdrawalVault.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



ValidatorWithdrawalVault.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



ValidatorWithdrawalVault.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



ValidatorWithdrawalVault.sol#198
Severity: Low
198     error maxKeyLimitReached();



ValidatorWithdrawalVault.sol#198
Severity: Low
198     error maxKeyLimitReached();



ValidatorWithdrawalVault.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



ValidatorWithdrawalVault.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



ValidatorWithdrawalVault.sol#200
Severity: Low
200     error InvalidKeyCount();



ValidatorWithdrawalVault.sol#200
Severity: Low
200     error InvalidKeyCount();



ValidatorWithdrawalVault.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



ValidatorWithdrawalVault.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



ValidatorWithdrawalVault.sol#202
Severity: Low
202     error OperatorIsDeactivate();



ValidatorWithdrawalVault.sol#202
Severity: Low
202     error OperatorIsDeactivate();



ValidatorWithdrawalVault.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



ValidatorWithdrawalVault.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



ValidatorWithdrawalVault.sol#204
Severity: Low
204     error PageNumberIsZero();



ValidatorWithdrawalVault.sol#204
Severity: Low
204     error PageNumberIsZero();



ValidatorWithdrawalVault.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



ValidatorWithdrawalVault.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



ValidatorWithdrawalVault.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



ValidatorWithdrawalVault.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



ValidatorWithdrawalVault.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



ValidatorWithdrawalVault.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



ValidatorWithdrawalVault.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



ValidatorWithdrawalVault.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



ValidatorWithdrawalVault.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



ValidatorWithdrawalVault.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



ValidatorWithdrawalVault.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



ValidatorWithdrawalVault.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



ValidatorWithdrawalVault.sol#240
Severity: Low
240             bytes calldata pubkey,



ValidatorWithdrawalVault.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



ValidatorWithdrawalVault.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



ValidatorWithdrawalVault.sol#242
Severity: Low
242             bytes calldata depositSignature,



ValidatorWithdrawalVault.sol#242
Severity: Low
242             bytes calldata depositSignature,



ValidatorWithdrawalVault.sol#243
Severity: Low
243             address withdrawVaultAddress,



ValidatorWithdrawalVault.sol#244
Severity: Low
244             uint256 operatorId,



ValidatorWithdrawalVault.sol#245
Severity: Low
245             uint256 depositTime,



ValidatorWithdrawalVault.sol#246
Severity: Low
246             uint256 withdrawnTime



ValidatorWithdrawalVault.sol#256
Severity: Low
256             string calldata operatorName,



ValidatorWithdrawalVault.sol#257
Severity: Low
257             address payable operatorRewardAddress,



ValidatorWithdrawalVault.sol#258
Severity: Low
258             address operatorAddress



ValidatorWithdrawalVault.sol#324
Severity: Low
324     error EmptyNameString();



ValidatorWithdrawalVault.sol#324
Severity: Low
324     error EmptyNameString();



ValidatorWithdrawalVault.sol#325
Severity: Low
325     error PoolIdNotPresent();



ValidatorWithdrawalVault.sol#325
Severity: Low
325     error PoolIdNotPresent();



ValidatorWithdrawalVault.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



ValidatorWithdrawalVault.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



ValidatorWithdrawalVault.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



ValidatorWithdrawalVault.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



ValidatorWithdrawalVault.sol#328
Severity: Low
328     error NameCrossedMaxLength();



ValidatorWithdrawalVault.sol#328
Severity: Low
328     error NameCrossedMaxLength();



ValidatorWithdrawalVault.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



ValidatorWithdrawalVault.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



ValidatorWithdrawalVault.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



ValidatorWithdrawalVault.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



ValidatorWithdrawalVault.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



ValidatorWithdrawalVault.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



ValidatorWithdrawalVault.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



ValidatorWithdrawalVault.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



ValidatorWithdrawalVault.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



ValidatorWithdrawalVault.sol#396
Severity: Low
396         bytes calldata _depositSignature



ValidatorWithdrawalVault.sol#410
Severity: Low
410     error CallerNotOwner();



ValidatorWithdrawalVault.sol#410
Severity: Low
410     error CallerNotOwner();



ValidatorWithdrawalVault.sol#411
Severity: Low
411     error AlreadyInitialized();



ValidatorWithdrawalVault.sol#411
Severity: Low
411     error AlreadyInitialized();



ValidatorWithdrawalVault.sol#437
Severity: Low
437     error ZeroAddress();



ValidatorWithdrawalVault.sol#437
Severity: Low
437     error ZeroAddress();



ValidatorWithdrawalVault.sol#438
Severity: Low
438     error InvalidPubkeyLength();



ValidatorWithdrawalVault.sol#438
Severity: Low
438     error InvalidPubkeyLength();



ValidatorWithdrawalVault.sol#439
Severity: Low
439     error CallerNotManager();



ValidatorWithdrawalVault.sol#439
Severity: Low
439     error CallerNotManager();



ValidatorWithdrawalVault.sol#440
Severity: Low
440     error CallerNotOperator();



ValidatorWithdrawalVault.sol#440
Severity: Low
440     error CallerNotOperator();



ValidatorWithdrawalVault.sol#441
Severity: Low
441     error CallerNotStaderContract();



ValidatorWithdrawalVault.sol#441
Severity: Low
441     error CallerNotStaderContract();



ValidatorWithdrawalVault.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



ValidatorWithdrawalVault.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



ValidatorWithdrawalVault.sol#443
Severity: Low
443     error TransferFailed();



ValidatorWithdrawalVault.sol#443
Severity: Low
443     error TransferFailed();



ValidatorWithdrawalVault.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



ValidatorWithdrawalVault.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



ValidatorWithdrawalVault.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



ValidatorWithdrawalVault.sol#637
Severity: Low
637         address vaultImplementation = isValidatorWithdrawalVault



ValidatorWithdrawalVault.sol#640
Severity: Low
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



ValidatorWithdrawalVault.sol#640
Severity: Low
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



ValidatorWithdrawalVault.sol#641
Severity: Low
641         if (!success) {



ValidatorWithdrawalVault.sol#642
Severity: Low
642             revert(string(data));



ValidatorWithdrawalVault.sol#642
Severity: Low
642             revert(string(data));



ValidatorWithdrawalVault.sol#681
Severity: Low
681     error ValidatorSettled();



ValidatorWithdrawalVault.sol#681
Severity: Low
681     error ValidatorSettled();



ValidatorWithdrawalVault.sol#772
Severity: Low
772     error InvalidDepositAmount();



ValidatorWithdrawalVault.sol#772
Severity: Low
772     error InvalidDepositAmount();



ValidatorWithdrawalVault.sol#773
Severity: Low
773     error UnsupportedOperation();



ValidatorWithdrawalVault.sol#773
Severity: Low
773     error UnsupportedOperation();



ValidatorWithdrawalVault.sol#774
Severity: Low
774     error InsufficientBalance();



ValidatorWithdrawalVault.sol#774
Severity: Low
774     error InsufficientBalance();



ValidatorWithdrawalVault.sol#775
Severity: Low
775     error TransferFailed();



ValidatorWithdrawalVault.sol#775
Severity: Low
775     error TransferFailed();



ValidatorWithdrawalVault.sol#776
Severity: Low
776     error PoolIdDoesNotExit();



ValidatorWithdrawalVault.sol#776
Severity: Low
776     error PoolIdDoesNotExit();



ValidatorWithdrawalVault.sol#777
Severity: Low
777     error CooldownNotComplete();



ValidatorWithdrawalVault.sol#777
Severity: Low
777     error CooldownNotComplete();



ValidatorWithdrawalVault.sol#778
Severity: Low
778     error UnsupportedOperationInSafeMode();



ValidatorWithdrawalVault.sol#778
Severity: Low
778     error UnsupportedOperationInSafeMode();



ValidatorWithdrawalVault.sol#828
Severity: Low
828     error InvalidRewardAmount();



ValidatorWithdrawalVault.sol#828
Severity: Low
828     error InvalidRewardAmount();



ValidatorWithdrawalVault.sol#829
Severity: Low
829     error NotEnoughRewardToDistribute();



ValidatorWithdrawalVault.sol#829
Severity: Low
829     error NotEnoughRewardToDistribute();



ValidatorWithdrawalVault.sol#830
Severity: Low
830     error CallerNotNodeRegistryContract();



ValidatorWithdrawalVault.sol#830
Severity: Low
830     error CallerNotNodeRegistryContract();



ValidatorWithdrawalVault.sol#870
Severity: Low
870     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



ValidatorWithdrawalVault.sol#870
Severity: Low
870     error InsufficientSDToWithdraw(uint256 operatorSDCollateral);



ValidatorWithdrawalVault.sol#871
Severity: Low
871     error InvalidPoolId();



ValidatorWithdrawalVault.sol#871
Severity: Low
871     error InvalidPoolId();



ValidatorWithdrawalVault.sol#872
Severity: Low
872     error InvalidPoolLimit();



ValidatorWithdrawalVault.sol#872
Severity: Low
872     error InvalidPoolLimit();



ValidatorWithdrawalVault.sol#873
Severity: Low
873     error SDTransferFailed();



ValidatorWithdrawalVault.sol#873
Severity: Low
873     error SDTransferFailed();



ValidatorWithdrawalVault.sol#874
Severity: Low
874     error NoStateChange();



ValidatorWithdrawalVault.sol#874
Severity: Low
874     error NoStateChange();



ValidatorWithdrawalVault.sol#1177
Severity: Low
1177     receive() external payable {



ValidatorWithdrawalVault.sol#1178
Severity: Low
1178         emit ETHReceived(msg.sender, msg.value);



ValidatorWithdrawalVault.sol#1178
Severity: Low
1178         emit ETHReceived(msg.sender, msg.value);



ValidatorWithdrawalVault.sol#1178
Severity: Low
1178         emit ETHReceived(msg.sender, msg.value);



```

### VaultFactory.sol

```

VaultFactory.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



VaultFactory.sol#393
Severity: Low
393     function onlyValidKeys(



VaultFactory.sol#612
Severity: Low
612     constructor() {}



VaultFactory.sol#945
Severity: Low
945     function sendValue(address payable recipient, uint256 amount) internal {



VaultFactory.sol#2023
Severity: Low
2023     constructor() {



VaultFactory.sol#6
Severity: Low
6     error InvalidLimits();



VaultFactory.sol#6
Severity: Low
6     error InvalidLimits();



VaultFactory.sol#7
Severity: Low
7     error InvalidMinDepositValue();



VaultFactory.sol#7
Severity: Low
7     error InvalidMinDepositValue();



VaultFactory.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



VaultFactory.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



VaultFactory.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



VaultFactory.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



VaultFactory.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



VaultFactory.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



VaultFactory.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



VaultFactory.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



VaultFactory.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



VaultFactory.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



VaultFactory.sol#198
Severity: Low
198     error maxKeyLimitReached();



VaultFactory.sol#198
Severity: Low
198     error maxKeyLimitReached();



VaultFactory.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



VaultFactory.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



VaultFactory.sol#200
Severity: Low
200     error InvalidKeyCount();



VaultFactory.sol#200
Severity: Low
200     error InvalidKeyCount();



VaultFactory.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



VaultFactory.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



VaultFactory.sol#202
Severity: Low
202     error OperatorIsDeactivate();



VaultFactory.sol#202
Severity: Low
202     error OperatorIsDeactivate();



VaultFactory.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



VaultFactory.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



VaultFactory.sol#204
Severity: Low
204     error PageNumberIsZero();



VaultFactory.sol#204
Severity: Low
204     error PageNumberIsZero();



VaultFactory.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



VaultFactory.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



VaultFactory.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



VaultFactory.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



VaultFactory.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



VaultFactory.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



VaultFactory.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



VaultFactory.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



VaultFactory.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



VaultFactory.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



VaultFactory.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



VaultFactory.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



VaultFactory.sol#240
Severity: Low
240             bytes calldata pubkey,



VaultFactory.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



VaultFactory.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



VaultFactory.sol#242
Severity: Low
242             bytes calldata depositSignature,



VaultFactory.sol#242
Severity: Low
242             bytes calldata depositSignature,



VaultFactory.sol#243
Severity: Low
243             address withdrawVaultAddress,



VaultFactory.sol#244
Severity: Low
244             uint256 operatorId,



VaultFactory.sol#245
Severity: Low
245             uint256 depositTime,



VaultFactory.sol#246
Severity: Low
246             uint256 withdrawnTime



VaultFactory.sol#256
Severity: Low
256             string calldata operatorName,



VaultFactory.sol#257
Severity: Low
257             address payable operatorRewardAddress,



VaultFactory.sol#258
Severity: Low
258             address operatorAddress



VaultFactory.sol#324
Severity: Low
324     error EmptyNameString();



VaultFactory.sol#324
Severity: Low
324     error EmptyNameString();



VaultFactory.sol#325
Severity: Low
325     error PoolIdNotPresent();



VaultFactory.sol#325
Severity: Low
325     error PoolIdNotPresent();



VaultFactory.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



VaultFactory.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



VaultFactory.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



VaultFactory.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



VaultFactory.sol#328
Severity: Low
328     error NameCrossedMaxLength();



VaultFactory.sol#328
Severity: Low
328     error NameCrossedMaxLength();



VaultFactory.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



VaultFactory.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



VaultFactory.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



VaultFactory.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



VaultFactory.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



VaultFactory.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



VaultFactory.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



VaultFactory.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



VaultFactory.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



VaultFactory.sol#396
Severity: Low
396         bytes calldata _depositSignature



VaultFactory.sol#410
Severity: Low
410     error CallerNotOwner();



VaultFactory.sol#410
Severity: Low
410     error CallerNotOwner();



VaultFactory.sol#411
Severity: Low
411     error AlreadyInitialized();



VaultFactory.sol#411
Severity: Low
411     error AlreadyInitialized();



VaultFactory.sol#437
Severity: Low
437     error ZeroAddress();



VaultFactory.sol#437
Severity: Low
437     error ZeroAddress();



VaultFactory.sol#438
Severity: Low
438     error InvalidPubkeyLength();



VaultFactory.sol#438
Severity: Low
438     error InvalidPubkeyLength();



VaultFactory.sol#439
Severity: Low
439     error CallerNotManager();



VaultFactory.sol#439
Severity: Low
439     error CallerNotManager();



VaultFactory.sol#440
Severity: Low
440     error CallerNotOperator();



VaultFactory.sol#440
Severity: Low
440     error CallerNotOperator();



VaultFactory.sol#441
Severity: Low
441     error CallerNotStaderContract();



VaultFactory.sol#441
Severity: Low
441     error CallerNotStaderContract();



VaultFactory.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



VaultFactory.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



VaultFactory.sol#443
Severity: Low
443     error TransferFailed();



VaultFactory.sol#443
Severity: Low
443     error TransferFailed();



VaultFactory.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



VaultFactory.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



VaultFactory.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



VaultFactory.sol#637
Severity: Low
637         address vaultImplementation = isValidatorWithdrawalVault



VaultFactory.sol#640
Severity: Low
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



VaultFactory.sol#640
Severity: Low
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



VaultFactory.sol#641
Severity: Low
641         if (!success) {



VaultFactory.sol#642
Severity: Low
642             revert(string(data));



VaultFactory.sol#642
Severity: Low
642             revert(string(data));



VaultFactory.sol#945
Severity: Low
945     function sendValue(address payable recipient, uint256 amount) internal {



VaultFactory.sol#945
Severity: Low
945     function sendValue(address payable recipient, uint256 amount) internal {



VaultFactory.sol#946
Severity: Low
946         require(address(this).balance >= amount, "Address: insufficient balance");



VaultFactory.sol#946
Severity: Low
946         require(address(this).balance >= amount, "Address: insufficient balance");



VaultFactory.sol#946
Severity: Low
946         require(address(this).balance >= amount, "Address: insufficient balance");



VaultFactory.sol#946
Severity: Low
946         require(address(this).balance >= amount, "Address: insufficient balance");



VaultFactory.sol#948
Severity: Low
948         (bool success, ) = recipient.call{value: amount}("");



VaultFactory.sol#948
Severity: Low
948         (bool success, ) = recipient.call{value: amount}("");



VaultFactory.sol#948
Severity: Low
948         (bool success, ) = recipient.call{value: amount}("");



```

### VaultProxy.sol

```

VaultProxy.sol#228
Severity: Low
228     function markValidatorReadyToDeposit(



VaultProxy.sol#393
Severity: Low
393     function onlyValidKeys(



VaultProxy.sol#612
Severity: Low
612     constructor() {}



VaultProxy.sol#6
Severity: Low
6     error InvalidLimits();



VaultProxy.sol#6
Severity: Low
6     error InvalidLimits();



VaultProxy.sol#7
Severity: Low
7     error InvalidMinDepositValue();



VaultProxy.sol#7
Severity: Low
7     error InvalidMinDepositValue();



VaultProxy.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



VaultProxy.sol#8
Severity: Low
8     error InvalidMaxDepositValue();



VaultProxy.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



VaultProxy.sol#9
Severity: Low
9     error InvalidMinWithdrawValue();



VaultProxy.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



VaultProxy.sol#10
Severity: Low
10     error InvalidMaxWithdrawValue();



VaultProxy.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



VaultProxy.sol#196
Severity: Low
196     error DuplicatePoolIDOrPoolNotAdded();



VaultProxy.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



VaultProxy.sol#197
Severity: Low
197     error OperatorAlreadyOnBoardedInProtocol();



VaultProxy.sol#198
Severity: Low
198     error maxKeyLimitReached();



VaultProxy.sol#198
Severity: Low
198     error maxKeyLimitReached();



VaultProxy.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



VaultProxy.sol#199
Severity: Low
199     error OperatorNotOnBoarded();



VaultProxy.sol#200
Severity: Low
200     error InvalidKeyCount();



VaultProxy.sol#200
Severity: Low
200     error InvalidKeyCount();



VaultProxy.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



VaultProxy.sol#201
Severity: Low
201     error InvalidStartAndEndIndex();



VaultProxy.sol#202
Severity: Low
202     error OperatorIsDeactivate();



VaultProxy.sol#202
Severity: Low
202     error OperatorIsDeactivate();



VaultProxy.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



VaultProxy.sol#203
Severity: Low
203     error MisMatchingInputKeysSize();



VaultProxy.sol#204
Severity: Low
204     error PageNumberIsZero();



VaultProxy.sol#204
Severity: Low
204     error PageNumberIsZero();



VaultProxy.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



VaultProxy.sol#205
Severity: Low
205     error UNEXPECTED_STATUS();



VaultProxy.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



VaultProxy.sol#206
Severity: Low
206     error PubkeyAlreadyExist();



VaultProxy.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



VaultProxy.sol#207
Severity: Low
207     error NotEnoughSDCollateral();



VaultProxy.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



VaultProxy.sol#208
Severity: Low
208     error TooManyVerifiedKeysReported();



VaultProxy.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



VaultProxy.sol#209
Severity: Low
209     error TooManyWithdrawnKeysReported();



VaultProxy.sol#230
Severity: Low
230         bytes[] calldata _frontRunPubkey,



VaultProxy.sol#231
Severity: Low
231         bytes[] calldata _invalidSignaturePubkey



VaultProxy.sol#240
Severity: Low
240             bytes calldata pubkey,



VaultProxy.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



VaultProxy.sol#241
Severity: Low
241             bytes calldata preDepositSignature,



VaultProxy.sol#242
Severity: Low
242             bytes calldata depositSignature,



VaultProxy.sol#242
Severity: Low
242             bytes calldata depositSignature,



VaultProxy.sol#243
Severity: Low
243             address withdrawVaultAddress,



VaultProxy.sol#244
Severity: Low
244             uint256 operatorId,



VaultProxy.sol#245
Severity: Low
245             uint256 depositTime,



VaultProxy.sol#246
Severity: Low
246             uint256 withdrawnTime



VaultProxy.sol#256
Severity: Low
256             string calldata operatorName,



VaultProxy.sol#257
Severity: Low
257             address payable operatorRewardAddress,



VaultProxy.sol#258
Severity: Low
258             address operatorAddress



VaultProxy.sol#324
Severity: Low
324     error EmptyNameString();



VaultProxy.sol#324
Severity: Low
324     error EmptyNameString();



VaultProxy.sol#325
Severity: Low
325     error PoolIdNotPresent();



VaultProxy.sol#325
Severity: Low
325     error PoolIdNotPresent();



VaultProxy.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



VaultProxy.sol#326
Severity: Low
326     error PubkeyDoesNotExit();



VaultProxy.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



VaultProxy.sol#327
Severity: Low
327     error PubkeyAlreadyExist();



VaultProxy.sol#328
Severity: Low
328     error NameCrossedMaxLength();



VaultProxy.sol#328
Severity: Low
328     error NameCrossedMaxLength();



VaultProxy.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



VaultProxy.sol#329
Severity: Low
329     error InvalidLengthOfPubkey();



VaultProxy.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



VaultProxy.sol#330
Severity: Low
330     error OperatorIsNotOnboarded();



VaultProxy.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



VaultProxy.sol#331
Severity: Low
331     error InvalidLengthOfSignature();



VaultProxy.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



VaultProxy.sol#332
Severity: Low
332     error ExistingOrMismatchingPoolId();



VaultProxy.sol#395
Severity: Low
395         bytes calldata _preDepositSignature,



VaultProxy.sol#396
Severity: Low
396         bytes calldata _depositSignature



VaultProxy.sol#410
Severity: Low
410     error CallerNotOwner();



VaultProxy.sol#410
Severity: Low
410     error CallerNotOwner();



VaultProxy.sol#411
Severity: Low
411     error AlreadyInitialized();



VaultProxy.sol#411
Severity: Low
411     error AlreadyInitialized();



VaultProxy.sol#437
Severity: Low
437     error ZeroAddress();



VaultProxy.sol#437
Severity: Low
437     error ZeroAddress();



VaultProxy.sol#438
Severity: Low
438     error InvalidPubkeyLength();



VaultProxy.sol#438
Severity: Low
438     error InvalidPubkeyLength();



VaultProxy.sol#439
Severity: Low
439     error CallerNotManager();



VaultProxy.sol#439
Severity: Low
439     error CallerNotManager();



VaultProxy.sol#440
Severity: Low
440     error CallerNotOperator();



VaultProxy.sol#440
Severity: Low
440     error CallerNotOperator();



VaultProxy.sol#441
Severity: Low
441     error CallerNotStaderContract();



VaultProxy.sol#441
Severity: Low
441     error CallerNotStaderContract();



VaultProxy.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



VaultProxy.sol#442
Severity: Low
442     error CallerNotWithdrawVault();



VaultProxy.sol#443
Severity: Low
443     error TransferFailed();



VaultProxy.sol#443
Severity: Low
443     error TransferFailed();



VaultProxy.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



VaultProxy.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



VaultProxy.sol#636
Severity: Low
636     fallback(bytes calldata _input) external payable returns (bytes memory) {



VaultProxy.sol#637
Severity: Low
637         address vaultImplementation = isValidatorWithdrawalVault



VaultProxy.sol#640
Severity: Low
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



VaultProxy.sol#640
Severity: Low
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



VaultProxy.sol#641
Severity: Low
641         if (!success) {



VaultProxy.sol#642
Severity: Low
642             revert(string(data));



VaultProxy.sol#642
Severity: Low
642             revert(string(data));



```

## SOLIDITY_ERC20_APPROVE
The ```approve``` function of ERC-20 is vulnerable. Using front-running attack one can spend approved tokens before change of ```allowance``` value.


### ETHx.sol

```

ETHx.sol#1250
Severity: Medium
1250     function approve(address spender, uint256 amount) public virtual override returns (bool) {



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#1251
Severity: Medium
1251     function approve(address spender, uint256 amount) public virtual override returns (bool) {



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#1250
Severity: Medium
1250     function approve(address spender, uint256 amount) public virtual override returns (bool) {



```

## SOLIDITY_LOCKED_MONEY
Contracts programmed to receive ether should implement a way to withdraw it, i.e., call ```transfer``` (recommended), ```send```, or ```call.value``` at least once.


### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#1946
Severity: High
1946 contract OperatorRewardsCollector is



```

### PermissionedNodeRegistry.sol

```

PermissionedNodeRegistry.sol#2452
Severity: High
2452 contract PermissionedNodeRegistry is



```

### StaderInsuranceFund.sol

```

StaderInsuranceFund.sol#1925
Severity: High
1925 contract StaderInsuranceFund is



```

## SOLIDITY_UNCHECKED_CALL
Expect calls to external contract to fail. When sending ether, check for the return value and handle errors. The recommended way of doing ether transfers is ```transfer```.


### OperatorRewardsCollector.sol

```

OperatorRewardsCollector.sol#1986
Severity: High
1986         UtilLib.sendValue(operatorRewardsAddr, amount);



```

### UserWithdrawalManager.sol

```

UserWithdrawalManager.sol#3315
Severity: High
3315         _callOptionalReturn(token, abi.encodeWithSelector(token.transfer.selector, to, value));



UserWithdrawalManager.sol#3324
Severity: High
3324         _callOptionalReturn(token, abi.encodeWithSelector(token.transferFrom.selector, from, to, value));



UserWithdrawalManager.sol#3346
Severity: High
3346         _callOptionalReturn(token, abi.encodeWithSelector(token.approve.selector, spender, value));



UserWithdrawalManager.sol#3355
Severity: High
3355         _callOptionalReturn(token, abi.encodeWithSelector(token.approve.selector, spender, newAllowance));



UserWithdrawalManager.sol#3367
Severity: High
3367             _callOptionalReturn(token, abi.encodeWithSelector(token.approve.selector, spender, newAllowance));



```

### ValidatorWithdrawalVault.sol

```

ValidatorWithdrawalVault.sol#640
Severity: High
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



```

### VaultFactory.sol

```

VaultFactory.sol#640
Severity: High
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



```

### VaultProxy.sol

```

VaultProxy.sol#640
Severity: High
640         (bool success, bytes memory data) = vaultImplementation.delegatecall(_input);



```

## SOLIDITY_SAFEMATH
```SafeMath``` library is used.


### PoolSelector.sol

```

PoolSelector.sol#2294
Severity: Low
2294     using SafeMath for uint256;



```

### StaderStakePoolsManager.sol

```

StaderStakePoolsManager.sol#3626
Severity: Low
3626     using SafeMath for uint256;



```

## SOLIDITY_EXTRA_GAS_IN_LOOPS
State variable, ```.balance```, or ```.length``` of non-memory array is used in the condition of ```for``` or ```while``` loop. In this case, every iteration of loop consumes extra gas.


### SocializingPool.sol

```

SocializingPool.sol#2292
Severity: Low
2292         for (uint256 i = 0; i < proof.length; i++) {



SocializingPool.sol#2305
Severity: Low
2305         for (uint256 i = 0; i < proof.length; i++) {



```

### StaderOracle.sol

```

StaderOracle.sol#2762
Severity: Low
2762         while ((j >= 1) && (_sdPrice < sdPrices[j - 1])) {



```

## SOLIDITY_DIV_MUL
Solidity operates only with integers. Thus, if the division is done before the  multiplication, the rounding errors can increase dramatically.
[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#arithmetic)
Precision issues.


### StaderOracle.sol

```

StaderOracle.sol#3060
Severity: Medium
3060         return (block.number / updateFrequency) * updateFrequency;



```

## SOLIDITY_FUNCTIONS_RETURNS_TYPE_AND_NO_RETURN
Function doesn't initialize return value. As result default value will be returned.


### VaultFactory.sol

```

VaultFactory.sol#731
Severity: Low
731     function clone(address implementation) internal returns (address instance) {



VaultFactory.sol#751
Severity: Low
751     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



VaultFactory.sol#767
Severity: Low
767     function predictDeterministicAddress(



```

## SOLIDITY_PRAGMAS_VERSION
Solidity source files indicate the versions of the compiler they can be compiled with.

pragma solidity ^0.4.17; // bad: compiles w 0.4.17 and above
pragma solidity 0.4.24; // good : compiles w 0.4.24 only

It is recommended to follow the latter example, as future compiler versions may handle certain language constructions in a way the developer did not foresee.


### VaultProxy.sol

```

VaultProxy.sol#2
Severity: Low
2 pragma solidity ^0.8.16;



```
