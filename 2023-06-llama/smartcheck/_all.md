
# SMARTCHECK ANALYSIS

## SOLIDITY_ADDRESS_HARDCODED
The contract contains unknown address. This address might be used for some malicious activity. Please check hardcoded address and it's usage.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#2199
Severity: Low
2199     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaAbsolutePeerReview.sol#2200
Severity: Low
2200       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaAbsolutePeerReview.sol#2201
Severity: Low
2201       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaAbsolutePeerReview.sol#2249
Severity: Low
2249         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaAbsolutePeerReview.sol#2260
Severity: Low
2260         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#2199
Severity: Low
2199     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaAbsoluteQuorum.sol#2200
Severity: Low
2200       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaAbsoluteQuorum.sol#2201
Severity: Low
2201       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaAbsoluteQuorum.sol#2249
Severity: Low
2249         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaAbsoluteQuorum.sol#2260
Severity: Low
2260         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaAccount.sol

```

LlamaAccount.sol#2759
Severity: Low
2759     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaAccount.sol#2760
Severity: Low
2760       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaAccount.sol#2761
Severity: Low
2761       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaAccount.sol#2809
Severity: Low
2809         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaAccount.sol#2820
Severity: Low
2820         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaCore.sol

```

LlamaCore.sol#1821
Severity: Low
1821     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaCore.sol#1822
Severity: Low
1822       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaCore.sol#1823
Severity: Low
1823       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaCore.sol#1871
Severity: Low
1871         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaCore.sol#1882
Severity: Low
1882         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaFactory.sol

```

LlamaFactory.sol#1943
Severity: Low
1943     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaFactory.sol#1944
Severity: Low
1944       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaFactory.sol#1945
Severity: Low
1945       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaFactory.sol#1993
Severity: Low
1993         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaFactory.sol#2004
Severity: Low
2004         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#1967
Severity: Low
1967     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaGovernanceScript.sol#1968
Severity: Low
1968       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaGovernanceScript.sol#1969
Severity: Low
1969       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaGovernanceScript.sol#2017
Severity: Low
2017         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaGovernanceScript.sol#2028
Severity: Low
2028         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1711
Severity: Low
1711     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaPolicy.sol#1712
Severity: Low
1712       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaPolicy.sol#1713
Severity: Low
1713       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaPolicy.sol#1761
Severity: Low
1761         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaPolicy.sol#1772
Severity: Low
1772         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#2199
Severity: Low
2199     return interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165



LlamaRelativeQuorum.sol#2200
Severity: Low
2200       || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721



LlamaRelativeQuorum.sol#2201
Severity: Low
2201       || interfaceId == 0x5b5e139f; // ERC165 Interface ID for ERC721Metadata



LlamaRelativeQuorum.sol#2249
Severity: Low
2249         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, "")



LlamaRelativeQuorum.sol#2260
Severity: Low
2260         || ERC721TokenReceiver(to).onERC721Received(msg.sender, address(0), id, data)



```

## SOLIDITY_DIV_MUL
Solidity operates only with integers. Thus, if the division is done before the  multiplication, the rounding errors can increase dramatically.
[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#arithmetic)
Precision issues.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#2827
Severity: Medium
2827         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#2827
Severity: Medium
2827         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaAccount.sol

```

LlamaAccount.sol#2902
Severity: Medium
2902         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaCore.sol

```

LlamaCore.sol#1964
Severity: Medium
1964         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaFactory.sol

```

LlamaFactory.sol#3464
Severity: Medium
3464         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#2595
Severity: Medium
2595         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#2002
Severity: Medium
2002         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaPolicyMetadata.sol

```

LlamaPolicyMetadata.sol#34
Severity: Medium
34         string memory result = new string(4 * ((data.length + 2) / 3));



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#2827
Severity: Medium
2827         string memory result = new string(4 * ((data.length + 2) / 3));



```

## SOLIDITY_EXTRA_GAS_IN_LOOPS
State variable, ```.balance```, or ```.length``` of non-memory array is used in the condition of ```for``` or ```while``` loop. In this case, every iteration of loop consumes extra gas.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#4410
Severity: Low
4410     for (uint256 i = 0; i < strategyConfig.forceApprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsolutePeerReview.sol#4418
Severity: Low
4418     for (uint256 i = 0; i < strategyConfig.forceDisapprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#4410
Severity: Low
4410     for (uint256 i = 0; i < strategyConfig.forceApprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsoluteQuorum.sol#4418
Severity: Low
4418     for (uint256 i = 0; i < strategyConfig.forceDisapprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#4410
Severity: Low
4410     for (uint256 i = 0; i < strategyConfig.forceApprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaRelativeQuorum.sol#4418
Severity: Low
4418     for (uint256 i = 0; i < strategyConfig.forceDisapprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



```

## SOLIDITY_FUNCTIONS_RETURNS_TYPE_AND_NO_RETURN
Function doesn't initialize return value. As result default value will be returned.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#219
Severity: Low
219     function mulDivDown(



LlamaAbsolutePeerReview.sol#236
Severity: Low
236     function mulDivUp(



LlamaAbsolutePeerReview.sol#254
Severity: Low
254     function rpow(



LlamaAbsolutePeerReview.sol#347
Severity: Low
347     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#412
Severity: Low
412     function unsafeMod(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#421
Severity: Low
421     function unsafeDiv(uint256 x, uint256 y) internal pure returns (uint256 r) {



LlamaAbsolutePeerReview.sol#430
Severity: Low
430     function unsafeDivUp(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#514
Severity: Low
514     function clone(address implementation) internal returns (address instance) {



LlamaAbsolutePeerReview.sol#536
Severity: Low
536     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaAbsolutePeerReview.sol#554
Severity: Low
554     function predictDeterministicAddress(



LlamaAbsolutePeerReview.sol#723
Severity: Low
723     function toString(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#804
Severity: Low
804     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaAbsolutePeerReview.sol#903
Severity: Low
903     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#977
Severity: Low
977     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#1027
Severity: Low
1027     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#1056
Severity: Low
1056     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaAbsolutePeerReview.sol#1074
Severity: Low
1074     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaAbsolutePeerReview.sol#1106
Severity: Low
1106     function replace(string memory subject, string memory search, string memory replacement)



LlamaAbsolutePeerReview.sol#1183
Severity: Low
1183     function indexOf(string memory subject, string memory search, uint256 from)



LlamaAbsolutePeerReview.sol#1252
Severity: Low
1252     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaAbsolutePeerReview.sol#1298
Severity: Low
1298     function startsWith(string memory subject, string memory search)



LlamaAbsolutePeerReview.sol#1319
Severity: Low
1319     function endsWith(string memory subject, string memory search)



LlamaAbsolutePeerReview.sol#1347
Severity: Low
1347     function repeat(string memory subject, uint256 times)



LlamaAbsolutePeerReview.sol#1381
Severity: Low
1381     function slice(string memory subject, uint256 start, uint256 end)



LlamaAbsolutePeerReview.sol#1424
Severity: Low
1424     function indicesOf(string memory subject, string memory search)



LlamaAbsolutePeerReview.sol#1483
Severity: Low
1483     function split(string memory subject, string memory delimiter)



LlamaAbsolutePeerReview.sol#1532
Severity: Low
1532     function concat(string memory a, string memory b)



LlamaAbsolutePeerReview.sol#1570
Severity: Low
1570     function toCase(string memory subject, bool toUpper)



LlamaAbsolutePeerReview.sol#1611
Severity: Low
1611     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaAbsolutePeerReview.sol#1645
Severity: Low
1645     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaAbsolutePeerReview.sol#1694
Severity: Low
1694     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaAbsolutePeerReview.sol#1702
Severity: Low
1702     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaAbsolutePeerReview.sol#1721
Severity: Low
1721     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaAbsolutePeerReview.sol#1739
Severity: Low
1739     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaAbsolutePeerReview.sol#1762
Severity: Low
1762     function unpackTwo(bytes32 packed)



LlamaAbsolutePeerReview.sol#1998
Severity: Low
1998     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaAbsolutePeerReview.sol#2021
Severity: Low
2021     function sqrt(uint256 x) internal pure returns (uint256 z) {



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#219
Severity: Low
219     function mulDivDown(



LlamaAbsoluteQuorum.sol#236
Severity: Low
236     function mulDivUp(



LlamaAbsoluteQuorum.sol#254
Severity: Low
254     function rpow(



LlamaAbsoluteQuorum.sol#347
Severity: Low
347     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#412
Severity: Low
412     function unsafeMod(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#421
Severity: Low
421     function unsafeDiv(uint256 x, uint256 y) internal pure returns (uint256 r) {



LlamaAbsoluteQuorum.sol#430
Severity: Low
430     function unsafeDivUp(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#514
Severity: Low
514     function clone(address implementation) internal returns (address instance) {



LlamaAbsoluteQuorum.sol#536
Severity: Low
536     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaAbsoluteQuorum.sol#554
Severity: Low
554     function predictDeterministicAddress(



LlamaAbsoluteQuorum.sol#723
Severity: Low
723     function toString(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#804
Severity: Low
804     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaAbsoluteQuorum.sol#903
Severity: Low
903     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#977
Severity: Low
977     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#1027
Severity: Low
1027     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#1056
Severity: Low
1056     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaAbsoluteQuorum.sol#1074
Severity: Low
1074     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaAbsoluteQuorum.sol#1106
Severity: Low
1106     function replace(string memory subject, string memory search, string memory replacement)



LlamaAbsoluteQuorum.sol#1183
Severity: Low
1183     function indexOf(string memory subject, string memory search, uint256 from)



LlamaAbsoluteQuorum.sol#1252
Severity: Low
1252     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaAbsoluteQuorum.sol#1298
Severity: Low
1298     function startsWith(string memory subject, string memory search)



LlamaAbsoluteQuorum.sol#1319
Severity: Low
1319     function endsWith(string memory subject, string memory search)



LlamaAbsoluteQuorum.sol#1347
Severity: Low
1347     function repeat(string memory subject, uint256 times)



LlamaAbsoluteQuorum.sol#1381
Severity: Low
1381     function slice(string memory subject, uint256 start, uint256 end)



LlamaAbsoluteQuorum.sol#1424
Severity: Low
1424     function indicesOf(string memory subject, string memory search)



LlamaAbsoluteQuorum.sol#1483
Severity: Low
1483     function split(string memory subject, string memory delimiter)



LlamaAbsoluteQuorum.sol#1532
Severity: Low
1532     function concat(string memory a, string memory b)



LlamaAbsoluteQuorum.sol#1570
Severity: Low
1570     function toCase(string memory subject, bool toUpper)



LlamaAbsoluteQuorum.sol#1611
Severity: Low
1611     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaAbsoluteQuorum.sol#1645
Severity: Low
1645     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaAbsoluteQuorum.sol#1694
Severity: Low
1694     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaAbsoluteQuorum.sol#1702
Severity: Low
1702     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaAbsoluteQuorum.sol#1721
Severity: Low
1721     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaAbsoluteQuorum.sol#1739
Severity: Low
1739     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaAbsoluteQuorum.sol#1762
Severity: Low
1762     function unpackTwo(bytes32 packed)



LlamaAbsoluteQuorum.sol#1998
Severity: Low
1998     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaAbsoluteQuorum.sol#2021
Severity: Low
2021     function sqrt(uint256 x) internal pure returns (uint256 z) {



```

### LlamaAccount.sol

```

LlamaAccount.sol#1191
Severity: Low
1191     function clone(address implementation) internal returns (address instance) {



LlamaAccount.sol#1213
Severity: Low
1213     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaAccount.sol#1231
Severity: Low
1231     function predictDeterministicAddress(



LlamaAccount.sol#1283
Severity: Low
1283     function toString(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1364
Severity: Low
1364     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaAccount.sol#1463
Severity: Low
1463     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1537
Severity: Low
1537     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaAccount.sol#1587
Severity: Low
1587     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaAccount.sol#1616
Severity: Low
1616     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaAccount.sol#1634
Severity: Low
1634     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaAccount.sol#1666
Severity: Low
1666     function replace(string memory subject, string memory search, string memory replacement)



LlamaAccount.sol#1743
Severity: Low
1743     function indexOf(string memory subject, string memory search, uint256 from)



LlamaAccount.sol#1812
Severity: Low
1812     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaAccount.sol#1858
Severity: Low
1858     function startsWith(string memory subject, string memory search)



LlamaAccount.sol#1879
Severity: Low
1879     function endsWith(string memory subject, string memory search)



LlamaAccount.sol#1907
Severity: Low
1907     function repeat(string memory subject, uint256 times)



LlamaAccount.sol#1941
Severity: Low
1941     function slice(string memory subject, uint256 start, uint256 end)



LlamaAccount.sol#1984
Severity: Low
1984     function indicesOf(string memory subject, string memory search)



LlamaAccount.sol#2043
Severity: Low
2043     function split(string memory subject, string memory delimiter)



LlamaAccount.sol#2092
Severity: Low
2092     function concat(string memory a, string memory b)



LlamaAccount.sol#2130
Severity: Low
2130     function toCase(string memory subject, bool toUpper)



LlamaAccount.sol#2171
Severity: Low
2171     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaAccount.sol#2205
Severity: Low
2205     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaAccount.sol#2254
Severity: Low
2254     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaAccount.sol#2262
Severity: Low
2262     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaAccount.sol#2281
Severity: Low
2281     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaAccount.sol#2299
Severity: Low
2299     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaAccount.sol#2322
Severity: Low
2322     function unpackTwo(bytes32 packed)



LlamaAccount.sol#2558
Severity: Low
2558     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaAccount.sol#2581
Severity: Low
2581     function sqrt(uint256 x) internal pure returns (uint256 z) {



```

### LlamaCore.sol

```

LlamaCore.sol#28
Severity: Low
28     function clone(address implementation) internal returns (address instance) {



LlamaCore.sol#50
Severity: Low
50     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaCore.sol#68
Severity: Low
68     function predictDeterministicAddress(



LlamaCore.sol#320
Severity: Low
320     function toString(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#401
Severity: Low
401     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaCore.sol#500
Severity: Low
500     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#574
Severity: Low
574     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaCore.sol#624
Severity: Low
624     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaCore.sol#653
Severity: Low
653     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaCore.sol#671
Severity: Low
671     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaCore.sol#703
Severity: Low
703     function replace(string memory subject, string memory search, string memory replacement)



LlamaCore.sol#780
Severity: Low
780     function indexOf(string memory subject, string memory search, uint256 from)



LlamaCore.sol#849
Severity: Low
849     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaCore.sol#895
Severity: Low
895     function startsWith(string memory subject, string memory search)



LlamaCore.sol#916
Severity: Low
916     function endsWith(string memory subject, string memory search)



LlamaCore.sol#944
Severity: Low
944     function repeat(string memory subject, uint256 times)



LlamaCore.sol#978
Severity: Low
978     function slice(string memory subject, uint256 start, uint256 end)



LlamaCore.sol#1021
Severity: Low
1021     function indicesOf(string memory subject, string memory search)



LlamaCore.sol#1080
Severity: Low
1080     function split(string memory subject, string memory delimiter)



LlamaCore.sol#1129
Severity: Low
1129     function concat(string memory a, string memory b)



LlamaCore.sol#1167
Severity: Low
1167     function toCase(string memory subject, bool toUpper)



LlamaCore.sol#1208
Severity: Low
1208     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaCore.sol#1242
Severity: Low
1242     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaCore.sol#1291
Severity: Low
1291     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaCore.sol#1299
Severity: Low
1299     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaCore.sol#1318
Severity: Low
1318     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaCore.sol#1336
Severity: Low
1336     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaCore.sol#1359
Severity: Low
1359     function unpackTwo(bytes32 packed)



LlamaCore.sol#1620
Severity: Low
1620     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaCore.sol#1643
Severity: Low
1643     function sqrt(uint256 x) internal pure returns (uint256 z) {



```

### LlamaFactory.sol

```

LlamaFactory.sol#28
Severity: Low
28     function clone(address implementation) internal returns (address instance) {



LlamaFactory.sol#50
Severity: Low
50     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaFactory.sol#68
Severity: Low
68     function predictDeterministicAddress(



LlamaFactory.sol#467
Severity: Low
467     function toString(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#548
Severity: Low
548     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaFactory.sol#647
Severity: Low
647     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#721
Severity: Low
721     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaFactory.sol#771
Severity: Low
771     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaFactory.sol#800
Severity: Low
800     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaFactory.sol#818
Severity: Low
818     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaFactory.sol#850
Severity: Low
850     function replace(string memory subject, string memory search, string memory replacement)



LlamaFactory.sol#927
Severity: Low
927     function indexOf(string memory subject, string memory search, uint256 from)



LlamaFactory.sol#996
Severity: Low
996     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaFactory.sol#1042
Severity: Low
1042     function startsWith(string memory subject, string memory search)



LlamaFactory.sol#1063
Severity: Low
1063     function endsWith(string memory subject, string memory search)



LlamaFactory.sol#1091
Severity: Low
1091     function repeat(string memory subject, uint256 times)



LlamaFactory.sol#1125
Severity: Low
1125     function slice(string memory subject, uint256 start, uint256 end)



LlamaFactory.sol#1168
Severity: Low
1168     function indicesOf(string memory subject, string memory search)



LlamaFactory.sol#1227
Severity: Low
1227     function split(string memory subject, string memory delimiter)



LlamaFactory.sol#1276
Severity: Low
1276     function concat(string memory a, string memory b)



LlamaFactory.sol#1314
Severity: Low
1314     function toCase(string memory subject, bool toUpper)



LlamaFactory.sol#1355
Severity: Low
1355     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaFactory.sol#1389
Severity: Low
1389     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaFactory.sol#1438
Severity: Low
1438     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaFactory.sol#1446
Severity: Low
1446     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaFactory.sol#1465
Severity: Low
1465     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaFactory.sol#1483
Severity: Low
1483     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaFactory.sol#1506
Severity: Low
1506     function unpackTwo(bytes32 packed)



LlamaFactory.sol#1742
Severity: Low
1742     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaFactory.sol#1765
Severity: Low
1765     function sqrt(uint256 x) internal pure returns (uint256 z) {



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#99
Severity: Low
99     function clone(address implementation) internal returns (address instance) {



LlamaGovernanceScript.sol#121
Severity: Low
121     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaGovernanceScript.sol#139
Severity: Low
139     function predictDeterministicAddress(



LlamaGovernanceScript.sol#491
Severity: Low
491     function toString(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#572
Severity: Low
572     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaGovernanceScript.sol#671
Severity: Low
671     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#745
Severity: Low
745     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#795
Severity: Low
795     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#824
Severity: Low
824     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaGovernanceScript.sol#842
Severity: Low
842     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaGovernanceScript.sol#874
Severity: Low
874     function replace(string memory subject, string memory search, string memory replacement)



LlamaGovernanceScript.sol#951
Severity: Low
951     function indexOf(string memory subject, string memory search, uint256 from)



LlamaGovernanceScript.sol#1020
Severity: Low
1020     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaGovernanceScript.sol#1066
Severity: Low
1066     function startsWith(string memory subject, string memory search)



LlamaGovernanceScript.sol#1087
Severity: Low
1087     function endsWith(string memory subject, string memory search)



LlamaGovernanceScript.sol#1115
Severity: Low
1115     function repeat(string memory subject, uint256 times)



LlamaGovernanceScript.sol#1149
Severity: Low
1149     function slice(string memory subject, uint256 start, uint256 end)



LlamaGovernanceScript.sol#1192
Severity: Low
1192     function indicesOf(string memory subject, string memory search)



LlamaGovernanceScript.sol#1251
Severity: Low
1251     function split(string memory subject, string memory delimiter)



LlamaGovernanceScript.sol#1300
Severity: Low
1300     function concat(string memory a, string memory b)



LlamaGovernanceScript.sol#1338
Severity: Low
1338     function toCase(string memory subject, bool toUpper)



LlamaGovernanceScript.sol#1379
Severity: Low
1379     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaGovernanceScript.sol#1413
Severity: Low
1413     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaGovernanceScript.sol#1462
Severity: Low
1462     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaGovernanceScript.sol#1470
Severity: Low
1470     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaGovernanceScript.sol#1489
Severity: Low
1489     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaGovernanceScript.sol#1507
Severity: Low
1507     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaGovernanceScript.sol#1530
Severity: Low
1530     function unpackTwo(bytes32 packed)



LlamaGovernanceScript.sol#1766
Severity: Low
1766     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaGovernanceScript.sol#1789
Severity: Low
1789     function sqrt(uint256 x) internal pure returns (uint256 z) {



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#27
Severity: Low
27     function toString(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#108
Severity: Low
108     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaPolicy.sol#207
Severity: Low
207     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#281
Severity: Low
281     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaPolicy.sol#331
Severity: Low
331     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaPolicy.sol#360
Severity: Low
360     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaPolicy.sol#378
Severity: Low
378     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaPolicy.sol#410
Severity: Low
410     function replace(string memory subject, string memory search, string memory replacement)



LlamaPolicy.sol#487
Severity: Low
487     function indexOf(string memory subject, string memory search, uint256 from)



LlamaPolicy.sol#556
Severity: Low
556     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaPolicy.sol#602
Severity: Low
602     function startsWith(string memory subject, string memory search)



LlamaPolicy.sol#623
Severity: Low
623     function endsWith(string memory subject, string memory search)



LlamaPolicy.sol#651
Severity: Low
651     function repeat(string memory subject, uint256 times)



LlamaPolicy.sol#685
Severity: Low
685     function slice(string memory subject, uint256 start, uint256 end)



LlamaPolicy.sol#728
Severity: Low
728     function indicesOf(string memory subject, string memory search)



LlamaPolicy.sol#787
Severity: Low
787     function split(string memory subject, string memory delimiter)



LlamaPolicy.sol#836
Severity: Low
836     function concat(string memory a, string memory b)



LlamaPolicy.sol#874
Severity: Low
874     function toCase(string memory subject, bool toUpper)



LlamaPolicy.sol#915
Severity: Low
915     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaPolicy.sol#949
Severity: Low
949     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaPolicy.sol#998
Severity: Low
998     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaPolicy.sol#1006
Severity: Low
1006     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaPolicy.sol#1025
Severity: Low
1025     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaPolicy.sol#1043
Severity: Low
1043     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaPolicy.sol#1066
Severity: Low
1066     function unpackTwo(bytes32 packed)



LlamaPolicy.sol#1327
Severity: Low
1327     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaPolicy.sol#1350
Severity: Low
1350     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaPolicy.sol#1811
Severity: Low
1811     function clone(address implementation) internal returns (address instance) {



LlamaPolicy.sol#1833
Severity: Low
1833     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaPolicy.sol#1851
Severity: Low
1851     function predictDeterministicAddress(



```

### LlamaPolicyMetadata.sol

```

LlamaPolicyMetadata.sol#115
Severity: Low
115     function toString(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#196
Severity: Low
196     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaPolicyMetadata.sol#295
Severity: Low
295     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#369
Severity: Low
369     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#419
Severity: Low
419     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#448
Severity: Low
448     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaPolicyMetadata.sol#466
Severity: Low
466     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaPolicyMetadata.sol#498
Severity: Low
498     function replace(string memory subject, string memory search, string memory replacement)



LlamaPolicyMetadata.sol#575
Severity: Low
575     function indexOf(string memory subject, string memory search, uint256 from)



LlamaPolicyMetadata.sol#644
Severity: Low
644     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaPolicyMetadata.sol#690
Severity: Low
690     function startsWith(string memory subject, string memory search)



LlamaPolicyMetadata.sol#711
Severity: Low
711     function endsWith(string memory subject, string memory search)



LlamaPolicyMetadata.sol#739
Severity: Low
739     function repeat(string memory subject, uint256 times)



LlamaPolicyMetadata.sol#773
Severity: Low
773     function slice(string memory subject, uint256 start, uint256 end)



LlamaPolicyMetadata.sol#816
Severity: Low
816     function indicesOf(string memory subject, string memory search)



LlamaPolicyMetadata.sol#875
Severity: Low
875     function split(string memory subject, string memory delimiter)



LlamaPolicyMetadata.sol#924
Severity: Low
924     function concat(string memory a, string memory b)



LlamaPolicyMetadata.sol#962
Severity: Low
962     function toCase(string memory subject, bool toUpper)



LlamaPolicyMetadata.sol#1003
Severity: Low
1003     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaPolicyMetadata.sol#1037
Severity: Low
1037     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaPolicyMetadata.sol#1086
Severity: Low
1086     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaPolicyMetadata.sol#1094
Severity: Low
1094     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaPolicyMetadata.sol#1113
Severity: Low
1113     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaPolicyMetadata.sol#1131
Severity: Low
1131     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaPolicyMetadata.sol#1154
Severity: Low
1154     function unpackTwo(bytes32 packed)



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#219
Severity: Low
219     function mulDivDown(



LlamaRelativeQuorum.sol#236
Severity: Low
236     function mulDivUp(



LlamaRelativeQuorum.sol#254
Severity: Low
254     function rpow(



LlamaRelativeQuorum.sol#347
Severity: Low
347     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#412
Severity: Low
412     function unsafeMod(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#421
Severity: Low
421     function unsafeDiv(uint256 x, uint256 y) internal pure returns (uint256 r) {



LlamaRelativeQuorum.sol#430
Severity: Low
430     function unsafeDivUp(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#514
Severity: Low
514     function clone(address implementation) internal returns (address instance) {



LlamaRelativeQuorum.sol#536
Severity: Low
536     function cloneDeterministic(address implementation, bytes32 salt) internal returns (address instance) {



LlamaRelativeQuorum.sol#554
Severity: Low
554     function predictDeterministicAddress(



LlamaRelativeQuorum.sol#723
Severity: Low
723     function toString(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#804
Severity: Low
804     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaRelativeQuorum.sol#903
Severity: Low
903     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#977
Severity: Low
977     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#1027
Severity: Low
1027     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#1056
Severity: Low
1056     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaRelativeQuorum.sol#1074
Severity: Low
1074     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaRelativeQuorum.sol#1106
Severity: Low
1106     function replace(string memory subject, string memory search, string memory replacement)



LlamaRelativeQuorum.sol#1183
Severity: Low
1183     function indexOf(string memory subject, string memory search, uint256 from)



LlamaRelativeQuorum.sol#1252
Severity: Low
1252     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaRelativeQuorum.sol#1298
Severity: Low
1298     function startsWith(string memory subject, string memory search)



LlamaRelativeQuorum.sol#1319
Severity: Low
1319     function endsWith(string memory subject, string memory search)



LlamaRelativeQuorum.sol#1347
Severity: Low
1347     function repeat(string memory subject, uint256 times)



LlamaRelativeQuorum.sol#1381
Severity: Low
1381     function slice(string memory subject, uint256 start, uint256 end)



LlamaRelativeQuorum.sol#1424
Severity: Low
1424     function indicesOf(string memory subject, string memory search)



LlamaRelativeQuorum.sol#1483
Severity: Low
1483     function split(string memory subject, string memory delimiter)



LlamaRelativeQuorum.sol#1532
Severity: Low
1532     function concat(string memory a, string memory b)



LlamaRelativeQuorum.sol#1570
Severity: Low
1570     function toCase(string memory subject, bool toUpper)



LlamaRelativeQuorum.sol#1611
Severity: Low
1611     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaRelativeQuorum.sol#1645
Severity: Low
1645     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaRelativeQuorum.sol#1694
Severity: Low
1694     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaRelativeQuorum.sol#1702
Severity: Low
1702     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaRelativeQuorum.sol#1721
Severity: Low
1721     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaRelativeQuorum.sol#1739
Severity: Low
1739     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaRelativeQuorum.sol#1762
Severity: Low
1762     function unpackTwo(bytes32 packed)



LlamaRelativeQuorum.sol#1998
Severity: Low
1998     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaRelativeQuorum.sol#2021
Severity: Low
2021     function sqrt(uint256 x) internal pure returns (uint256 z) {



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


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#4410
Severity: Medium
4410     for (uint256 i = 0; i < strategyConfig.forceApprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsolutePeerReview.sol#4418
Severity: Medium
4418     for (uint256 i = 0; i < strategyConfig.forceDisapprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsolutePeerReview.sol#1963
Severity: Low
1963         while (low < high) {



LlamaAbsolutePeerReview.sol#1987
Severity: Low
1987         while (low < high) {



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#4410
Severity: Medium
4410     for (uint256 i = 0; i < strategyConfig.forceApprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsoluteQuorum.sol#4418
Severity: Medium
4418     for (uint256 i = 0; i < strategyConfig.forceDisapprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsoluteQuorum.sol#1963
Severity: Low
1963         while (low < high) {



LlamaAbsoluteQuorum.sol#1987
Severity: Low
1987         while (low < high) {



```

### LlamaAccount.sol

```

LlamaAccount.sol#2523
Severity: Low
2523         while (low < high) {



LlamaAccount.sol#2547
Severity: Low
2547         while (low < high) {



```

### LlamaCore.sol

```

LlamaCore.sol#1585
Severity: Low
1585         while (low < high) {



LlamaCore.sol#1609
Severity: Low
1609         while (low < high) {



```

### LlamaFactory.sol

```

LlamaFactory.sol#1707
Severity: Low
1707         while (low < high) {



LlamaFactory.sol#1731
Severity: Low
1731         while (low < high) {



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#4074
Severity: Medium
4074     for (uint256 i = 0; i < length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaGovernanceScript.sol#1731
Severity: Low
1731         while (low < high) {



LlamaGovernanceScript.sol#1755
Severity: Low
1755         while (low < high) {



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1292
Severity: Low
1292         while (low < high) {



LlamaPolicy.sol#1316
Severity: Low
1316         while (low < high) {



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#4410
Severity: Medium
4410     for (uint256 i = 0; i < strategyConfig.forceApprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaRelativeQuorum.sol#4418
Severity: Medium
4418     for (uint256 i = 0; i < strategyConfig.forceDisapprovalRoles.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaRelativeQuorum.sol#1963
Severity: Low
1963         while (low < high) {



LlamaRelativeQuorum.sol#1987
Severity: Low
1987         while (low < high) {



```

## SOLIDITY_PRIVATE_MODIFIER_DONT_HIDE_DATA
Contrary to a popular misconception, the ```private``` modifier does not make a variable invisible. Miners have access to all contractsâ€™ code and data. Developers must account for the lack of privacy in Ethereum.

[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#privacy)

Privacy.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#60
Severity: Low
60     uint8 private _initialized;



LlamaAbsolutePeerReview.sol#65
Severity: Low
65     bool private _initializing;



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#60
Severity: Low
60     uint8 private _initialized;



LlamaAbsoluteQuorum.sol#65
Severity: Low
65     bool private _initializing;



```

### LlamaAccount.sol

```

LlamaAccount.sol#60
Severity: Low
60     uint8 private _initialized;



LlamaAccount.sol#65
Severity: Low
65     bool private _initializing;



```

### LlamaCore.sol

```

LlamaCore.sol#153
Severity: Low
153     uint8 private _initialized;



LlamaCore.sol#158
Severity: Low
158     bool private _initializing;



```

### LlamaFactory.sol

```

LlamaFactory.sol#220
Severity: Low
220     uint8 private _initialized;



LlamaFactory.sol#225
Severity: Low
225     bool private _initializing;



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#224
Severity: Low
224     uint8 private _initialized;



LlamaGovernanceScript.sol#229
Severity: Low
229     bool private _initializing;



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1473
Severity: Low
1473     uint8 private _initialized;



LlamaPolicy.sol#1478
Severity: Low
1478     bool private _initializing;



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#60
Severity: Low
60     uint8 private _initialized;



LlamaRelativeQuorum.sol#65
Severity: Low
65     bool private _initializing;



```

## SOLIDITY_SHOULD_NOT_BE_PURE
In Solidity, function that do not read from the state or modify it can be declared as ```pure```.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#219
Severity: Low
219     function mulDivDown(



LlamaAbsolutePeerReview.sol#236
Severity: Low
236     function mulDivUp(



LlamaAbsolutePeerReview.sol#254
Severity: Low
254     function rpow(



LlamaAbsolutePeerReview.sol#347
Severity: Low
347     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#412
Severity: Low
412     function unsafeMod(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#421
Severity: Low
421     function unsafeDiv(uint256 x, uint256 y) internal pure returns (uint256 r) {



LlamaAbsolutePeerReview.sol#430
Severity: Low
430     function unsafeDivUp(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#554
Severity: Low
554     function predictDeterministicAddress(



LlamaAbsolutePeerReview.sol#723
Severity: Low
723     function toString(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#761
Severity: Low
761     function toString(int256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#788
Severity: Low
788     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#804
Severity: Low
804     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaAbsolutePeerReview.sol#858
Severity: Low
858     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#873
Severity: Low
873     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#888
Severity: Low
888     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#903
Severity: Low
903     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#943
Severity: Low
943     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#964
Severity: Low
964     function toHexString(address value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#977
Severity: Low
977     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#1014
Severity: Low
1014     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#1027
Severity: Low
1027     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaAbsolutePeerReview.sol#1056
Severity: Low
1056     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaAbsolutePeerReview.sol#1074
Severity: Low
1074     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaAbsolutePeerReview.sol#1106
Severity: Low
1106     function replace(string memory subject, string memory search, string memory replacement)



LlamaAbsolutePeerReview.sol#1183
Severity: Low
1183     function indexOf(string memory subject, string memory search, uint256 from)



LlamaAbsolutePeerReview.sol#1252
Severity: Low
1252     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaAbsolutePeerReview.sol#1298
Severity: Low
1298     function startsWith(string memory subject, string memory search)



LlamaAbsolutePeerReview.sol#1319
Severity: Low
1319     function endsWith(string memory subject, string memory search)



LlamaAbsolutePeerReview.sol#1347
Severity: Low
1347     function repeat(string memory subject, uint256 times)



LlamaAbsolutePeerReview.sol#1381
Severity: Low
1381     function slice(string memory subject, uint256 start, uint256 end)



LlamaAbsolutePeerReview.sol#1424
Severity: Low
1424     function indicesOf(string memory subject, string memory search)



LlamaAbsolutePeerReview.sol#1483
Severity: Low
1483     function split(string memory subject, string memory delimiter)



LlamaAbsolutePeerReview.sol#1532
Severity: Low
1532     function concat(string memory a, string memory b)



LlamaAbsolutePeerReview.sol#1570
Severity: Low
1570     function toCase(string memory subject, bool toUpper)



LlamaAbsolutePeerReview.sol#1611
Severity: Low
1611     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaAbsolutePeerReview.sol#1645
Severity: Low
1645     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaAbsolutePeerReview.sol#1694
Severity: Low
1694     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaAbsolutePeerReview.sol#1702
Severity: Low
1702     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaAbsolutePeerReview.sol#1721
Severity: Low
1721     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaAbsolutePeerReview.sol#1739
Severity: Low
1739     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaAbsolutePeerReview.sol#1762
Severity: Low
1762     function unpackTwo(bytes32 packed)



LlamaAbsolutePeerReview.sol#1787
Severity: Low
1787     function directReturn(string memory a) internal pure {



LlamaAbsolutePeerReview.sol#1998
Severity: Low
1998     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaAbsolutePeerReview.sol#2021
Severity: Low
2021     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAbsolutePeerReview.sol#2811
Severity: Low
2811     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#219
Severity: Low
219     function mulDivDown(



LlamaAbsoluteQuorum.sol#236
Severity: Low
236     function mulDivUp(



LlamaAbsoluteQuorum.sol#254
Severity: Low
254     function rpow(



LlamaAbsoluteQuorum.sol#347
Severity: Low
347     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#412
Severity: Low
412     function unsafeMod(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#421
Severity: Low
421     function unsafeDiv(uint256 x, uint256 y) internal pure returns (uint256 r) {



LlamaAbsoluteQuorum.sol#430
Severity: Low
430     function unsafeDivUp(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#554
Severity: Low
554     function predictDeterministicAddress(



LlamaAbsoluteQuorum.sol#723
Severity: Low
723     function toString(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#761
Severity: Low
761     function toString(int256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#788
Severity: Low
788     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#804
Severity: Low
804     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaAbsoluteQuorum.sol#858
Severity: Low
858     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#873
Severity: Low
873     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#888
Severity: Low
888     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#903
Severity: Low
903     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#943
Severity: Low
943     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#964
Severity: Low
964     function toHexString(address value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#977
Severity: Low
977     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#1014
Severity: Low
1014     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#1027
Severity: Low
1027     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaAbsoluteQuorum.sol#1056
Severity: Low
1056     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaAbsoluteQuorum.sol#1074
Severity: Low
1074     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaAbsoluteQuorum.sol#1106
Severity: Low
1106     function replace(string memory subject, string memory search, string memory replacement)



LlamaAbsoluteQuorum.sol#1183
Severity: Low
1183     function indexOf(string memory subject, string memory search, uint256 from)



LlamaAbsoluteQuorum.sol#1252
Severity: Low
1252     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaAbsoluteQuorum.sol#1298
Severity: Low
1298     function startsWith(string memory subject, string memory search)



LlamaAbsoluteQuorum.sol#1319
Severity: Low
1319     function endsWith(string memory subject, string memory search)



LlamaAbsoluteQuorum.sol#1347
Severity: Low
1347     function repeat(string memory subject, uint256 times)



LlamaAbsoluteQuorum.sol#1381
Severity: Low
1381     function slice(string memory subject, uint256 start, uint256 end)



LlamaAbsoluteQuorum.sol#1424
Severity: Low
1424     function indicesOf(string memory subject, string memory search)



LlamaAbsoluteQuorum.sol#1483
Severity: Low
1483     function split(string memory subject, string memory delimiter)



LlamaAbsoluteQuorum.sol#1532
Severity: Low
1532     function concat(string memory a, string memory b)



LlamaAbsoluteQuorum.sol#1570
Severity: Low
1570     function toCase(string memory subject, bool toUpper)



LlamaAbsoluteQuorum.sol#1611
Severity: Low
1611     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaAbsoluteQuorum.sol#1645
Severity: Low
1645     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaAbsoluteQuorum.sol#1694
Severity: Low
1694     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaAbsoluteQuorum.sol#1702
Severity: Low
1702     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaAbsoluteQuorum.sol#1721
Severity: Low
1721     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaAbsoluteQuorum.sol#1739
Severity: Low
1739     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaAbsoluteQuorum.sol#1762
Severity: Low
1762     function unpackTwo(bytes32 packed)



LlamaAbsoluteQuorum.sol#1787
Severity: Low
1787     function directReturn(string memory a) internal pure {



LlamaAbsoluteQuorum.sol#1998
Severity: Low
1998     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaAbsoluteQuorum.sol#2021
Severity: Low
2021     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAbsoluteQuorum.sol#2811
Severity: Low
2811     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaAccount.sol

```

LlamaAccount.sol#1231
Severity: Low
1231     function predictDeterministicAddress(



LlamaAccount.sol#1283
Severity: Low
1283     function toString(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1321
Severity: Low
1321     function toString(int256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1348
Severity: Low
1348     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaAccount.sol#1364
Severity: Low
1364     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaAccount.sol#1418
Severity: Low
1418     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1433
Severity: Low
1433     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1448
Severity: Low
1448     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1463
Severity: Low
1463     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaAccount.sol#1503
Severity: Low
1503     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaAccount.sol#1524
Severity: Low
1524     function toHexString(address value) internal pure returns (string memory str) {



LlamaAccount.sol#1537
Severity: Low
1537     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaAccount.sol#1574
Severity: Low
1574     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaAccount.sol#1587
Severity: Low
1587     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaAccount.sol#1616
Severity: Low
1616     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaAccount.sol#1634
Severity: Low
1634     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaAccount.sol#1666
Severity: Low
1666     function replace(string memory subject, string memory search, string memory replacement)



LlamaAccount.sol#1743
Severity: Low
1743     function indexOf(string memory subject, string memory search, uint256 from)



LlamaAccount.sol#1812
Severity: Low
1812     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaAccount.sol#1858
Severity: Low
1858     function startsWith(string memory subject, string memory search)



LlamaAccount.sol#1879
Severity: Low
1879     function endsWith(string memory subject, string memory search)



LlamaAccount.sol#1907
Severity: Low
1907     function repeat(string memory subject, uint256 times)



LlamaAccount.sol#1941
Severity: Low
1941     function slice(string memory subject, uint256 start, uint256 end)



LlamaAccount.sol#1984
Severity: Low
1984     function indicesOf(string memory subject, string memory search)



LlamaAccount.sol#2043
Severity: Low
2043     function split(string memory subject, string memory delimiter)



LlamaAccount.sol#2092
Severity: Low
2092     function concat(string memory a, string memory b)



LlamaAccount.sol#2130
Severity: Low
2130     function toCase(string memory subject, bool toUpper)



LlamaAccount.sol#2171
Severity: Low
2171     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaAccount.sol#2205
Severity: Low
2205     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaAccount.sol#2254
Severity: Low
2254     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaAccount.sol#2262
Severity: Low
2262     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaAccount.sol#2281
Severity: Low
2281     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaAccount.sol#2299
Severity: Low
2299     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaAccount.sol#2322
Severity: Low
2322     function unpackTwo(bytes32 packed)



LlamaAccount.sol#2347
Severity: Low
2347     function directReturn(string memory a) internal pure {



LlamaAccount.sol#2558
Severity: Low
2558     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaAccount.sol#2581
Severity: Low
2581     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaAccount.sol#2886
Severity: Low
2886     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaCore.sol

```

LlamaCore.sol#68
Severity: Low
68     function predictDeterministicAddress(



LlamaCore.sol#320
Severity: Low
320     function toString(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#358
Severity: Low
358     function toString(int256 value) internal pure returns (string memory str) {



LlamaCore.sol#385
Severity: Low
385     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaCore.sol#401
Severity: Low
401     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaCore.sol#455
Severity: Low
455     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#470
Severity: Low
470     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#485
Severity: Low
485     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#500
Severity: Low
500     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaCore.sol#540
Severity: Low
540     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaCore.sol#561
Severity: Low
561     function toHexString(address value) internal pure returns (string memory str) {



LlamaCore.sol#574
Severity: Low
574     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaCore.sol#611
Severity: Low
611     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaCore.sol#624
Severity: Low
624     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaCore.sol#653
Severity: Low
653     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaCore.sol#671
Severity: Low
671     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaCore.sol#703
Severity: Low
703     function replace(string memory subject, string memory search, string memory replacement)



LlamaCore.sol#780
Severity: Low
780     function indexOf(string memory subject, string memory search, uint256 from)



LlamaCore.sol#849
Severity: Low
849     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaCore.sol#895
Severity: Low
895     function startsWith(string memory subject, string memory search)



LlamaCore.sol#916
Severity: Low
916     function endsWith(string memory subject, string memory search)



LlamaCore.sol#944
Severity: Low
944     function repeat(string memory subject, uint256 times)



LlamaCore.sol#978
Severity: Low
978     function slice(string memory subject, uint256 start, uint256 end)



LlamaCore.sol#1021
Severity: Low
1021     function indicesOf(string memory subject, string memory search)



LlamaCore.sol#1080
Severity: Low
1080     function split(string memory subject, string memory delimiter)



LlamaCore.sol#1129
Severity: Low
1129     function concat(string memory a, string memory b)



LlamaCore.sol#1167
Severity: Low
1167     function toCase(string memory subject, bool toUpper)



LlamaCore.sol#1208
Severity: Low
1208     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaCore.sol#1242
Severity: Low
1242     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaCore.sol#1291
Severity: Low
1291     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaCore.sol#1299
Severity: Low
1299     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaCore.sol#1318
Severity: Low
1318     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaCore.sol#1336
Severity: Low
1336     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaCore.sol#1359
Severity: Low
1359     function unpackTwo(bytes32 packed)



LlamaCore.sol#1384
Severity: Low
1384     function directReturn(string memory a) internal pure {



LlamaCore.sol#1620
Severity: Low
1620     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaCore.sol#1643
Severity: Low
1643     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaCore.sol#1948
Severity: Low
1948     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaFactory.sol

```

LlamaFactory.sol#68
Severity: Low
68     function predictDeterministicAddress(



LlamaFactory.sol#467
Severity: Low
467     function toString(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#505
Severity: Low
505     function toString(int256 value) internal pure returns (string memory str) {



LlamaFactory.sol#532
Severity: Low
532     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaFactory.sol#548
Severity: Low
548     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaFactory.sol#602
Severity: Low
602     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#617
Severity: Low
617     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#632
Severity: Low
632     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#647
Severity: Low
647     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaFactory.sol#687
Severity: Low
687     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaFactory.sol#708
Severity: Low
708     function toHexString(address value) internal pure returns (string memory str) {



LlamaFactory.sol#721
Severity: Low
721     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaFactory.sol#758
Severity: Low
758     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaFactory.sol#771
Severity: Low
771     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaFactory.sol#800
Severity: Low
800     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaFactory.sol#818
Severity: Low
818     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaFactory.sol#850
Severity: Low
850     function replace(string memory subject, string memory search, string memory replacement)



LlamaFactory.sol#927
Severity: Low
927     function indexOf(string memory subject, string memory search, uint256 from)



LlamaFactory.sol#996
Severity: Low
996     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaFactory.sol#1042
Severity: Low
1042     function startsWith(string memory subject, string memory search)



LlamaFactory.sol#1063
Severity: Low
1063     function endsWith(string memory subject, string memory search)



LlamaFactory.sol#1091
Severity: Low
1091     function repeat(string memory subject, uint256 times)



LlamaFactory.sol#1125
Severity: Low
1125     function slice(string memory subject, uint256 start, uint256 end)



LlamaFactory.sol#1168
Severity: Low
1168     function indicesOf(string memory subject, string memory search)



LlamaFactory.sol#1227
Severity: Low
1227     function split(string memory subject, string memory delimiter)



LlamaFactory.sol#1276
Severity: Low
1276     function concat(string memory a, string memory b)



LlamaFactory.sol#1314
Severity: Low
1314     function toCase(string memory subject, bool toUpper)



LlamaFactory.sol#1355
Severity: Low
1355     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaFactory.sol#1389
Severity: Low
1389     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaFactory.sol#1438
Severity: Low
1438     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaFactory.sol#1446
Severity: Low
1446     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaFactory.sol#1465
Severity: Low
1465     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaFactory.sol#1483
Severity: Low
1483     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaFactory.sol#1506
Severity: Low
1506     function unpackTwo(bytes32 packed)



LlamaFactory.sol#1531
Severity: Low
1531     function directReturn(string memory a) internal pure {



LlamaFactory.sol#1742
Severity: Low
1742     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaFactory.sol#1765
Severity: Low
1765     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaFactory.sol#3448
Severity: Low
3448     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#139
Severity: Low
139     function predictDeterministicAddress(



LlamaGovernanceScript.sol#491
Severity: Low
491     function toString(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#529
Severity: Low
529     function toString(int256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#556
Severity: Low
556     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#572
Severity: Low
572     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaGovernanceScript.sol#626
Severity: Low
626     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#641
Severity: Low
641     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#656
Severity: Low
656     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#671
Severity: Low
671     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#711
Severity: Low
711     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#732
Severity: Low
732     function toHexString(address value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#745
Severity: Low
745     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#782
Severity: Low
782     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#795
Severity: Low
795     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaGovernanceScript.sol#824
Severity: Low
824     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaGovernanceScript.sol#842
Severity: Low
842     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaGovernanceScript.sol#874
Severity: Low
874     function replace(string memory subject, string memory search, string memory replacement)



LlamaGovernanceScript.sol#951
Severity: Low
951     function indexOf(string memory subject, string memory search, uint256 from)



LlamaGovernanceScript.sol#1020
Severity: Low
1020     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaGovernanceScript.sol#1066
Severity: Low
1066     function startsWith(string memory subject, string memory search)



LlamaGovernanceScript.sol#1087
Severity: Low
1087     function endsWith(string memory subject, string memory search)



LlamaGovernanceScript.sol#1115
Severity: Low
1115     function repeat(string memory subject, uint256 times)



LlamaGovernanceScript.sol#1149
Severity: Low
1149     function slice(string memory subject, uint256 start, uint256 end)



LlamaGovernanceScript.sol#1192
Severity: Low
1192     function indicesOf(string memory subject, string memory search)



LlamaGovernanceScript.sol#1251
Severity: Low
1251     function split(string memory subject, string memory delimiter)



LlamaGovernanceScript.sol#1300
Severity: Low
1300     function concat(string memory a, string memory b)



LlamaGovernanceScript.sol#1338
Severity: Low
1338     function toCase(string memory subject, bool toUpper)



LlamaGovernanceScript.sol#1379
Severity: Low
1379     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaGovernanceScript.sol#1413
Severity: Low
1413     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaGovernanceScript.sol#1462
Severity: Low
1462     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaGovernanceScript.sol#1470
Severity: Low
1470     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaGovernanceScript.sol#1489
Severity: Low
1489     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaGovernanceScript.sol#1507
Severity: Low
1507     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaGovernanceScript.sol#1530
Severity: Low
1530     function unpackTwo(bytes32 packed)



LlamaGovernanceScript.sol#1555
Severity: Low
1555     function directReturn(string memory a) internal pure {



LlamaGovernanceScript.sol#1766
Severity: Low
1766     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaGovernanceScript.sol#1789
Severity: Low
1789     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaGovernanceScript.sol#2579
Severity: Low
2579     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#27
Severity: Low
27     function toString(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#65
Severity: Low
65     function toString(int256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#92
Severity: Low
92     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaPolicy.sol#108
Severity: Low
108     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaPolicy.sol#162
Severity: Low
162     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#177
Severity: Low
177     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#192
Severity: Low
192     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#207
Severity: Low
207     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaPolicy.sol#247
Severity: Low
247     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaPolicy.sol#268
Severity: Low
268     function toHexString(address value) internal pure returns (string memory str) {



LlamaPolicy.sol#281
Severity: Low
281     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaPolicy.sol#318
Severity: Low
318     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaPolicy.sol#331
Severity: Low
331     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaPolicy.sol#360
Severity: Low
360     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaPolicy.sol#378
Severity: Low
378     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaPolicy.sol#410
Severity: Low
410     function replace(string memory subject, string memory search, string memory replacement)



LlamaPolicy.sol#487
Severity: Low
487     function indexOf(string memory subject, string memory search, uint256 from)



LlamaPolicy.sol#556
Severity: Low
556     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaPolicy.sol#602
Severity: Low
602     function startsWith(string memory subject, string memory search)



LlamaPolicy.sol#623
Severity: Low
623     function endsWith(string memory subject, string memory search)



LlamaPolicy.sol#651
Severity: Low
651     function repeat(string memory subject, uint256 times)



LlamaPolicy.sol#685
Severity: Low
685     function slice(string memory subject, uint256 start, uint256 end)



LlamaPolicy.sol#728
Severity: Low
728     function indicesOf(string memory subject, string memory search)



LlamaPolicy.sol#787
Severity: Low
787     function split(string memory subject, string memory delimiter)



LlamaPolicy.sol#836
Severity: Low
836     function concat(string memory a, string memory b)



LlamaPolicy.sol#874
Severity: Low
874     function toCase(string memory subject, bool toUpper)



LlamaPolicy.sol#915
Severity: Low
915     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaPolicy.sol#949
Severity: Low
949     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaPolicy.sol#998
Severity: Low
998     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaPolicy.sol#1006
Severity: Low
1006     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaPolicy.sol#1025
Severity: Low
1025     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaPolicy.sol#1043
Severity: Low
1043     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaPolicy.sol#1066
Severity: Low
1066     function unpackTwo(bytes32 packed)



LlamaPolicy.sol#1091
Severity: Low
1091     function directReturn(string memory a) internal pure {



LlamaPolicy.sol#1327
Severity: Low
1327     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaPolicy.sol#1350
Severity: Low
1350     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaPolicy.sol#1851
Severity: Low
1851     function predictDeterministicAddress(



LlamaPolicy.sol#1986
Severity: Low
1986     function encode(bytes memory data) internal pure returns (string memory) {



```

### LlamaPolicyMetadata.sol

```

LlamaPolicyMetadata.sol#18
Severity: Low
18     function encode(bytes memory data) internal pure returns (string memory) {



LlamaPolicyMetadata.sol#115
Severity: Low
115     function toString(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#153
Severity: Low
153     function toString(int256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#180
Severity: Low
180     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#196
Severity: Low
196     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaPolicyMetadata.sol#250
Severity: Low
250     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#265
Severity: Low
265     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#280
Severity: Low
280     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#295
Severity: Low
295     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#335
Severity: Low
335     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#356
Severity: Low
356     function toHexString(address value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#369
Severity: Low
369     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#406
Severity: Low
406     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#419
Severity: Low
419     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaPolicyMetadata.sol#448
Severity: Low
448     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaPolicyMetadata.sol#466
Severity: Low
466     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaPolicyMetadata.sol#498
Severity: Low
498     function replace(string memory subject, string memory search, string memory replacement)



LlamaPolicyMetadata.sol#575
Severity: Low
575     function indexOf(string memory subject, string memory search, uint256 from)



LlamaPolicyMetadata.sol#644
Severity: Low
644     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaPolicyMetadata.sol#690
Severity: Low
690     function startsWith(string memory subject, string memory search)



LlamaPolicyMetadata.sol#711
Severity: Low
711     function endsWith(string memory subject, string memory search)



LlamaPolicyMetadata.sol#739
Severity: Low
739     function repeat(string memory subject, uint256 times)



LlamaPolicyMetadata.sol#773
Severity: Low
773     function slice(string memory subject, uint256 start, uint256 end)



LlamaPolicyMetadata.sol#816
Severity: Low
816     function indicesOf(string memory subject, string memory search)



LlamaPolicyMetadata.sol#875
Severity: Low
875     function split(string memory subject, string memory delimiter)



LlamaPolicyMetadata.sol#924
Severity: Low
924     function concat(string memory a, string memory b)



LlamaPolicyMetadata.sol#962
Severity: Low
962     function toCase(string memory subject, bool toUpper)



LlamaPolicyMetadata.sol#1003
Severity: Low
1003     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaPolicyMetadata.sol#1037
Severity: Low
1037     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaPolicyMetadata.sol#1086
Severity: Low
1086     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaPolicyMetadata.sol#1094
Severity: Low
1094     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaPolicyMetadata.sol#1113
Severity: Low
1113     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaPolicyMetadata.sol#1131
Severity: Low
1131     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaPolicyMetadata.sol#1154
Severity: Low
1154     function unpackTwo(bytes32 packed)



LlamaPolicyMetadata.sol#1179
Severity: Low
1179     function directReturn(string memory a) internal pure {



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#219
Severity: Low
219     function mulDivDown(



LlamaRelativeQuorum.sol#236
Severity: Low
236     function mulDivUp(



LlamaRelativeQuorum.sol#254
Severity: Low
254     function rpow(



LlamaRelativeQuorum.sol#347
Severity: Low
347     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#412
Severity: Low
412     function unsafeMod(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#421
Severity: Low
421     function unsafeDiv(uint256 x, uint256 y) internal pure returns (uint256 r) {



LlamaRelativeQuorum.sol#430
Severity: Low
430     function unsafeDivUp(uint256 x, uint256 y) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#554
Severity: Low
554     function predictDeterministicAddress(



LlamaRelativeQuorum.sol#723
Severity: Low
723     function toString(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#761
Severity: Low
761     function toString(int256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#788
Severity: Low
788     function toHexString(uint256 value, uint256 length) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#804
Severity: Low
804     function toHexStringNoPrefix(uint256 value, uint256 length)



LlamaRelativeQuorum.sol#858
Severity: Low
858     function toHexString(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#873
Severity: Low
873     function toMinimalHexString(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#888
Severity: Low
888     function toMinimalHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#903
Severity: Low
903     function toHexStringNoPrefix(uint256 value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#943
Severity: Low
943     function toHexStringChecksummed(address value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#964
Severity: Low
964     function toHexString(address value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#977
Severity: Low
977     function toHexStringNoPrefix(address value) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#1014
Severity: Low
1014     function toHexString(bytes memory raw) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#1027
Severity: Low
1027     function toHexStringNoPrefix(bytes memory raw) internal pure returns (string memory str) {



LlamaRelativeQuorum.sol#1056
Severity: Low
1056     function runeCount(string memory s) internal pure returns (uint256 result) {



LlamaRelativeQuorum.sol#1074
Severity: Low
1074     function is7BitASCII(string memory s) internal pure returns (bool result) {



LlamaRelativeQuorum.sol#1106
Severity: Low
1106     function replace(string memory subject, string memory search, string memory replacement)



LlamaRelativeQuorum.sol#1183
Severity: Low
1183     function indexOf(string memory subject, string memory search, uint256 from)



LlamaRelativeQuorum.sol#1252
Severity: Low
1252     function lastIndexOf(string memory subject, string memory search, uint256 from)



LlamaRelativeQuorum.sol#1298
Severity: Low
1298     function startsWith(string memory subject, string memory search)



LlamaRelativeQuorum.sol#1319
Severity: Low
1319     function endsWith(string memory subject, string memory search)



LlamaRelativeQuorum.sol#1347
Severity: Low
1347     function repeat(string memory subject, uint256 times)



LlamaRelativeQuorum.sol#1381
Severity: Low
1381     function slice(string memory subject, uint256 start, uint256 end)



LlamaRelativeQuorum.sol#1424
Severity: Low
1424     function indicesOf(string memory subject, string memory search)



LlamaRelativeQuorum.sol#1483
Severity: Low
1483     function split(string memory subject, string memory delimiter)



LlamaRelativeQuorum.sol#1532
Severity: Low
1532     function concat(string memory a, string memory b)



LlamaRelativeQuorum.sol#1570
Severity: Low
1570     function toCase(string memory subject, bool toUpper)



LlamaRelativeQuorum.sol#1611
Severity: Low
1611     function escapeHTML(string memory s) internal pure returns (string memory result) {



LlamaRelativeQuorum.sol#1645
Severity: Low
1645     function escapeJSON(string memory s) internal pure returns (string memory result) {



LlamaRelativeQuorum.sol#1694
Severity: Low
1694     function eq(string memory a, string memory b) internal pure returns (bool result) {



LlamaRelativeQuorum.sol#1702
Severity: Low
1702     function packOne(string memory a) internal pure returns (bytes32 result) {



LlamaRelativeQuorum.sol#1721
Severity: Low
1721     function unpackOne(bytes32 packed) internal pure returns (string memory result) {



LlamaRelativeQuorum.sol#1739
Severity: Low
1739     function packTwo(string memory a, string memory b) internal pure returns (bytes32 result) {



LlamaRelativeQuorum.sol#1762
Severity: Low
1762     function unpackTwo(bytes32 packed)



LlamaRelativeQuorum.sol#1787
Severity: Low
1787     function directReturn(string memory a) internal pure {



LlamaRelativeQuorum.sol#1998
Severity: Low
1998     function _unsafeAccess(Checkpoint[] storage self, uint256 pos)



LlamaRelativeQuorum.sol#2021
Severity: Low
2021     function sqrt(uint256 x) internal pure returns (uint256 z) {



LlamaRelativeQuorum.sol#2811
Severity: Low
2811     function encode(bytes memory data) internal pure returns (string memory) {



```

## SOLIDITY_SHOULD_RETURN_STRUCT
Consider using struct instead of multiple return values for ```internal``` or ```private``` functions. It can improve code readability.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#690
Severity: Low
690     returns (bool success, bytes memory result)



LlamaAbsolutePeerReview.sol#1765
Severity: Low
1765         returns (string memory resultA, string memory resultB)



LlamaAbsolutePeerReview.sol#1864
Severity: Low
1864     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaAbsolutePeerReview.sol#1874
Severity: Low
1874     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaAbsolutePeerReview.sol#1893
Severity: Low
1893         returns (



LlamaAbsolutePeerReview.sol#1925
Severity: Low
1925     ) private returns (uint128, uint128) {



LlamaAbsolutePeerReview.sol#3062
Severity: Low
3062   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaAbsolutePeerReview.sol#3232
Severity: Low
3232   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaAbsolutePeerReview.sol#3303
Severity: Low
3303   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#690
Severity: Low
690     returns (bool success, bytes memory result)



LlamaAbsoluteQuorum.sol#1765
Severity: Low
1765         returns (string memory resultA, string memory resultB)



LlamaAbsoluteQuorum.sol#1864
Severity: Low
1864     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaAbsoluteQuorum.sol#1874
Severity: Low
1874     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaAbsoluteQuorum.sol#1893
Severity: Low
1893         returns (



LlamaAbsoluteQuorum.sol#1925
Severity: Low
1925     ) private returns (uint128, uint128) {



LlamaAbsoluteQuorum.sol#3062
Severity: Low
3062   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaAbsoluteQuorum.sol#3232
Severity: Low
3232   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaAbsoluteQuorum.sol#3303
Severity: Low
3303   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaAccount.sol

```

LlamaAccount.sol#2325
Severity: Low
2325         returns (string memory resultA, string memory resultB)



LlamaAccount.sol#2424
Severity: Low
2424     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaAccount.sol#2434
Severity: Low
2434     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaAccount.sol#2453
Severity: Low
2453         returns (



LlamaAccount.sol#2485
Severity: Low
2485     ) private returns (uint128, uint128) {



LlamaAccount.sol#2865
Severity: Low
2865     returns (bool success, bytes memory result)



LlamaAccount.sol#3137
Severity: Low
3137   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaAccount.sol#3307
Severity: Low
3307   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaAccount.sol#3378
Severity: Low
3378   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaCore.sol

```

LlamaCore.sol#1362
Severity: Low
1362         returns (string memory resultA, string memory resultB)



LlamaCore.sol#1486
Severity: Low
1486     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaCore.sol#1496
Severity: Low
1496     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaCore.sol#1515
Severity: Low
1515         returns (



LlamaCore.sol#1547
Severity: Low
1547     ) private returns (uint128, uint128) {



LlamaCore.sol#1927
Severity: Low
1927     returns (bool success, bytes memory result)



LlamaCore.sol#2199
Severity: Low
2199   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaCore.sol#2369
Severity: Low
2369   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaCore.sol#2440
Severity: Low
2440   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaExecutor.sol

```

LlamaExecutor.sol#31
Severity: Low
31     returns (bool success, bytes memory result)



```

### LlamaFactory.sol

```

LlamaFactory.sol#437
Severity: Low
437     returns (bool success, bytes memory result)



LlamaFactory.sol#1509
Severity: Low
1509         returns (string memory resultA, string memory resultB)



LlamaFactory.sol#1608
Severity: Low
1608     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaFactory.sol#1618
Severity: Low
1618     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaFactory.sol#1637
Severity: Low
1637         returns (



LlamaFactory.sol#1669
Severity: Low
1669     ) private returns (uint128, uint128) {



LlamaFactory.sol#3699
Severity: Low
3699   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaFactory.sol#3869
Severity: Low
3869   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaFactory.sol#3940
Severity: Low
3940   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#458
Severity: Low
458     returns (bool success, bytes memory result)



LlamaGovernanceScript.sol#1533
Severity: Low
1533         returns (string memory resultA, string memory resultB)



LlamaGovernanceScript.sol#1632
Severity: Low
1632     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaGovernanceScript.sol#1642
Severity: Low
1642     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaGovernanceScript.sol#1661
Severity: Low
1661         returns (



LlamaGovernanceScript.sol#1693
Severity: Low
1693     ) private returns (uint128, uint128) {



LlamaGovernanceScript.sol#2830
Severity: Low
2830   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaGovernanceScript.sol#3000
Severity: Low
3000   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaGovernanceScript.sol#3071
Severity: Low
3071   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1069
Severity: Low
1069         returns (string memory resultA, string memory resultB)



LlamaPolicy.sol#1193
Severity: Low
1193     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaPolicy.sol#1203
Severity: Low
1203     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaPolicy.sol#1222
Severity: Low
1222         returns (



LlamaPolicy.sol#1254
Severity: Low
1254     ) private returns (uint128, uint128) {



LlamaPolicy.sol#1962
Severity: Low
1962     returns (bool success, bytes memory result)



LlamaPolicy.sol#2237
Severity: Low
2237   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaPolicy.sol#2407
Severity: Low
2407   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaPolicy.sol#2478
Severity: Low
2478   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

### LlamaPolicyMetadata.sol

```

LlamaPolicyMetadata.sol#1157
Severity: Low
1157         returns (string memory resultA, string memory resultB)



```

### LlamaPolicyMetadataParamRegistry.sol

```

LlamaPolicyMetadataParamRegistry.sol#31
Severity: Low
31     returns (bool success, bytes memory result)



LlamaPolicyMetadataParamRegistry.sol#106
Severity: Low
106   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#690
Severity: Low
690     returns (bool success, bytes memory result)



LlamaRelativeQuorum.sol#1765
Severity: Low
1765         returns (string memory resultA, string memory resultB)



LlamaRelativeQuorum.sol#1864
Severity: Low
1864     function push(History storage self, uint256 quantity, uint256 expiration) internal returns (uint128, uint128) {



LlamaRelativeQuorum.sol#1874
Severity: Low
1874     function push(History storage self, uint256 quantity) internal returns (uint128, uint128) {



LlamaRelativeQuorum.sol#1893
Severity: Low
1893         returns (



LlamaRelativeQuorum.sol#1925
Severity: Low
1925     ) private returns (uint128, uint128) {



LlamaRelativeQuorum.sol#3062
Severity: Low
3062   function getMetadata(LlamaExecutor llamaExecutor) external view returns (string memory _color, string memory _logo) {



LlamaRelativeQuorum.sol#3232
Severity: Low
3232   ) external onlyRootLlama returns (LlamaExecutor executor, LlamaCore core) {



LlamaRelativeQuorum.sol#3303
Severity: Low
3303   ) internal returns (LlamaExecutor llamaExecutor, LlamaCore llamaCore) {



```

## SOLIDITY_UNCHECKED_CALL
Expect calls to external contract to fail. When sending ether, check for the return value and handle errors. The recommended way of doing ether transfers is ```transfer```.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#693
Severity: High
693     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#693
Severity: High
693     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaAccount.sol

```

LlamaAccount.sol#586
Severity: High
586         _callOptionalReturn(token, abi.encodeCall(token.transfer, (to, value)));



LlamaAccount.sol#594
Severity: High
594         _callOptionalReturn(token, abi.encodeCall(token.transferFrom, (from, to, value)));



LlamaAccount.sol#686
Severity: High
686         (bool success, bytes memory returndata) = address(token).call(data);



LlamaAccount.sol#2868
Severity: High
2868     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaCore.sol

```

LlamaCore.sol#1930
Severity: High
1930     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaExecutor.sol

```

LlamaExecutor.sol#34
Severity: High
34     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaFactory.sol

```

LlamaFactory.sol#440
Severity: High
440     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#461
Severity: High
461     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



LlamaGovernanceScript.sol#4078
Severity: High
4078       (bool success, bytes memory response) = targets[i].call(data[i]);



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1965
Severity: High
1965     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaPolicyMetadataParamRegistry.sol

```

LlamaPolicyMetadataParamRegistry.sol#34
Severity: High
34     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#693
Severity: High
693     (success, result) = isScript ? target.delegatecall(data) : target.call{value: value}(data);



```

## SOLIDITY_UPGRADE_TO_050
Prepare your code for Solidity 0.5.0 release.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#2192
Severity: Low
2192   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#2192
Severity: Low
2192   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaAccount.sol

```

LlamaAccount.sol#2752
Severity: Low
2752   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaCore.sol

```

LlamaCore.sol#1814
Severity: Low
1814   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaFactory.sol

```

LlamaFactory.sol#1936
Severity: Low
1936   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#1960
Severity: Low
1960   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1704
Severity: Low
1704   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#2192
Severity: Low
2192   function safeTransferFrom(address from, address to, uint256 id, bytes calldata data) public virtual;



```

## SOLIDITY_USING_INLINE_ASSEMBLY
Inline assembly is a way to access the Ethereum Virtual Machine at a low level. This discards several important safety features of Solidity.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#225
Severity: Low
225         assembly {



LlamaAbsolutePeerReview.sol#242
Severity: Low
242         assembly {



LlamaAbsolutePeerReview.sol#260
Severity: Low
260         assembly {



LlamaAbsolutePeerReview.sol#349
Severity: Low
349         assembly {



LlamaAbsolutePeerReview.sol#414
Severity: Low
414         assembly {



LlamaAbsolutePeerReview.sol#423
Severity: Low
423         assembly {



LlamaAbsolutePeerReview.sol#432
Severity: Low
432         assembly {



LlamaAbsolutePeerReview.sol#516
Severity: Low
516         assembly {



LlamaAbsolutePeerReview.sol#538
Severity: Low
538         assembly {



LlamaAbsolutePeerReview.sol#560
Severity: Low
560         assembly {



LlamaAbsolutePeerReview.sol#725
Severity: Low
725         assembly {



LlamaAbsolutePeerReview.sol#769
Severity: Low
769         assembly {



LlamaAbsolutePeerReview.sol#791
Severity: Low
791         assembly {



LlamaAbsolutePeerReview.sol#810
Severity: Low
810         assembly {



LlamaAbsolutePeerReview.sol#861
Severity: Low
861         assembly {



LlamaAbsolutePeerReview.sol#876
Severity: Low
876         assembly {



LlamaAbsolutePeerReview.sol#891
Severity: Low
891         assembly {



LlamaAbsolutePeerReview.sol#905
Severity: Low
905         assembly {



LlamaAbsolutePeerReview.sol#946
Severity: Low
946         assembly {



LlamaAbsolutePeerReview.sol#967
Severity: Low
967         assembly {



LlamaAbsolutePeerReview.sol#979
Severity: Low
979         assembly {



LlamaAbsolutePeerReview.sol#1017
Severity: Low
1017         assembly {



LlamaAbsolutePeerReview.sol#1029
Severity: Low
1029         assembly {



LlamaAbsolutePeerReview.sol#1058
Severity: Low
1058         assembly {



LlamaAbsolutePeerReview.sol#1076
Severity: Low
1076         assembly {



LlamaAbsolutePeerReview.sol#1112
Severity: Low
1112         assembly {



LlamaAbsolutePeerReview.sol#1189
Severity: Low
1189         assembly {



LlamaAbsolutePeerReview.sol#1258
Severity: Low
1258         assembly {



LlamaAbsolutePeerReview.sol#1304
Severity: Low
1304         assembly {



LlamaAbsolutePeerReview.sol#1325
Severity: Low
1325         assembly {



LlamaAbsolutePeerReview.sol#1353
Severity: Low
1353         assembly {



LlamaAbsolutePeerReview.sol#1387
Severity: Low
1387         assembly {



LlamaAbsolutePeerReview.sol#1430
Severity: Low
1430         assembly {



LlamaAbsolutePeerReview.sol#1490
Severity: Low
1490         assembly {



LlamaAbsolutePeerReview.sol#1538
Severity: Low
1538         assembly {



LlamaAbsolutePeerReview.sol#1576
Severity: Low
1576         assembly {



LlamaAbsolutePeerReview.sol#1613
Severity: Low
1613         assembly {



LlamaAbsolutePeerReview.sol#1647
Severity: Low
1647         assembly {



LlamaAbsolutePeerReview.sol#1695
Severity: Low
1695         assembly {



LlamaAbsolutePeerReview.sol#1704
Severity: Low
1704         assembly {



LlamaAbsolutePeerReview.sol#1723
Severity: Low
1723         assembly {



LlamaAbsolutePeerReview.sol#1741
Severity: Low
1741         assembly {



LlamaAbsolutePeerReview.sol#1768
Severity: Low
1768         assembly {



LlamaAbsolutePeerReview.sol#1788
Severity: Low
1788         assembly {



LlamaAbsolutePeerReview.sol#2003
Severity: Low
2003         assembly {



LlamaAbsolutePeerReview.sol#2022
Severity: Low
2022         assembly {



LlamaAbsolutePeerReview.sol#2830
Severity: Low
2830         assembly {



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#225
Severity: Low
225         assembly {



LlamaAbsoluteQuorum.sol#242
Severity: Low
242         assembly {



LlamaAbsoluteQuorum.sol#260
Severity: Low
260         assembly {



LlamaAbsoluteQuorum.sol#349
Severity: Low
349         assembly {



LlamaAbsoluteQuorum.sol#414
Severity: Low
414         assembly {



LlamaAbsoluteQuorum.sol#423
Severity: Low
423         assembly {



LlamaAbsoluteQuorum.sol#432
Severity: Low
432         assembly {



LlamaAbsoluteQuorum.sol#516
Severity: Low
516         assembly {



LlamaAbsoluteQuorum.sol#538
Severity: Low
538         assembly {



LlamaAbsoluteQuorum.sol#560
Severity: Low
560         assembly {



LlamaAbsoluteQuorum.sol#725
Severity: Low
725         assembly {



LlamaAbsoluteQuorum.sol#769
Severity: Low
769         assembly {



LlamaAbsoluteQuorum.sol#791
Severity: Low
791         assembly {



LlamaAbsoluteQuorum.sol#810
Severity: Low
810         assembly {



LlamaAbsoluteQuorum.sol#861
Severity: Low
861         assembly {



LlamaAbsoluteQuorum.sol#876
Severity: Low
876         assembly {



LlamaAbsoluteQuorum.sol#891
Severity: Low
891         assembly {



LlamaAbsoluteQuorum.sol#905
Severity: Low
905         assembly {



LlamaAbsoluteQuorum.sol#946
Severity: Low
946         assembly {



LlamaAbsoluteQuorum.sol#967
Severity: Low
967         assembly {



LlamaAbsoluteQuorum.sol#979
Severity: Low
979         assembly {



LlamaAbsoluteQuorum.sol#1017
Severity: Low
1017         assembly {



LlamaAbsoluteQuorum.sol#1029
Severity: Low
1029         assembly {



LlamaAbsoluteQuorum.sol#1058
Severity: Low
1058         assembly {



LlamaAbsoluteQuorum.sol#1076
Severity: Low
1076         assembly {



LlamaAbsoluteQuorum.sol#1112
Severity: Low
1112         assembly {



LlamaAbsoluteQuorum.sol#1189
Severity: Low
1189         assembly {



LlamaAbsoluteQuorum.sol#1258
Severity: Low
1258         assembly {



LlamaAbsoluteQuorum.sol#1304
Severity: Low
1304         assembly {



LlamaAbsoluteQuorum.sol#1325
Severity: Low
1325         assembly {



LlamaAbsoluteQuorum.sol#1353
Severity: Low
1353         assembly {



LlamaAbsoluteQuorum.sol#1387
Severity: Low
1387         assembly {



LlamaAbsoluteQuorum.sol#1430
Severity: Low
1430         assembly {



LlamaAbsoluteQuorum.sol#1490
Severity: Low
1490         assembly {



LlamaAbsoluteQuorum.sol#1538
Severity: Low
1538         assembly {



LlamaAbsoluteQuorum.sol#1576
Severity: Low
1576         assembly {



LlamaAbsoluteQuorum.sol#1613
Severity: Low
1613         assembly {



LlamaAbsoluteQuorum.sol#1647
Severity: Low
1647         assembly {



LlamaAbsoluteQuorum.sol#1695
Severity: Low
1695         assembly {



LlamaAbsoluteQuorum.sol#1704
Severity: Low
1704         assembly {



LlamaAbsoluteQuorum.sol#1723
Severity: Low
1723         assembly {



LlamaAbsoluteQuorum.sol#1741
Severity: Low
1741         assembly {



LlamaAbsoluteQuorum.sol#1768
Severity: Low
1768         assembly {



LlamaAbsoluteQuorum.sol#1788
Severity: Low
1788         assembly {



LlamaAbsoluteQuorum.sol#2003
Severity: Low
2003         assembly {



LlamaAbsoluteQuorum.sol#2022
Severity: Low
2022         assembly {



LlamaAbsoluteQuorum.sol#2830
Severity: Low
2830         assembly {



```

### LlamaAccount.sol

```

LlamaAccount.sol#1193
Severity: Low
1193         assembly {



LlamaAccount.sol#1215
Severity: Low
1215         assembly {



LlamaAccount.sol#1237
Severity: Low
1237         assembly {



LlamaAccount.sol#1285
Severity: Low
1285         assembly {



LlamaAccount.sol#1329
Severity: Low
1329         assembly {



LlamaAccount.sol#1351
Severity: Low
1351         assembly {



LlamaAccount.sol#1370
Severity: Low
1370         assembly {



LlamaAccount.sol#1421
Severity: Low
1421         assembly {



LlamaAccount.sol#1436
Severity: Low
1436         assembly {



LlamaAccount.sol#1451
Severity: Low
1451         assembly {



LlamaAccount.sol#1465
Severity: Low
1465         assembly {



LlamaAccount.sol#1506
Severity: Low
1506         assembly {



LlamaAccount.sol#1527
Severity: Low
1527         assembly {



LlamaAccount.sol#1539
Severity: Low
1539         assembly {



LlamaAccount.sol#1577
Severity: Low
1577         assembly {



LlamaAccount.sol#1589
Severity: Low
1589         assembly {



LlamaAccount.sol#1618
Severity: Low
1618         assembly {



LlamaAccount.sol#1636
Severity: Low
1636         assembly {



LlamaAccount.sol#1672
Severity: Low
1672         assembly {



LlamaAccount.sol#1749
Severity: Low
1749         assembly {



LlamaAccount.sol#1818
Severity: Low
1818         assembly {



LlamaAccount.sol#1864
Severity: Low
1864         assembly {



LlamaAccount.sol#1885
Severity: Low
1885         assembly {



LlamaAccount.sol#1913
Severity: Low
1913         assembly {



LlamaAccount.sol#1947
Severity: Low
1947         assembly {



LlamaAccount.sol#1990
Severity: Low
1990         assembly {



LlamaAccount.sol#2050
Severity: Low
2050         assembly {



LlamaAccount.sol#2098
Severity: Low
2098         assembly {



LlamaAccount.sol#2136
Severity: Low
2136         assembly {



LlamaAccount.sol#2173
Severity: Low
2173         assembly {



LlamaAccount.sol#2207
Severity: Low
2207         assembly {



LlamaAccount.sol#2255
Severity: Low
2255         assembly {



LlamaAccount.sol#2264
Severity: Low
2264         assembly {



LlamaAccount.sol#2283
Severity: Low
2283         assembly {



LlamaAccount.sol#2301
Severity: Low
2301         assembly {



LlamaAccount.sol#2328
Severity: Low
2328         assembly {



LlamaAccount.sol#2348
Severity: Low
2348         assembly {



LlamaAccount.sol#2563
Severity: Low
2563         assembly {



LlamaAccount.sol#2582
Severity: Low
2582         assembly {



LlamaAccount.sol#2905
Severity: Low
2905         assembly {



```

### LlamaCore.sol

```

LlamaCore.sol#30
Severity: Low
30         assembly {



LlamaCore.sol#52
Severity: Low
52         assembly {



LlamaCore.sol#74
Severity: Low
74         assembly {



LlamaCore.sol#322
Severity: Low
322         assembly {



LlamaCore.sol#366
Severity: Low
366         assembly {



LlamaCore.sol#388
Severity: Low
388         assembly {



LlamaCore.sol#407
Severity: Low
407         assembly {



LlamaCore.sol#458
Severity: Low
458         assembly {



LlamaCore.sol#473
Severity: Low
473         assembly {



LlamaCore.sol#488
Severity: Low
488         assembly {



LlamaCore.sol#502
Severity: Low
502         assembly {



LlamaCore.sol#543
Severity: Low
543         assembly {



LlamaCore.sol#564
Severity: Low
564         assembly {



LlamaCore.sol#576
Severity: Low
576         assembly {



LlamaCore.sol#614
Severity: Low
614         assembly {



LlamaCore.sol#626
Severity: Low
626         assembly {



LlamaCore.sol#655
Severity: Low
655         assembly {



LlamaCore.sol#673
Severity: Low
673         assembly {



LlamaCore.sol#709
Severity: Low
709         assembly {



LlamaCore.sol#786
Severity: Low
786         assembly {



LlamaCore.sol#855
Severity: Low
855         assembly {



LlamaCore.sol#901
Severity: Low
901         assembly {



LlamaCore.sol#922
Severity: Low
922         assembly {



LlamaCore.sol#950
Severity: Low
950         assembly {



LlamaCore.sol#984
Severity: Low
984         assembly {



LlamaCore.sol#1027
Severity: Low
1027         assembly {



LlamaCore.sol#1087
Severity: Low
1087         assembly {



LlamaCore.sol#1135
Severity: Low
1135         assembly {



LlamaCore.sol#1173
Severity: Low
1173         assembly {



LlamaCore.sol#1210
Severity: Low
1210         assembly {



LlamaCore.sol#1244
Severity: Low
1244         assembly {



LlamaCore.sol#1292
Severity: Low
1292         assembly {



LlamaCore.sol#1301
Severity: Low
1301         assembly {



LlamaCore.sol#1320
Severity: Low
1320         assembly {



LlamaCore.sol#1338
Severity: Low
1338         assembly {



LlamaCore.sol#1365
Severity: Low
1365         assembly {



LlamaCore.sol#1385
Severity: Low
1385         assembly {



LlamaCore.sol#1625
Severity: Low
1625         assembly {



LlamaCore.sol#1644
Severity: Low
1644         assembly {



LlamaCore.sol#1967
Severity: Low
1967         assembly {



```

### LlamaFactory.sol

```

LlamaFactory.sol#30
Severity: Low
30         assembly {



LlamaFactory.sol#52
Severity: Low
52         assembly {



LlamaFactory.sol#74
Severity: Low
74         assembly {



LlamaFactory.sol#469
Severity: Low
469         assembly {



LlamaFactory.sol#513
Severity: Low
513         assembly {



LlamaFactory.sol#535
Severity: Low
535         assembly {



LlamaFactory.sol#554
Severity: Low
554         assembly {



LlamaFactory.sol#605
Severity: Low
605         assembly {



LlamaFactory.sol#620
Severity: Low
620         assembly {



LlamaFactory.sol#635
Severity: Low
635         assembly {



LlamaFactory.sol#649
Severity: Low
649         assembly {



LlamaFactory.sol#690
Severity: Low
690         assembly {



LlamaFactory.sol#711
Severity: Low
711         assembly {



LlamaFactory.sol#723
Severity: Low
723         assembly {



LlamaFactory.sol#761
Severity: Low
761         assembly {



LlamaFactory.sol#773
Severity: Low
773         assembly {



LlamaFactory.sol#802
Severity: Low
802         assembly {



LlamaFactory.sol#820
Severity: Low
820         assembly {



LlamaFactory.sol#856
Severity: Low
856         assembly {



LlamaFactory.sol#933
Severity: Low
933         assembly {



LlamaFactory.sol#1002
Severity: Low
1002         assembly {



LlamaFactory.sol#1048
Severity: Low
1048         assembly {



LlamaFactory.sol#1069
Severity: Low
1069         assembly {



LlamaFactory.sol#1097
Severity: Low
1097         assembly {



LlamaFactory.sol#1131
Severity: Low
1131         assembly {



LlamaFactory.sol#1174
Severity: Low
1174         assembly {



LlamaFactory.sol#1234
Severity: Low
1234         assembly {



LlamaFactory.sol#1282
Severity: Low
1282         assembly {



LlamaFactory.sol#1320
Severity: Low
1320         assembly {



LlamaFactory.sol#1357
Severity: Low
1357         assembly {



LlamaFactory.sol#1391
Severity: Low
1391         assembly {



LlamaFactory.sol#1439
Severity: Low
1439         assembly {



LlamaFactory.sol#1448
Severity: Low
1448         assembly {



LlamaFactory.sol#1467
Severity: Low
1467         assembly {



LlamaFactory.sol#1485
Severity: Low
1485         assembly {



LlamaFactory.sol#1512
Severity: Low
1512         assembly {



LlamaFactory.sol#1532
Severity: Low
1532         assembly {



LlamaFactory.sol#1747
Severity: Low
1747         assembly {



LlamaFactory.sol#1766
Severity: Low
1766         assembly {



LlamaFactory.sol#3467
Severity: Low
3467         assembly {



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#101
Severity: Low
101         assembly {



LlamaGovernanceScript.sol#123
Severity: Low
123         assembly {



LlamaGovernanceScript.sol#145
Severity: Low
145         assembly {



LlamaGovernanceScript.sol#493
Severity: Low
493         assembly {



LlamaGovernanceScript.sol#537
Severity: Low
537         assembly {



LlamaGovernanceScript.sol#559
Severity: Low
559         assembly {



LlamaGovernanceScript.sol#578
Severity: Low
578         assembly {



LlamaGovernanceScript.sol#629
Severity: Low
629         assembly {



LlamaGovernanceScript.sol#644
Severity: Low
644         assembly {



LlamaGovernanceScript.sol#659
Severity: Low
659         assembly {



LlamaGovernanceScript.sol#673
Severity: Low
673         assembly {



LlamaGovernanceScript.sol#714
Severity: Low
714         assembly {



LlamaGovernanceScript.sol#735
Severity: Low
735         assembly {



LlamaGovernanceScript.sol#747
Severity: Low
747         assembly {



LlamaGovernanceScript.sol#785
Severity: Low
785         assembly {



LlamaGovernanceScript.sol#797
Severity: Low
797         assembly {



LlamaGovernanceScript.sol#826
Severity: Low
826         assembly {



LlamaGovernanceScript.sol#844
Severity: Low
844         assembly {



LlamaGovernanceScript.sol#880
Severity: Low
880         assembly {



LlamaGovernanceScript.sol#957
Severity: Low
957         assembly {



LlamaGovernanceScript.sol#1026
Severity: Low
1026         assembly {



LlamaGovernanceScript.sol#1072
Severity: Low
1072         assembly {



LlamaGovernanceScript.sol#1093
Severity: Low
1093         assembly {



LlamaGovernanceScript.sol#1121
Severity: Low
1121         assembly {



LlamaGovernanceScript.sol#1155
Severity: Low
1155         assembly {



LlamaGovernanceScript.sol#1198
Severity: Low
1198         assembly {



LlamaGovernanceScript.sol#1258
Severity: Low
1258         assembly {



LlamaGovernanceScript.sol#1306
Severity: Low
1306         assembly {



LlamaGovernanceScript.sol#1344
Severity: Low
1344         assembly {



LlamaGovernanceScript.sol#1381
Severity: Low
1381         assembly {



LlamaGovernanceScript.sol#1415
Severity: Low
1415         assembly {



LlamaGovernanceScript.sol#1463
Severity: Low
1463         assembly {



LlamaGovernanceScript.sol#1472
Severity: Low
1472         assembly {



LlamaGovernanceScript.sol#1491
Severity: Low
1491         assembly {



LlamaGovernanceScript.sol#1509
Severity: Low
1509         assembly {



LlamaGovernanceScript.sol#1536
Severity: Low
1536         assembly {



LlamaGovernanceScript.sol#1556
Severity: Low
1556         assembly {



LlamaGovernanceScript.sol#1771
Severity: Low
1771         assembly {



LlamaGovernanceScript.sol#1790
Severity: Low
1790         assembly {



LlamaGovernanceScript.sol#2598
Severity: Low
2598         assembly {



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#29
Severity: Low
29         assembly {



LlamaPolicy.sol#73
Severity: Low
73         assembly {



LlamaPolicy.sol#95
Severity: Low
95         assembly {



LlamaPolicy.sol#114
Severity: Low
114         assembly {



LlamaPolicy.sol#165
Severity: Low
165         assembly {



LlamaPolicy.sol#180
Severity: Low
180         assembly {



LlamaPolicy.sol#195
Severity: Low
195         assembly {



LlamaPolicy.sol#209
Severity: Low
209         assembly {



LlamaPolicy.sol#250
Severity: Low
250         assembly {



LlamaPolicy.sol#271
Severity: Low
271         assembly {



LlamaPolicy.sol#283
Severity: Low
283         assembly {



LlamaPolicy.sol#321
Severity: Low
321         assembly {



LlamaPolicy.sol#333
Severity: Low
333         assembly {



LlamaPolicy.sol#362
Severity: Low
362         assembly {



LlamaPolicy.sol#380
Severity: Low
380         assembly {



LlamaPolicy.sol#416
Severity: Low
416         assembly {



LlamaPolicy.sol#493
Severity: Low
493         assembly {



LlamaPolicy.sol#562
Severity: Low
562         assembly {



LlamaPolicy.sol#608
Severity: Low
608         assembly {



LlamaPolicy.sol#629
Severity: Low
629         assembly {



LlamaPolicy.sol#657
Severity: Low
657         assembly {



LlamaPolicy.sol#691
Severity: Low
691         assembly {



LlamaPolicy.sol#734
Severity: Low
734         assembly {



LlamaPolicy.sol#794
Severity: Low
794         assembly {



LlamaPolicy.sol#842
Severity: Low
842         assembly {



LlamaPolicy.sol#880
Severity: Low
880         assembly {



LlamaPolicy.sol#917
Severity: Low
917         assembly {



LlamaPolicy.sol#951
Severity: Low
951         assembly {



LlamaPolicy.sol#999
Severity: Low
999         assembly {



LlamaPolicy.sol#1008
Severity: Low
1008         assembly {



LlamaPolicy.sol#1027
Severity: Low
1027         assembly {



LlamaPolicy.sol#1045
Severity: Low
1045         assembly {



LlamaPolicy.sol#1072
Severity: Low
1072         assembly {



LlamaPolicy.sol#1092
Severity: Low
1092         assembly {



LlamaPolicy.sol#1332
Severity: Low
1332         assembly {



LlamaPolicy.sol#1351
Severity: Low
1351         assembly {



LlamaPolicy.sol#1813
Severity: Low
1813         assembly {



LlamaPolicy.sol#1835
Severity: Low
1835         assembly {



LlamaPolicy.sol#1857
Severity: Low
1857         assembly {



LlamaPolicy.sol#2005
Severity: Low
2005         assembly {



```

### LlamaPolicyMetadata.sol

```

LlamaPolicyMetadata.sol#37
Severity: Low
37         assembly {



LlamaPolicyMetadata.sol#117
Severity: Low
117         assembly {



LlamaPolicyMetadata.sol#161
Severity: Low
161         assembly {



LlamaPolicyMetadata.sol#183
Severity: Low
183         assembly {



LlamaPolicyMetadata.sol#202
Severity: Low
202         assembly {



LlamaPolicyMetadata.sol#253
Severity: Low
253         assembly {



LlamaPolicyMetadata.sol#268
Severity: Low
268         assembly {



LlamaPolicyMetadata.sol#283
Severity: Low
283         assembly {



LlamaPolicyMetadata.sol#297
Severity: Low
297         assembly {



LlamaPolicyMetadata.sol#338
Severity: Low
338         assembly {



LlamaPolicyMetadata.sol#359
Severity: Low
359         assembly {



LlamaPolicyMetadata.sol#371
Severity: Low
371         assembly {



LlamaPolicyMetadata.sol#409
Severity: Low
409         assembly {



LlamaPolicyMetadata.sol#421
Severity: Low
421         assembly {



LlamaPolicyMetadata.sol#450
Severity: Low
450         assembly {



LlamaPolicyMetadata.sol#468
Severity: Low
468         assembly {



LlamaPolicyMetadata.sol#504
Severity: Low
504         assembly {



LlamaPolicyMetadata.sol#581
Severity: Low
581         assembly {



LlamaPolicyMetadata.sol#650
Severity: Low
650         assembly {



LlamaPolicyMetadata.sol#696
Severity: Low
696         assembly {



LlamaPolicyMetadata.sol#717
Severity: Low
717         assembly {



LlamaPolicyMetadata.sol#745
Severity: Low
745         assembly {



LlamaPolicyMetadata.sol#779
Severity: Low
779         assembly {



LlamaPolicyMetadata.sol#822
Severity: Low
822         assembly {



LlamaPolicyMetadata.sol#882
Severity: Low
882         assembly {



LlamaPolicyMetadata.sol#930
Severity: Low
930         assembly {



LlamaPolicyMetadata.sol#968
Severity: Low
968         assembly {



LlamaPolicyMetadata.sol#1005
Severity: Low
1005         assembly {



LlamaPolicyMetadata.sol#1039
Severity: Low
1039         assembly {



LlamaPolicyMetadata.sol#1087
Severity: Low
1087         assembly {



LlamaPolicyMetadata.sol#1096
Severity: Low
1096         assembly {



LlamaPolicyMetadata.sol#1115
Severity: Low
1115         assembly {



LlamaPolicyMetadata.sol#1133
Severity: Low
1133         assembly {



LlamaPolicyMetadata.sol#1160
Severity: Low
1160         assembly {



LlamaPolicyMetadata.sol#1180
Severity: Low
1180         assembly {



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#225
Severity: Low
225         assembly {



LlamaRelativeQuorum.sol#242
Severity: Low
242         assembly {



LlamaRelativeQuorum.sol#260
Severity: Low
260         assembly {



LlamaRelativeQuorum.sol#349
Severity: Low
349         assembly {



LlamaRelativeQuorum.sol#414
Severity: Low
414         assembly {



LlamaRelativeQuorum.sol#423
Severity: Low
423         assembly {



LlamaRelativeQuorum.sol#432
Severity: Low
432         assembly {



LlamaRelativeQuorum.sol#516
Severity: Low
516         assembly {



LlamaRelativeQuorum.sol#538
Severity: Low
538         assembly {



LlamaRelativeQuorum.sol#560
Severity: Low
560         assembly {



LlamaRelativeQuorum.sol#725
Severity: Low
725         assembly {



LlamaRelativeQuorum.sol#769
Severity: Low
769         assembly {



LlamaRelativeQuorum.sol#791
Severity: Low
791         assembly {



LlamaRelativeQuorum.sol#810
Severity: Low
810         assembly {



LlamaRelativeQuorum.sol#861
Severity: Low
861         assembly {



LlamaRelativeQuorum.sol#876
Severity: Low
876         assembly {



LlamaRelativeQuorum.sol#891
Severity: Low
891         assembly {



LlamaRelativeQuorum.sol#905
Severity: Low
905         assembly {



LlamaRelativeQuorum.sol#946
Severity: Low
946         assembly {



LlamaRelativeQuorum.sol#967
Severity: Low
967         assembly {



LlamaRelativeQuorum.sol#979
Severity: Low
979         assembly {



LlamaRelativeQuorum.sol#1017
Severity: Low
1017         assembly {



LlamaRelativeQuorum.sol#1029
Severity: Low
1029         assembly {



LlamaRelativeQuorum.sol#1058
Severity: Low
1058         assembly {



LlamaRelativeQuorum.sol#1076
Severity: Low
1076         assembly {



LlamaRelativeQuorum.sol#1112
Severity: Low
1112         assembly {



LlamaRelativeQuorum.sol#1189
Severity: Low
1189         assembly {



LlamaRelativeQuorum.sol#1258
Severity: Low
1258         assembly {



LlamaRelativeQuorum.sol#1304
Severity: Low
1304         assembly {



LlamaRelativeQuorum.sol#1325
Severity: Low
1325         assembly {



LlamaRelativeQuorum.sol#1353
Severity: Low
1353         assembly {



LlamaRelativeQuorum.sol#1387
Severity: Low
1387         assembly {



LlamaRelativeQuorum.sol#1430
Severity: Low
1430         assembly {



LlamaRelativeQuorum.sol#1490
Severity: Low
1490         assembly {



LlamaRelativeQuorum.sol#1538
Severity: Low
1538         assembly {



LlamaRelativeQuorum.sol#1576
Severity: Low
1576         assembly {



LlamaRelativeQuorum.sol#1613
Severity: Low
1613         assembly {



LlamaRelativeQuorum.sol#1647
Severity: Low
1647         assembly {



LlamaRelativeQuorum.sol#1695
Severity: Low
1695         assembly {



LlamaRelativeQuorum.sol#1704
Severity: Low
1704         assembly {



LlamaRelativeQuorum.sol#1723
Severity: Low
1723         assembly {



LlamaRelativeQuorum.sol#1741
Severity: Low
1741         assembly {



LlamaRelativeQuorum.sol#1768
Severity: Low
1768         assembly {



LlamaRelativeQuorum.sol#1788
Severity: Low
1788         assembly {



LlamaRelativeQuorum.sol#2003
Severity: Low
2003         assembly {



LlamaRelativeQuorum.sol#2022
Severity: Low
2022         assembly {



LlamaRelativeQuorum.sol#2830
Severity: Low
2830         assembly {



```

## SOLIDITY_VISIBILITY
The default function visibility level in contracts is ```public```, in interfaces - ```external```, state variable default visibility level is ```internal```.

In contracts, the fallback function can be ```external``` or ```public```. In interfaces, all the functions should be declared as ```external```. Explicitly define function visibility to prevent confusion.


### LlamaAbsolutePeerReview.sol

```

LlamaAbsolutePeerReview.sol#674
Severity: Low
674   constructor() {



LlamaAbsolutePeerReview.sol#2393
Severity: Low
2393   constructor() {



LlamaAbsolutePeerReview.sol#2402
Severity: Low
2402   function initialize(



LlamaAbsolutePeerReview.sol#3045
Severity: Low
3045   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaAbsolutePeerReview.sol#3169
Severity: Low
3169   constructor(



LlamaAbsolutePeerReview.sol#3553
Severity: Low
3553   constructor() {



LlamaAbsolutePeerReview.sol#3565
Severity: Low
3565   function initialize(



LlamaAbsolutePeerReview.sol#4375
Severity: Low
4375   constructor() {



LlamaAbsolutePeerReview.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaAbsolutePeerReview.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaAbsolutePeerReview.sol#75
Severity: Low
75     error NotInitializing();



LlamaAbsolutePeerReview.sol#75
Severity: Low
75     error NotInitializing();



LlamaAbsolutePeerReview.sol#507
Severity: Low
507     error ERC1167FailedCreateClone();



LlamaAbsolutePeerReview.sol#507
Severity: Low
507     error ERC1167FailedCreateClone();



LlamaAbsolutePeerReview.sol#641
Severity: Low
641   error UnsafeCast(uint256 n);



LlamaAbsolutePeerReview.sol#641
Severity: Low
641   error UnsafeCast(uint256 n);



LlamaAbsolutePeerReview.sol#668
Severity: Low
668   error OnlyLlamaCore();



LlamaAbsolutePeerReview.sol#668
Severity: Low
668   error OnlyLlamaCore();



LlamaAbsolutePeerReview.sol#709
Severity: Low
709     error HexLengthInsufficient();



LlamaAbsolutePeerReview.sol#709
Severity: Low
709     error HexLengthInsufficient();



LlamaAbsolutePeerReview.sol#2298
Severity: Low
2298   error ActionCreationAtSameTimestamp();



LlamaAbsolutePeerReview.sol#2298
Severity: Low
2298   error ActionCreationAtSameTimestamp();



LlamaAbsolutePeerReview.sol#2302
Severity: Low
2302   error AddressDoesNotHoldPolicy(address userAddress);



LlamaAbsolutePeerReview.sol#2302
Severity: Low
2302   error AddressDoesNotHoldPolicy(address userAddress);



LlamaAbsolutePeerReview.sol#2305
Severity: Low
2305   error AllHoldersRole();



LlamaAbsolutePeerReview.sol#2305
Severity: Low
2305   error AllHoldersRole();



LlamaAbsolutePeerReview.sol#2312
Severity: Low
2312   error InvalidIndices();



LlamaAbsolutePeerReview.sol#2312
Severity: Low
2312   error InvalidIndices();



LlamaAbsolutePeerReview.sol#2315
Severity: Low
2315   error InvalidRoleHolderInput();



LlamaAbsolutePeerReview.sol#2315
Severity: Low
2315   error InvalidRoleHolderInput();



LlamaAbsolutePeerReview.sol#2318
Severity: Low
2318   error NonTransferableToken();



LlamaAbsolutePeerReview.sol#2318
Severity: Low
2318   error NonTransferableToken();



LlamaAbsolutePeerReview.sol#2321
Severity: Low
2321   error OnlyLlama();



LlamaAbsolutePeerReview.sol#2321
Severity: Low
2321   error OnlyLlama();



LlamaAbsolutePeerReview.sol#2324
Severity: Low
2324   error RoleNotInitialized(uint8 role);



LlamaAbsolutePeerReview.sol#2324
Severity: Low
2324   error RoleNotInitialized(uint8 role);



LlamaAbsolutePeerReview.sol#2404
Severity: Low
2404     RoleDescription[] calldata roleDescriptions,



LlamaAbsolutePeerReview.sol#2405
Severity: Low
2405     RoleHolderData[] calldata roleHolders,



LlamaAbsolutePeerReview.sol#2406
Severity: Low
2406     RolePermissionData[] calldata rolePermissions



LlamaAbsolutePeerReview.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsolutePeerReview.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsolutePeerReview.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsolutePeerReview.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsolutePeerReview.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsolutePeerReview.sol#2409
Severity: Low
2409     factory = LlamaFactory(msg.sender);



LlamaAbsolutePeerReview.sol#2409
Severity: Low
2409     factory = LlamaFactory(msg.sender);



LlamaAbsolutePeerReview.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsolutePeerReview.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsolutePeerReview.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsolutePeerReview.sol#2411
Severity: Low
2411       _initializeRole(roleDescriptions[i]);



LlamaAbsolutePeerReview.sol#2411
Severity: Low
2411       _initializeRole(roleDescriptions[i]);



LlamaAbsolutePeerReview.sol#3003
Severity: Low
3003   error UnauthorizedCaller();



LlamaAbsolutePeerReview.sol#3003
Severity: Low
3003   error UnauthorizedCaller();



LlamaAbsolutePeerReview.sol#3093
Severity: Low
3093   error InvalidDeployConfiguration();



LlamaAbsolutePeerReview.sol#3093
Severity: Low
3093   error InvalidDeployConfiguration();



LlamaAbsolutePeerReview.sol#3096
Severity: Low
3096   error OnlyRootLlama();



LlamaAbsolutePeerReview.sol#3096
Severity: Low
3096   error OnlyRootLlama();



LlamaAbsolutePeerReview.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAbsolutePeerReview.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAbsolutePeerReview.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAbsolutePeerReview.sol#3372
Severity: Low
3372   error CannotSetExecutorAsTarget();



LlamaAbsolutePeerReview.sol#3372
Severity: Low
3372   error CannotSetExecutorAsTarget();



LlamaAbsolutePeerReview.sol#3375
Severity: Low
3375   error RestrictedAddress();



LlamaAbsolutePeerReview.sol#3375
Severity: Low
3375   error RestrictedAddress();



LlamaAbsolutePeerReview.sol#3378
Severity: Low
3378   error DuplicateCast();



LlamaAbsolutePeerReview.sol#3378
Severity: Low
3378   error DuplicateCast();



LlamaAbsolutePeerReview.sol#3382
Severity: Low
3382   error FailedActionExecution(bytes reason);



LlamaAbsolutePeerReview.sol#3382
Severity: Low
3382   error FailedActionExecution(bytes reason);



LlamaAbsolutePeerReview.sol#3385
Severity: Low
3385   error InfoHashMismatch();



LlamaAbsolutePeerReview.sol#3385
Severity: Low
3385   error InfoHashMismatch();



LlamaAbsolutePeerReview.sol#3388
Severity: Low
3388   error IncorrectMsgValue();



LlamaAbsolutePeerReview.sol#3388
Severity: Low
3388   error IncorrectMsgValue();



LlamaAbsolutePeerReview.sol#3392
Severity: Low
3392   error InvalidActionState(ActionState current);



LlamaAbsolutePeerReview.sol#3392
Severity: Low
3392   error InvalidActionState(ActionState current);



LlamaAbsolutePeerReview.sol#3395
Severity: Low
3395   error InvalidPolicyholder();



LlamaAbsolutePeerReview.sol#3395
Severity: Low
3395   error InvalidPolicyholder();



LlamaAbsolutePeerReview.sol#3398
Severity: Low
3398   error InvalidSignature();



LlamaAbsolutePeerReview.sol#3398
Severity: Low
3398   error InvalidSignature();



LlamaAbsolutePeerReview.sol#3401
Severity: Low
3401   error InvalidStrategy();



LlamaAbsolutePeerReview.sol#3401
Severity: Low
3401   error InvalidStrategy();



LlamaAbsolutePeerReview.sol#3404
Severity: Low
3404   error MinExecutionTimeCannotBeInThePast();



LlamaAbsolutePeerReview.sol#3404
Severity: Low
3404   error MinExecutionTimeCannotBeInThePast();



LlamaAbsolutePeerReview.sol#3407
Severity: Low
3407   error OnlyLlama();



LlamaAbsolutePeerReview.sol#3407
Severity: Low
3407   error OnlyLlama();



LlamaAbsolutePeerReview.sol#3410
Severity: Low
3410   error PolicyholderDoesNotHavePermission();



LlamaAbsolutePeerReview.sol#3410
Severity: Low
3410   error PolicyholderDoesNotHavePermission();



LlamaAbsolutePeerReview.sol#3413
Severity: Low
3413   error MinExecutionTimeNotReached();



LlamaAbsolutePeerReview.sol#3413
Severity: Low
3413   error MinExecutionTimeNotReached();



LlamaAbsolutePeerReview.sol#3416
Severity: Low
3416   error UnauthorizedStrategyLogic();



LlamaAbsolutePeerReview.sol#3416
Severity: Low
3416   error UnauthorizedStrategyLogic();



LlamaAbsolutePeerReview.sol#3419
Severity: Low
3419   error UnauthorizedAccountLogic();



LlamaAbsolutePeerReview.sol#3419
Severity: Low
3419   error UnauthorizedAccountLogic();



LlamaAbsolutePeerReview.sol#3570
Severity: Low
3570     bytes[] calldata initialStrategies,



LlamaAbsolutePeerReview.sol#3571
Severity: Low
3571     bytes[] calldata initialAccounts



LlamaAbsolutePeerReview.sol#3572
Severity: Low
3572   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaAbsolutePeerReview.sol#3574
Severity: Low
3574     name = _name;



LlamaAbsolutePeerReview.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaAbsolutePeerReview.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaAbsolutePeerReview.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaAbsolutePeerReview.sol#3578
Severity: Low
3578     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaAbsolutePeerReview.sol#3579
Severity: Low
3579     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaAbsolutePeerReview.sol#3579
Severity: Low
3579     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaAbsolutePeerReview.sol#3582
Severity: Low
3582     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaAbsolutePeerReview.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsolutePeerReview.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsolutePeerReview.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsolutePeerReview.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsolutePeerReview.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsolutePeerReview.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsolutePeerReview.sol#4280
Severity: Low
4280   error CannotCancelInState(ActionState currentState);



LlamaAbsolutePeerReview.sol#4280
Severity: Low
4280   error CannotCancelInState(ActionState currentState);



LlamaAbsolutePeerReview.sol#4283
Severity: Low
4283   error DisapprovalDisabled();



LlamaAbsolutePeerReview.sol#4283
Severity: Low
4283   error DisapprovalDisabled();



LlamaAbsolutePeerReview.sol#4286
Severity: Low
4286   error InsufficientApprovalQuantity();



LlamaAbsolutePeerReview.sol#4286
Severity: Low
4286   error InsufficientApprovalQuantity();



LlamaAbsolutePeerReview.sol#4289
Severity: Low
4289   error InsufficientDisapprovalQuantity();



LlamaAbsolutePeerReview.sol#4289
Severity: Low
4289   error InsufficientDisapprovalQuantity();



LlamaAbsolutePeerReview.sol#4293
Severity: Low
4293   error InvalidMinApprovals(uint256 minApprovals);



LlamaAbsolutePeerReview.sol#4293
Severity: Low
4293   error InvalidMinApprovals(uint256 minApprovals);



LlamaAbsolutePeerReview.sol#4297
Severity: Low
4297   error InvalidRole(uint8 role);



LlamaAbsolutePeerReview.sol#4297
Severity: Low
4297   error InvalidRole(uint8 role);



LlamaAbsolutePeerReview.sol#4300
Severity: Low
4300   error OnlyActionCreator();



LlamaAbsolutePeerReview.sol#4300
Severity: Low
4300   error OnlyActionCreator();



LlamaAbsolutePeerReview.sol#4304
Severity: Low
4304   error RoleHasZeroSupply(uint8 role);



LlamaAbsolutePeerReview.sol#4304
Severity: Low
4304   error RoleHasZeroSupply(uint8 role);



LlamaAbsolutePeerReview.sol#4308
Severity: Low
4308   error RoleNotInitialized(uint8 role);



LlamaAbsolutePeerReview.sol#4308
Severity: Low
4308   error RoleNotInitialized(uint8 role);



LlamaAbsolutePeerReview.sol#4559
Severity: Low
4559   error ActionCreatorCannotCast();



LlamaAbsolutePeerReview.sol#4559
Severity: Low
4559   error ActionCreatorCannotCast();



```

### LlamaAbsoluteQuorum.sol

```

LlamaAbsoluteQuorum.sol#674
Severity: Low
674   constructor() {



LlamaAbsoluteQuorum.sol#2393
Severity: Low
2393   constructor() {



LlamaAbsoluteQuorum.sol#2402
Severity: Low
2402   function initialize(



LlamaAbsoluteQuorum.sol#3045
Severity: Low
3045   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaAbsoluteQuorum.sol#3169
Severity: Low
3169   constructor(



LlamaAbsoluteQuorum.sol#3553
Severity: Low
3553   constructor() {



LlamaAbsoluteQuorum.sol#3565
Severity: Low
3565   function initialize(



LlamaAbsoluteQuorum.sol#4375
Severity: Low
4375   constructor() {



LlamaAbsoluteQuorum.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaAbsoluteQuorum.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaAbsoluteQuorum.sol#75
Severity: Low
75     error NotInitializing();



LlamaAbsoluteQuorum.sol#75
Severity: Low
75     error NotInitializing();



LlamaAbsoluteQuorum.sol#507
Severity: Low
507     error ERC1167FailedCreateClone();



LlamaAbsoluteQuorum.sol#507
Severity: Low
507     error ERC1167FailedCreateClone();



LlamaAbsoluteQuorum.sol#641
Severity: Low
641   error UnsafeCast(uint256 n);



LlamaAbsoluteQuorum.sol#641
Severity: Low
641   error UnsafeCast(uint256 n);



LlamaAbsoluteQuorum.sol#668
Severity: Low
668   error OnlyLlamaCore();



LlamaAbsoluteQuorum.sol#668
Severity: Low
668   error OnlyLlamaCore();



LlamaAbsoluteQuorum.sol#709
Severity: Low
709     error HexLengthInsufficient();



LlamaAbsoluteQuorum.sol#709
Severity: Low
709     error HexLengthInsufficient();



LlamaAbsoluteQuorum.sol#2298
Severity: Low
2298   error ActionCreationAtSameTimestamp();



LlamaAbsoluteQuorum.sol#2298
Severity: Low
2298   error ActionCreationAtSameTimestamp();



LlamaAbsoluteQuorum.sol#2302
Severity: Low
2302   error AddressDoesNotHoldPolicy(address userAddress);



LlamaAbsoluteQuorum.sol#2302
Severity: Low
2302   error AddressDoesNotHoldPolicy(address userAddress);



LlamaAbsoluteQuorum.sol#2305
Severity: Low
2305   error AllHoldersRole();



LlamaAbsoluteQuorum.sol#2305
Severity: Low
2305   error AllHoldersRole();



LlamaAbsoluteQuorum.sol#2312
Severity: Low
2312   error InvalidIndices();



LlamaAbsoluteQuorum.sol#2312
Severity: Low
2312   error InvalidIndices();



LlamaAbsoluteQuorum.sol#2315
Severity: Low
2315   error InvalidRoleHolderInput();



LlamaAbsoluteQuorum.sol#2315
Severity: Low
2315   error InvalidRoleHolderInput();



LlamaAbsoluteQuorum.sol#2318
Severity: Low
2318   error NonTransferableToken();



LlamaAbsoluteQuorum.sol#2318
Severity: Low
2318   error NonTransferableToken();



LlamaAbsoluteQuorum.sol#2321
Severity: Low
2321   error OnlyLlama();



LlamaAbsoluteQuorum.sol#2321
Severity: Low
2321   error OnlyLlama();



LlamaAbsoluteQuorum.sol#2324
Severity: Low
2324   error RoleNotInitialized(uint8 role);



LlamaAbsoluteQuorum.sol#2324
Severity: Low
2324   error RoleNotInitialized(uint8 role);



LlamaAbsoluteQuorum.sol#2404
Severity: Low
2404     RoleDescription[] calldata roleDescriptions,



LlamaAbsoluteQuorum.sol#2405
Severity: Low
2405     RoleHolderData[] calldata roleHolders,



LlamaAbsoluteQuorum.sol#2406
Severity: Low
2406     RolePermissionData[] calldata rolePermissions



LlamaAbsoluteQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsoluteQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsoluteQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsoluteQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsoluteQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAbsoluteQuorum.sol#2409
Severity: Low
2409     factory = LlamaFactory(msg.sender);



LlamaAbsoluteQuorum.sol#2409
Severity: Low
2409     factory = LlamaFactory(msg.sender);



LlamaAbsoluteQuorum.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsoluteQuorum.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsoluteQuorum.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAbsoluteQuorum.sol#2411
Severity: Low
2411       _initializeRole(roleDescriptions[i]);



LlamaAbsoluteQuorum.sol#2411
Severity: Low
2411       _initializeRole(roleDescriptions[i]);



LlamaAbsoluteQuorum.sol#3003
Severity: Low
3003   error UnauthorizedCaller();



LlamaAbsoluteQuorum.sol#3003
Severity: Low
3003   error UnauthorizedCaller();



LlamaAbsoluteQuorum.sol#3093
Severity: Low
3093   error InvalidDeployConfiguration();



LlamaAbsoluteQuorum.sol#3093
Severity: Low
3093   error InvalidDeployConfiguration();



LlamaAbsoluteQuorum.sol#3096
Severity: Low
3096   error OnlyRootLlama();



LlamaAbsoluteQuorum.sol#3096
Severity: Low
3096   error OnlyRootLlama();



LlamaAbsoluteQuorum.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAbsoluteQuorum.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAbsoluteQuorum.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAbsoluteQuorum.sol#3372
Severity: Low
3372   error CannotSetExecutorAsTarget();



LlamaAbsoluteQuorum.sol#3372
Severity: Low
3372   error CannotSetExecutorAsTarget();



LlamaAbsoluteQuorum.sol#3375
Severity: Low
3375   error RestrictedAddress();



LlamaAbsoluteQuorum.sol#3375
Severity: Low
3375   error RestrictedAddress();



LlamaAbsoluteQuorum.sol#3378
Severity: Low
3378   error DuplicateCast();



LlamaAbsoluteQuorum.sol#3378
Severity: Low
3378   error DuplicateCast();



LlamaAbsoluteQuorum.sol#3382
Severity: Low
3382   error FailedActionExecution(bytes reason);



LlamaAbsoluteQuorum.sol#3382
Severity: Low
3382   error FailedActionExecution(bytes reason);



LlamaAbsoluteQuorum.sol#3385
Severity: Low
3385   error InfoHashMismatch();



LlamaAbsoluteQuorum.sol#3385
Severity: Low
3385   error InfoHashMismatch();



LlamaAbsoluteQuorum.sol#3388
Severity: Low
3388   error IncorrectMsgValue();



LlamaAbsoluteQuorum.sol#3388
Severity: Low
3388   error IncorrectMsgValue();



LlamaAbsoluteQuorum.sol#3392
Severity: Low
3392   error InvalidActionState(ActionState current);



LlamaAbsoluteQuorum.sol#3392
Severity: Low
3392   error InvalidActionState(ActionState current);



LlamaAbsoluteQuorum.sol#3395
Severity: Low
3395   error InvalidPolicyholder();



LlamaAbsoluteQuorum.sol#3395
Severity: Low
3395   error InvalidPolicyholder();



LlamaAbsoluteQuorum.sol#3398
Severity: Low
3398   error InvalidSignature();



LlamaAbsoluteQuorum.sol#3398
Severity: Low
3398   error InvalidSignature();



LlamaAbsoluteQuorum.sol#3401
Severity: Low
3401   error InvalidStrategy();



LlamaAbsoluteQuorum.sol#3401
Severity: Low
3401   error InvalidStrategy();



LlamaAbsoluteQuorum.sol#3404
Severity: Low
3404   error MinExecutionTimeCannotBeInThePast();



LlamaAbsoluteQuorum.sol#3404
Severity: Low
3404   error MinExecutionTimeCannotBeInThePast();



LlamaAbsoluteQuorum.sol#3407
Severity: Low
3407   error OnlyLlama();



LlamaAbsoluteQuorum.sol#3407
Severity: Low
3407   error OnlyLlama();



LlamaAbsoluteQuorum.sol#3410
Severity: Low
3410   error PolicyholderDoesNotHavePermission();



LlamaAbsoluteQuorum.sol#3410
Severity: Low
3410   error PolicyholderDoesNotHavePermission();



LlamaAbsoluteQuorum.sol#3413
Severity: Low
3413   error MinExecutionTimeNotReached();



LlamaAbsoluteQuorum.sol#3413
Severity: Low
3413   error MinExecutionTimeNotReached();



LlamaAbsoluteQuorum.sol#3416
Severity: Low
3416   error UnauthorizedStrategyLogic();



LlamaAbsoluteQuorum.sol#3416
Severity: Low
3416   error UnauthorizedStrategyLogic();



LlamaAbsoluteQuorum.sol#3419
Severity: Low
3419   error UnauthorizedAccountLogic();



LlamaAbsoluteQuorum.sol#3419
Severity: Low
3419   error UnauthorizedAccountLogic();



LlamaAbsoluteQuorum.sol#3570
Severity: Low
3570     bytes[] calldata initialStrategies,



LlamaAbsoluteQuorum.sol#3571
Severity: Low
3571     bytes[] calldata initialAccounts



LlamaAbsoluteQuorum.sol#3572
Severity: Low
3572   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaAbsoluteQuorum.sol#3574
Severity: Low
3574     name = _name;



LlamaAbsoluteQuorum.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaAbsoluteQuorum.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaAbsoluteQuorum.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaAbsoluteQuorum.sol#3578
Severity: Low
3578     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaAbsoluteQuorum.sol#3579
Severity: Low
3579     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaAbsoluteQuorum.sol#3579
Severity: Low
3579     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaAbsoluteQuorum.sol#3582
Severity: Low
3582     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaAbsoluteQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsoluteQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsoluteQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsoluteQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsoluteQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsoluteQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAbsoluteQuorum.sol#4280
Severity: Low
4280   error CannotCancelInState(ActionState currentState);



LlamaAbsoluteQuorum.sol#4280
Severity: Low
4280   error CannotCancelInState(ActionState currentState);



LlamaAbsoluteQuorum.sol#4283
Severity: Low
4283   error DisapprovalDisabled();



LlamaAbsoluteQuorum.sol#4283
Severity: Low
4283   error DisapprovalDisabled();



LlamaAbsoluteQuorum.sol#4286
Severity: Low
4286   error InsufficientApprovalQuantity();



LlamaAbsoluteQuorum.sol#4286
Severity: Low
4286   error InsufficientApprovalQuantity();



LlamaAbsoluteQuorum.sol#4289
Severity: Low
4289   error InsufficientDisapprovalQuantity();



LlamaAbsoluteQuorum.sol#4289
Severity: Low
4289   error InsufficientDisapprovalQuantity();



LlamaAbsoluteQuorum.sol#4293
Severity: Low
4293   error InvalidMinApprovals(uint256 minApprovals);



LlamaAbsoluteQuorum.sol#4293
Severity: Low
4293   error InvalidMinApprovals(uint256 minApprovals);



LlamaAbsoluteQuorum.sol#4297
Severity: Low
4297   error InvalidRole(uint8 role);



LlamaAbsoluteQuorum.sol#4297
Severity: Low
4297   error InvalidRole(uint8 role);



LlamaAbsoluteQuorum.sol#4300
Severity: Low
4300   error OnlyActionCreator();



LlamaAbsoluteQuorum.sol#4300
Severity: Low
4300   error OnlyActionCreator();



LlamaAbsoluteQuorum.sol#4304
Severity: Low
4304   error RoleHasZeroSupply(uint8 role);



LlamaAbsoluteQuorum.sol#4304
Severity: Low
4304   error RoleHasZeroSupply(uint8 role);



LlamaAbsoluteQuorum.sol#4308
Severity: Low
4308   error RoleNotInitialized(uint8 role);



LlamaAbsoluteQuorum.sol#4308
Severity: Low
4308   error RoleNotInitialized(uint8 role);



```

### LlamaAccount.sol

```

LlamaAccount.sol#361
Severity: Low
361     function sendValue(address payable recipient, uint256 amount) internal {



LlamaAccount.sol#1001
Severity: Low
1001     function safeBatchTransferFrom(



LlamaAccount.sol#1081
Severity: Low
1081     function onERC1155BatchReceived(



LlamaAccount.sol#2849
Severity: Low
2849   constructor() {



LlamaAccount.sol#3120
Severity: Low
3120   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaAccount.sol#3244
Severity: Low
3244   constructor(



LlamaAccount.sol#3551
Severity: Low
3551   constructor() {



LlamaAccount.sol#3560
Severity: Low
3560   function initialize(



LlamaAccount.sol#4340
Severity: Low
4340   constructor() {



LlamaAccount.sol#4352
Severity: Low
4352   function initialize(



LlamaAccount.sol#5040
Severity: Low
5040   constructor() {



LlamaAccount.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaAccount.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaAccount.sol#75
Severity: Low
75     error NotInitializing();



LlamaAccount.sol#75
Severity: Low
75     error NotInitializing();



LlamaAccount.sol#333
Severity: Low
333     error AddressInsufficientBalance(address account);



LlamaAccount.sol#333
Severity: Low
333     error AddressInsufficientBalance(address account);



LlamaAccount.sol#338
Severity: Low
338     error AddressEmptyCode(address target);



LlamaAccount.sol#338
Severity: Low
338     error AddressEmptyCode(address target);



LlamaAccount.sol#343
Severity: Low
343     error FailedInnerCall();



LlamaAccount.sol#343
Severity: Low
343     error FailedInnerCall();



LlamaAccount.sol#361
Severity: Low
361     function sendValue(address payable recipient, uint256 amount) internal {



LlamaAccount.sol#361
Severity: Low
361     function sendValue(address payable recipient, uint256 amount) internal {



LlamaAccount.sol#362
Severity: Low
362         if (address(this).balance < amount) {



LlamaAccount.sol#362
Severity: Low
362         if (address(this).balance < amount) {



LlamaAccount.sol#362
Severity: Low
362         if (address(this).balance < amount) {



LlamaAccount.sol#363
Severity: Low
363             revert AddressInsufficientBalance(address(this));



LlamaAccount.sol#363
Severity: Low
363             revert AddressInsufficientBalance(address(this));



LlamaAccount.sol#363
Severity: Low
363             revert AddressInsufficientBalance(address(this));



LlamaAccount.sol#574
Severity: Low
574     error SafeERC20FailedOperation(address token);



LlamaAccount.sol#574
Severity: Low
574     error SafeERC20FailedOperation(address token);



LlamaAccount.sol#579
Severity: Low
579     error SafeERC20FailedDecreaseAllowance(address spender, uint256 currentAllowance, uint256 requestedDecrease);



LlamaAccount.sol#579
Severity: Low
579     error SafeERC20FailedDecreaseAllowance(address spender, uint256 currentAllowance, uint256 requestedDecrease);



LlamaAccount.sol#579
Severity: Low
579     error SafeERC20FailedDecreaseAllowance(address spender, uint256 currentAllowance, uint256 requestedDecrease);



LlamaAccount.sol#579
Severity: Low
579     error SafeERC20FailedDecreaseAllowance(address spender, uint256 currentAllowance, uint256 requestedDecrease);



LlamaAccount.sol#1004
Severity: Low
1004         uint256[] calldata ids,



LlamaAccount.sol#1005
Severity: Low
1005         uint256[] calldata values,



LlamaAccount.sol#1005
Severity: Low
1005         uint256[] calldata values,



LlamaAccount.sol#1006
Severity: Low
1006         bytes calldata data



LlamaAccount.sol#1084
Severity: Low
1084         uint256[] calldata ids,



LlamaAccount.sol#1085
Severity: Low
1085         uint256[] calldata values,



LlamaAccount.sol#1085
Severity: Low
1085         uint256[] calldata values,



LlamaAccount.sol#1086
Severity: Low
1086         bytes calldata data



LlamaAccount.sol#1087
Severity: Low
1087     ) external returns (bytes4);



LlamaAccount.sol#1145
Severity: Low
1145   error UnsafeCast(uint256 n);



LlamaAccount.sol#1145
Severity: Low
1145   error UnsafeCast(uint256 n);



LlamaAccount.sol#1184
Severity: Low
1184     error ERC1167FailedCreateClone();



LlamaAccount.sol#1184
Severity: Low
1184     error ERC1167FailedCreateClone();



LlamaAccount.sol#1269
Severity: Low
1269     error HexLengthInsufficient();



LlamaAccount.sol#1269
Severity: Low
1269     error HexLengthInsufficient();



LlamaAccount.sol#2843
Severity: Low
2843   error OnlyLlamaCore();



LlamaAccount.sol#2843
Severity: Low
2843   error OnlyLlamaCore();



LlamaAccount.sol#3078
Severity: Low
3078   error UnauthorizedCaller();



LlamaAccount.sol#3078
Severity: Low
3078   error UnauthorizedCaller();



LlamaAccount.sol#3168
Severity: Low
3168   error InvalidDeployConfiguration();



LlamaAccount.sol#3168
Severity: Low
3168   error InvalidDeployConfiguration();



LlamaAccount.sol#3171
Severity: Low
3171   error OnlyRootLlama();



LlamaAccount.sol#3171
Severity: Low
3171   error OnlyRootLlama();



LlamaAccount.sol#3456
Severity: Low
3456   error ActionCreationAtSameTimestamp();



LlamaAccount.sol#3456
Severity: Low
3456   error ActionCreationAtSameTimestamp();



LlamaAccount.sol#3460
Severity: Low
3460   error AddressDoesNotHoldPolicy(address userAddress);



LlamaAccount.sol#3460
Severity: Low
3460   error AddressDoesNotHoldPolicy(address userAddress);



LlamaAccount.sol#3463
Severity: Low
3463   error AllHoldersRole();



LlamaAccount.sol#3463
Severity: Low
3463   error AllHoldersRole();



LlamaAccount.sol#3470
Severity: Low
3470   error InvalidIndices();



LlamaAccount.sol#3470
Severity: Low
3470   error InvalidIndices();



LlamaAccount.sol#3473
Severity: Low
3473   error InvalidRoleHolderInput();



LlamaAccount.sol#3473
Severity: Low
3473   error InvalidRoleHolderInput();



LlamaAccount.sol#3476
Severity: Low
3476   error NonTransferableToken();



LlamaAccount.sol#3476
Severity: Low
3476   error NonTransferableToken();



LlamaAccount.sol#3479
Severity: Low
3479   error OnlyLlama();



LlamaAccount.sol#3479
Severity: Low
3479   error OnlyLlama();



LlamaAccount.sol#3482
Severity: Low
3482   error RoleNotInitialized(uint8 role);



LlamaAccount.sol#3482
Severity: Low
3482   error RoleNotInitialized(uint8 role);



LlamaAccount.sol#3562
Severity: Low
3562     RoleDescription[] calldata roleDescriptions,



LlamaAccount.sol#3563
Severity: Low
3563     RoleHolderData[] calldata roleHolders,



LlamaAccount.sol#3564
Severity: Low
3564     RolePermissionData[] calldata rolePermissions



LlamaAccount.sol#3566
Severity: Low
3566     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAccount.sol#3566
Severity: Low
3566     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAccount.sol#3566
Severity: Low
3566     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAccount.sol#3566
Severity: Low
3566     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAccount.sol#3566
Severity: Low
3566     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaAccount.sol#3567
Severity: Low
3567     factory = LlamaFactory(msg.sender);



LlamaAccount.sol#3567
Severity: Low
3567     factory = LlamaFactory(msg.sender);



LlamaAccount.sol#3568
Severity: Low
3568     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAccount.sol#3568
Severity: Low
3568     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAccount.sol#3568
Severity: Low
3568     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaAccount.sol#3569
Severity: Low
3569       _initializeRole(roleDescriptions[i]);



LlamaAccount.sol#3569
Severity: Low
3569       _initializeRole(roleDescriptions[i]);



LlamaAccount.sol#4156
Severity: Low
4156   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAccount.sol#4156
Severity: Low
4156   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAccount.sol#4156
Severity: Low
4156   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaAccount.sol#4159
Severity: Low
4159   error CannotSetExecutorAsTarget();



LlamaAccount.sol#4159
Severity: Low
4159   error CannotSetExecutorAsTarget();



LlamaAccount.sol#4162
Severity: Low
4162   error RestrictedAddress();



LlamaAccount.sol#4162
Severity: Low
4162   error RestrictedAddress();



LlamaAccount.sol#4165
Severity: Low
4165   error DuplicateCast();



LlamaAccount.sol#4165
Severity: Low
4165   error DuplicateCast();



LlamaAccount.sol#4169
Severity: Low
4169   error FailedActionExecution(bytes reason);



LlamaAccount.sol#4169
Severity: Low
4169   error FailedActionExecution(bytes reason);



LlamaAccount.sol#4172
Severity: Low
4172   error InfoHashMismatch();



LlamaAccount.sol#4172
Severity: Low
4172   error InfoHashMismatch();



LlamaAccount.sol#4175
Severity: Low
4175   error IncorrectMsgValue();



LlamaAccount.sol#4175
Severity: Low
4175   error IncorrectMsgValue();



LlamaAccount.sol#4179
Severity: Low
4179   error InvalidActionState(ActionState current);



LlamaAccount.sol#4179
Severity: Low
4179   error InvalidActionState(ActionState current);



LlamaAccount.sol#4182
Severity: Low
4182   error InvalidPolicyholder();



LlamaAccount.sol#4182
Severity: Low
4182   error InvalidPolicyholder();



LlamaAccount.sol#4185
Severity: Low
4185   error InvalidSignature();



LlamaAccount.sol#4185
Severity: Low
4185   error InvalidSignature();



LlamaAccount.sol#4188
Severity: Low
4188   error InvalidStrategy();



LlamaAccount.sol#4188
Severity: Low
4188   error InvalidStrategy();



LlamaAccount.sol#4191
Severity: Low
4191   error MinExecutionTimeCannotBeInThePast();



LlamaAccount.sol#4191
Severity: Low
4191   error MinExecutionTimeCannotBeInThePast();



LlamaAccount.sol#4194
Severity: Low
4194   error OnlyLlama();



LlamaAccount.sol#4194
Severity: Low
4194   error OnlyLlama();



LlamaAccount.sol#4197
Severity: Low
4197   error PolicyholderDoesNotHavePermission();



LlamaAccount.sol#4197
Severity: Low
4197   error PolicyholderDoesNotHavePermission();



LlamaAccount.sol#4200
Severity: Low
4200   error MinExecutionTimeNotReached();



LlamaAccount.sol#4200
Severity: Low
4200   error MinExecutionTimeNotReached();



LlamaAccount.sol#4203
Severity: Low
4203   error UnauthorizedStrategyLogic();



LlamaAccount.sol#4203
Severity: Low
4203   error UnauthorizedStrategyLogic();



LlamaAccount.sol#4206
Severity: Low
4206   error UnauthorizedAccountLogic();



LlamaAccount.sol#4206
Severity: Low
4206   error UnauthorizedAccountLogic();



LlamaAccount.sol#4357
Severity: Low
4357     bytes[] calldata initialStrategies,



LlamaAccount.sol#4358
Severity: Low
4358     bytes[] calldata initialAccounts



LlamaAccount.sol#4359
Severity: Low
4359   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaAccount.sol#4361
Severity: Low
4361     name = _name;



LlamaAccount.sol#4362
Severity: Low
4362     executor = new LlamaExecutor();



LlamaAccount.sol#4362
Severity: Low
4362     executor = new LlamaExecutor();



LlamaAccount.sol#4362
Severity: Low
4362     executor = new LlamaExecutor();



LlamaAccount.sol#4365
Severity: Low
4365     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaAccount.sol#4366
Severity: Low
4366     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaAccount.sol#4366
Severity: Low
4366     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaAccount.sol#4369
Severity: Low
4369     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaAccount.sol#4370
Severity: Low
4370     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAccount.sol#4370
Severity: Low
4370     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAccount.sol#4370
Severity: Low
4370     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAccount.sol#4370
Severity: Low
4370     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAccount.sol#4370
Severity: Low
4370     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAccount.sol#4370
Severity: Low
4370     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaAccount.sol#5006
Severity: Low
5006   error OnlyLlama();



LlamaAccount.sol#5006
Severity: Low
5006   error OnlyLlama();



LlamaAccount.sol#5009
Severity: Low
5009   error ZeroAddressNotAllowed();



LlamaAccount.sol#5009
Severity: Low
5009   error ZeroAddressNotAllowed();



LlamaAccount.sol#5013
Severity: Low
5013   error FailedExecution(bytes result);



LlamaAccount.sol#5013
Severity: Low
5013   error FailedExecution(bytes result);



LlamaAccount.sol#5016
Severity: Low
5016   error Slot0Changed();



LlamaAccount.sol#5016
Severity: Low
5016   error Slot0Changed();



LlamaAccount.sol#5059
Severity: Low
5059   receive() external payable {}



```

### LlamaCore.sol

```

LlamaCore.sol#1911
Severity: Low
1911   constructor() {



LlamaCore.sol#2182
Severity: Low
2182   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaCore.sol#2306
Severity: Low
2306   constructor(



LlamaCore.sol#2613
Severity: Low
2613   constructor() {



LlamaCore.sol#2622
Severity: Low
2622   function initialize(



LlamaCore.sol#3402
Severity: Low
3402   constructor() {



LlamaCore.sol#3414
Severity: Low
3414   function initialize(



LlamaCore.sol#21
Severity: Low
21     error ERC1167FailedCreateClone();



LlamaCore.sol#21
Severity: Low
21     error ERC1167FailedCreateClone();



LlamaCore.sol#163
Severity: Low
163     error AlreadyInitialized();



LlamaCore.sol#163
Severity: Low
163     error AlreadyInitialized();



LlamaCore.sol#168
Severity: Low
168     error NotInitializing();



LlamaCore.sol#168
Severity: Low
168     error NotInitializing();



LlamaCore.sol#306
Severity: Low
306     error HexLengthInsufficient();



LlamaCore.sol#306
Severity: Low
306     error HexLengthInsufficient();



LlamaCore.sol#1405
Severity: Low
1405   error UnsafeCast(uint256 n);



LlamaCore.sol#1405
Severity: Low
1405   error UnsafeCast(uint256 n);



LlamaCore.sol#1905
Severity: Low
1905   error OnlyLlamaCore();



LlamaCore.sol#1905
Severity: Low
1905   error OnlyLlamaCore();



LlamaCore.sol#2140
Severity: Low
2140   error UnauthorizedCaller();



LlamaCore.sol#2140
Severity: Low
2140   error UnauthorizedCaller();



LlamaCore.sol#2230
Severity: Low
2230   error InvalidDeployConfiguration();



LlamaCore.sol#2230
Severity: Low
2230   error InvalidDeployConfiguration();



LlamaCore.sol#2233
Severity: Low
2233   error OnlyRootLlama();



LlamaCore.sol#2233
Severity: Low
2233   error OnlyRootLlama();



LlamaCore.sol#2518
Severity: Low
2518   error ActionCreationAtSameTimestamp();



LlamaCore.sol#2518
Severity: Low
2518   error ActionCreationAtSameTimestamp();



LlamaCore.sol#2522
Severity: Low
2522   error AddressDoesNotHoldPolicy(address userAddress);



LlamaCore.sol#2522
Severity: Low
2522   error AddressDoesNotHoldPolicy(address userAddress);



LlamaCore.sol#2525
Severity: Low
2525   error AllHoldersRole();



LlamaCore.sol#2525
Severity: Low
2525   error AllHoldersRole();



LlamaCore.sol#2532
Severity: Low
2532   error InvalidIndices();



LlamaCore.sol#2532
Severity: Low
2532   error InvalidIndices();



LlamaCore.sol#2535
Severity: Low
2535   error InvalidRoleHolderInput();



LlamaCore.sol#2535
Severity: Low
2535   error InvalidRoleHolderInput();



LlamaCore.sol#2538
Severity: Low
2538   error NonTransferableToken();



LlamaCore.sol#2538
Severity: Low
2538   error NonTransferableToken();



LlamaCore.sol#2541
Severity: Low
2541   error OnlyLlama();



LlamaCore.sol#2541
Severity: Low
2541   error OnlyLlama();



LlamaCore.sol#2544
Severity: Low
2544   error RoleNotInitialized(uint8 role);



LlamaCore.sol#2544
Severity: Low
2544   error RoleNotInitialized(uint8 role);



LlamaCore.sol#2624
Severity: Low
2624     RoleDescription[] calldata roleDescriptions,



LlamaCore.sol#2625
Severity: Low
2625     RoleHolderData[] calldata roleHolders,



LlamaCore.sol#2626
Severity: Low
2626     RolePermissionData[] calldata rolePermissions



LlamaCore.sol#2628
Severity: Low
2628     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaCore.sol#2628
Severity: Low
2628     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaCore.sol#2628
Severity: Low
2628     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaCore.sol#2628
Severity: Low
2628     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaCore.sol#2628
Severity: Low
2628     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaCore.sol#2629
Severity: Low
2629     factory = LlamaFactory(msg.sender);



LlamaCore.sol#2629
Severity: Low
2629     factory = LlamaFactory(msg.sender);



LlamaCore.sol#2630
Severity: Low
2630     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaCore.sol#2630
Severity: Low
2630     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaCore.sol#2630
Severity: Low
2630     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaCore.sol#2631
Severity: Low
2631       _initializeRole(roleDescriptions[i]);



LlamaCore.sol#2631
Severity: Low
2631       _initializeRole(roleDescriptions[i]);



LlamaCore.sol#3218
Severity: Low
3218   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaCore.sol#3218
Severity: Low
3218   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaCore.sol#3218
Severity: Low
3218   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaCore.sol#3221
Severity: Low
3221   error CannotSetExecutorAsTarget();



LlamaCore.sol#3221
Severity: Low
3221   error CannotSetExecutorAsTarget();



LlamaCore.sol#3224
Severity: Low
3224   error RestrictedAddress();



LlamaCore.sol#3224
Severity: Low
3224   error RestrictedAddress();



LlamaCore.sol#3227
Severity: Low
3227   error DuplicateCast();



LlamaCore.sol#3227
Severity: Low
3227   error DuplicateCast();



LlamaCore.sol#3231
Severity: Low
3231   error FailedActionExecution(bytes reason);



LlamaCore.sol#3231
Severity: Low
3231   error FailedActionExecution(bytes reason);



LlamaCore.sol#3234
Severity: Low
3234   error InfoHashMismatch();



LlamaCore.sol#3234
Severity: Low
3234   error InfoHashMismatch();



LlamaCore.sol#3237
Severity: Low
3237   error IncorrectMsgValue();



LlamaCore.sol#3237
Severity: Low
3237   error IncorrectMsgValue();



LlamaCore.sol#3241
Severity: Low
3241   error InvalidActionState(ActionState current);



LlamaCore.sol#3241
Severity: Low
3241   error InvalidActionState(ActionState current);



LlamaCore.sol#3244
Severity: Low
3244   error InvalidPolicyholder();



LlamaCore.sol#3244
Severity: Low
3244   error InvalidPolicyholder();



LlamaCore.sol#3247
Severity: Low
3247   error InvalidSignature();



LlamaCore.sol#3247
Severity: Low
3247   error InvalidSignature();



LlamaCore.sol#3250
Severity: Low
3250   error InvalidStrategy();



LlamaCore.sol#3250
Severity: Low
3250   error InvalidStrategy();



LlamaCore.sol#3253
Severity: Low
3253   error MinExecutionTimeCannotBeInThePast();



LlamaCore.sol#3253
Severity: Low
3253   error MinExecutionTimeCannotBeInThePast();



LlamaCore.sol#3256
Severity: Low
3256   error OnlyLlama();



LlamaCore.sol#3256
Severity: Low
3256   error OnlyLlama();



LlamaCore.sol#3259
Severity: Low
3259   error PolicyholderDoesNotHavePermission();



LlamaCore.sol#3259
Severity: Low
3259   error PolicyholderDoesNotHavePermission();



LlamaCore.sol#3262
Severity: Low
3262   error MinExecutionTimeNotReached();



LlamaCore.sol#3262
Severity: Low
3262   error MinExecutionTimeNotReached();



LlamaCore.sol#3265
Severity: Low
3265   error UnauthorizedStrategyLogic();



LlamaCore.sol#3265
Severity: Low
3265   error UnauthorizedStrategyLogic();



LlamaCore.sol#3268
Severity: Low
3268   error UnauthorizedAccountLogic();



LlamaCore.sol#3268
Severity: Low
3268   error UnauthorizedAccountLogic();



LlamaCore.sol#3419
Severity: Low
3419     bytes[] calldata initialStrategies,



LlamaCore.sol#3420
Severity: Low
3420     bytes[] calldata initialAccounts



LlamaCore.sol#3421
Severity: Low
3421   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaCore.sol#3423
Severity: Low
3423     name = _name;



LlamaCore.sol#3424
Severity: Low
3424     executor = new LlamaExecutor();



LlamaCore.sol#3424
Severity: Low
3424     executor = new LlamaExecutor();



LlamaCore.sol#3424
Severity: Low
3424     executor = new LlamaExecutor();



LlamaCore.sol#3427
Severity: Low
3427     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaCore.sol#3428
Severity: Low
3428     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaCore.sol#3428
Severity: Low
3428     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaCore.sol#3431
Severity: Low
3431     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaCore.sol#3432
Severity: Low
3432     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaCore.sol#3432
Severity: Low
3432     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaCore.sol#3432
Severity: Low
3432     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaCore.sol#3432
Severity: Low
3432     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaCore.sol#3432
Severity: Low
3432     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaCore.sol#3432
Severity: Low
3432     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



```

### LlamaExecutor.sol

```

LlamaExecutor.sol#15
Severity: Low
15   constructor() {



LlamaExecutor.sol#9
Severity: Low
9   error OnlyLlamaCore();



LlamaExecutor.sol#9
Severity: Low
9   error OnlyLlamaCore();



```

### LlamaFactory.sol

```

LlamaFactory.sol#421
Severity: Low
421   constructor() {



LlamaFactory.sol#2140
Severity: Low
2140   constructor() {



LlamaFactory.sol#2149
Severity: Low
2149   function initialize(



LlamaFactory.sol#2739
Severity: Low
2739   constructor() {



LlamaFactory.sol#2751
Severity: Low
2751   function initialize(



LlamaFactory.sol#3682
Severity: Low
3682   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaFactory.sol#3806
Severity: Low
3806   constructor(



LlamaFactory.sol#21
Severity: Low
21     error ERC1167FailedCreateClone();



LlamaFactory.sol#21
Severity: Low
21     error ERC1167FailedCreateClone();



LlamaFactory.sol#230
Severity: Low
230     error AlreadyInitialized();



LlamaFactory.sol#230
Severity: Low
230     error AlreadyInitialized();



LlamaFactory.sol#235
Severity: Low
235     error NotInitializing();



LlamaFactory.sol#235
Severity: Low
235     error NotInitializing();



LlamaFactory.sol#388
Severity: Low
388   error UnsafeCast(uint256 n);



LlamaFactory.sol#388
Severity: Low
388   error UnsafeCast(uint256 n);



LlamaFactory.sol#415
Severity: Low
415   error OnlyLlamaCore();



LlamaFactory.sol#415
Severity: Low
415   error OnlyLlamaCore();



LlamaFactory.sol#453
Severity: Low
453     error HexLengthInsufficient();



LlamaFactory.sol#453
Severity: Low
453     error HexLengthInsufficient();



LlamaFactory.sol#2045
Severity: Low
2045   error ActionCreationAtSameTimestamp();



LlamaFactory.sol#2045
Severity: Low
2045   error ActionCreationAtSameTimestamp();



LlamaFactory.sol#2049
Severity: Low
2049   error AddressDoesNotHoldPolicy(address userAddress);



LlamaFactory.sol#2049
Severity: Low
2049   error AddressDoesNotHoldPolicy(address userAddress);



LlamaFactory.sol#2052
Severity: Low
2052   error AllHoldersRole();



LlamaFactory.sol#2052
Severity: Low
2052   error AllHoldersRole();



LlamaFactory.sol#2059
Severity: Low
2059   error InvalidIndices();



LlamaFactory.sol#2059
Severity: Low
2059   error InvalidIndices();



LlamaFactory.sol#2062
Severity: Low
2062   error InvalidRoleHolderInput();



LlamaFactory.sol#2062
Severity: Low
2062   error InvalidRoleHolderInput();



LlamaFactory.sol#2065
Severity: Low
2065   error NonTransferableToken();



LlamaFactory.sol#2065
Severity: Low
2065   error NonTransferableToken();



LlamaFactory.sol#2068
Severity: Low
2068   error OnlyLlama();



LlamaFactory.sol#2068
Severity: Low
2068   error OnlyLlama();



LlamaFactory.sol#2071
Severity: Low
2071   error RoleNotInitialized(uint8 role);



LlamaFactory.sol#2071
Severity: Low
2071   error RoleNotInitialized(uint8 role);



LlamaFactory.sol#2151
Severity: Low
2151     RoleDescription[] calldata roleDescriptions,



LlamaFactory.sol#2152
Severity: Low
2152     RoleHolderData[] calldata roleHolders,



LlamaFactory.sol#2153
Severity: Low
2153     RolePermissionData[] calldata rolePermissions



LlamaFactory.sol#2155
Severity: Low
2155     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaFactory.sol#2155
Severity: Low
2155     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaFactory.sol#2155
Severity: Low
2155     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaFactory.sol#2155
Severity: Low
2155     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaFactory.sol#2155
Severity: Low
2155     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaFactory.sol#2156
Severity: Low
2156     factory = LlamaFactory(msg.sender);



LlamaFactory.sol#2156
Severity: Low
2156     factory = LlamaFactory(msg.sender);



LlamaFactory.sol#2157
Severity: Low
2157     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaFactory.sol#2157
Severity: Low
2157     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaFactory.sol#2157
Severity: Low
2157     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaFactory.sol#2158
Severity: Low
2158       _initializeRole(roleDescriptions[i]);



LlamaFactory.sol#2158
Severity: Low
2158       _initializeRole(roleDescriptions[i]);



LlamaFactory.sol#2555
Severity: Low
2555   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaFactory.sol#2555
Severity: Low
2555   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaFactory.sol#2555
Severity: Low
2555   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaFactory.sol#2558
Severity: Low
2558   error CannotSetExecutorAsTarget();



LlamaFactory.sol#2558
Severity: Low
2558   error CannotSetExecutorAsTarget();



LlamaFactory.sol#2561
Severity: Low
2561   error RestrictedAddress();



LlamaFactory.sol#2561
Severity: Low
2561   error RestrictedAddress();



LlamaFactory.sol#2564
Severity: Low
2564   error DuplicateCast();



LlamaFactory.sol#2564
Severity: Low
2564   error DuplicateCast();



LlamaFactory.sol#2568
Severity: Low
2568   error FailedActionExecution(bytes reason);



LlamaFactory.sol#2568
Severity: Low
2568   error FailedActionExecution(bytes reason);



LlamaFactory.sol#2571
Severity: Low
2571   error InfoHashMismatch();



LlamaFactory.sol#2571
Severity: Low
2571   error InfoHashMismatch();



LlamaFactory.sol#2574
Severity: Low
2574   error IncorrectMsgValue();



LlamaFactory.sol#2574
Severity: Low
2574   error IncorrectMsgValue();



LlamaFactory.sol#2578
Severity: Low
2578   error InvalidActionState(ActionState current);



LlamaFactory.sol#2578
Severity: Low
2578   error InvalidActionState(ActionState current);



LlamaFactory.sol#2581
Severity: Low
2581   error InvalidPolicyholder();



LlamaFactory.sol#2581
Severity: Low
2581   error InvalidPolicyholder();



LlamaFactory.sol#2584
Severity: Low
2584   error InvalidSignature();



LlamaFactory.sol#2584
Severity: Low
2584   error InvalidSignature();



LlamaFactory.sol#2587
Severity: Low
2587   error InvalidStrategy();



LlamaFactory.sol#2587
Severity: Low
2587   error InvalidStrategy();



LlamaFactory.sol#2590
Severity: Low
2590   error MinExecutionTimeCannotBeInThePast();



LlamaFactory.sol#2590
Severity: Low
2590   error MinExecutionTimeCannotBeInThePast();



LlamaFactory.sol#2593
Severity: Low
2593   error OnlyLlama();



LlamaFactory.sol#2593
Severity: Low
2593   error OnlyLlama();



LlamaFactory.sol#2596
Severity: Low
2596   error PolicyholderDoesNotHavePermission();



LlamaFactory.sol#2596
Severity: Low
2596   error PolicyholderDoesNotHavePermission();



LlamaFactory.sol#2599
Severity: Low
2599   error MinExecutionTimeNotReached();



LlamaFactory.sol#2599
Severity: Low
2599   error MinExecutionTimeNotReached();



LlamaFactory.sol#2602
Severity: Low
2602   error UnauthorizedStrategyLogic();



LlamaFactory.sol#2602
Severity: Low
2602   error UnauthorizedStrategyLogic();



LlamaFactory.sol#2605
Severity: Low
2605   error UnauthorizedAccountLogic();



LlamaFactory.sol#2605
Severity: Low
2605   error UnauthorizedAccountLogic();



LlamaFactory.sol#2756
Severity: Low
2756     bytes[] calldata initialStrategies,



LlamaFactory.sol#2757
Severity: Low
2757     bytes[] calldata initialAccounts



LlamaFactory.sol#2758
Severity: Low
2758   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaFactory.sol#2760
Severity: Low
2760     name = _name;



LlamaFactory.sol#2761
Severity: Low
2761     executor = new LlamaExecutor();



LlamaFactory.sol#2761
Severity: Low
2761     executor = new LlamaExecutor();



LlamaFactory.sol#2761
Severity: Low
2761     executor = new LlamaExecutor();



LlamaFactory.sol#2764
Severity: Low
2764     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaFactory.sol#2765
Severity: Low
2765     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaFactory.sol#2765
Severity: Low
2765     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaFactory.sol#2768
Severity: Low
2768     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaFactory.sol#2769
Severity: Low
2769     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaFactory.sol#2769
Severity: Low
2769     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaFactory.sol#2769
Severity: Low
2769     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaFactory.sol#2769
Severity: Low
2769     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaFactory.sol#2769
Severity: Low
2769     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaFactory.sol#2769
Severity: Low
2769     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaFactory.sol#3640
Severity: Low
3640   error UnauthorizedCaller();



LlamaFactory.sol#3640
Severity: Low
3640   error UnauthorizedCaller();



LlamaFactory.sol#3730
Severity: Low
3730   error InvalidDeployConfiguration();



LlamaFactory.sol#3730
Severity: Low
3730   error InvalidDeployConfiguration();



LlamaFactory.sol#3733
Severity: Low
3733   error OnlyRootLlama();



LlamaFactory.sol#3733
Severity: Low
3733   error OnlyRootLlama();



```

### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#20
Severity: Low
20   constructor() {



LlamaGovernanceScript.sol#442
Severity: Low
442   constructor() {



LlamaGovernanceScript.sol#2161
Severity: Low
2161   constructor() {



LlamaGovernanceScript.sol#2170
Severity: Low
2170   function initialize(



LlamaGovernanceScript.sol#2813
Severity: Low
2813   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaGovernanceScript.sol#2937
Severity: Low
2937   constructor(



LlamaGovernanceScript.sol#3321
Severity: Low
3321   constructor() {



LlamaGovernanceScript.sol#3333
Severity: Low
3333   function initialize(



LlamaGovernanceScript.sol#4104
Severity: Low
4104   function initializeRolesAndSetRoleHoldersAndSetRolePermissions(



LlamaGovernanceScript.sol#7
Severity: Low
7   error OnlyDelegateCall();



LlamaGovernanceScript.sol#7
Severity: Low
7   error OnlyDelegateCall();



LlamaGovernanceScript.sol#92
Severity: Low
92     error ERC1167FailedCreateClone();



LlamaGovernanceScript.sol#92
Severity: Low
92     error ERC1167FailedCreateClone();



LlamaGovernanceScript.sol#234
Severity: Low
234     error AlreadyInitialized();



LlamaGovernanceScript.sol#234
Severity: Low
234     error AlreadyInitialized();



LlamaGovernanceScript.sol#239
Severity: Low
239     error NotInitializing();



LlamaGovernanceScript.sol#239
Severity: Low
239     error NotInitializing();



LlamaGovernanceScript.sol#409
Severity: Low
409   error UnsafeCast(uint256 n);



LlamaGovernanceScript.sol#409
Severity: Low
409   error UnsafeCast(uint256 n);



LlamaGovernanceScript.sol#436
Severity: Low
436   error OnlyLlamaCore();



LlamaGovernanceScript.sol#436
Severity: Low
436   error OnlyLlamaCore();



LlamaGovernanceScript.sol#477
Severity: Low
477     error HexLengthInsufficient();



LlamaGovernanceScript.sol#477
Severity: Low
477     error HexLengthInsufficient();



LlamaGovernanceScript.sol#2066
Severity: Low
2066   error ActionCreationAtSameTimestamp();



LlamaGovernanceScript.sol#2066
Severity: Low
2066   error ActionCreationAtSameTimestamp();



LlamaGovernanceScript.sol#2070
Severity: Low
2070   error AddressDoesNotHoldPolicy(address userAddress);



LlamaGovernanceScript.sol#2070
Severity: Low
2070   error AddressDoesNotHoldPolicy(address userAddress);



LlamaGovernanceScript.sol#2073
Severity: Low
2073   error AllHoldersRole();



LlamaGovernanceScript.sol#2073
Severity: Low
2073   error AllHoldersRole();



LlamaGovernanceScript.sol#2080
Severity: Low
2080   error InvalidIndices();



LlamaGovernanceScript.sol#2080
Severity: Low
2080   error InvalidIndices();



LlamaGovernanceScript.sol#2083
Severity: Low
2083   error InvalidRoleHolderInput();



LlamaGovernanceScript.sol#2083
Severity: Low
2083   error InvalidRoleHolderInput();



LlamaGovernanceScript.sol#2086
Severity: Low
2086   error NonTransferableToken();



LlamaGovernanceScript.sol#2086
Severity: Low
2086   error NonTransferableToken();



LlamaGovernanceScript.sol#2089
Severity: Low
2089   error OnlyLlama();



LlamaGovernanceScript.sol#2089
Severity: Low
2089   error OnlyLlama();



LlamaGovernanceScript.sol#2092
Severity: Low
2092   error RoleNotInitialized(uint8 role);



LlamaGovernanceScript.sol#2092
Severity: Low
2092   error RoleNotInitialized(uint8 role);



LlamaGovernanceScript.sol#2172
Severity: Low
2172     RoleDescription[] calldata roleDescriptions,



LlamaGovernanceScript.sol#2173
Severity: Low
2173     RoleHolderData[] calldata roleHolders,



LlamaGovernanceScript.sol#2174
Severity: Low
2174     RolePermissionData[] calldata rolePermissions



LlamaGovernanceScript.sol#2176
Severity: Low
2176     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaGovernanceScript.sol#2176
Severity: Low
2176     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaGovernanceScript.sol#2176
Severity: Low
2176     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaGovernanceScript.sol#2176
Severity: Low
2176     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaGovernanceScript.sol#2176
Severity: Low
2176     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaGovernanceScript.sol#2177
Severity: Low
2177     factory = LlamaFactory(msg.sender);



LlamaGovernanceScript.sol#2177
Severity: Low
2177     factory = LlamaFactory(msg.sender);



LlamaGovernanceScript.sol#2178
Severity: Low
2178     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaGovernanceScript.sol#2178
Severity: Low
2178     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaGovernanceScript.sol#2178
Severity: Low
2178     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaGovernanceScript.sol#2179
Severity: Low
2179       _initializeRole(roleDescriptions[i]);



LlamaGovernanceScript.sol#2179
Severity: Low
2179       _initializeRole(roleDescriptions[i]);



LlamaGovernanceScript.sol#2771
Severity: Low
2771   error UnauthorizedCaller();



LlamaGovernanceScript.sol#2771
Severity: Low
2771   error UnauthorizedCaller();



LlamaGovernanceScript.sol#2861
Severity: Low
2861   error InvalidDeployConfiguration();



LlamaGovernanceScript.sol#2861
Severity: Low
2861   error InvalidDeployConfiguration();



LlamaGovernanceScript.sol#2864
Severity: Low
2864   error OnlyRootLlama();



LlamaGovernanceScript.sol#2864
Severity: Low
2864   error OnlyRootLlama();



LlamaGovernanceScript.sol#3137
Severity: Low
3137   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaGovernanceScript.sol#3137
Severity: Low
3137   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaGovernanceScript.sol#3137
Severity: Low
3137   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaGovernanceScript.sol#3140
Severity: Low
3140   error CannotSetExecutorAsTarget();



LlamaGovernanceScript.sol#3140
Severity: Low
3140   error CannotSetExecutorAsTarget();



LlamaGovernanceScript.sol#3143
Severity: Low
3143   error RestrictedAddress();



LlamaGovernanceScript.sol#3143
Severity: Low
3143   error RestrictedAddress();



LlamaGovernanceScript.sol#3146
Severity: Low
3146   error DuplicateCast();



LlamaGovernanceScript.sol#3146
Severity: Low
3146   error DuplicateCast();



LlamaGovernanceScript.sol#3150
Severity: Low
3150   error FailedActionExecution(bytes reason);



LlamaGovernanceScript.sol#3150
Severity: Low
3150   error FailedActionExecution(bytes reason);



LlamaGovernanceScript.sol#3153
Severity: Low
3153   error InfoHashMismatch();



LlamaGovernanceScript.sol#3153
Severity: Low
3153   error InfoHashMismatch();



LlamaGovernanceScript.sol#3156
Severity: Low
3156   error IncorrectMsgValue();



LlamaGovernanceScript.sol#3156
Severity: Low
3156   error IncorrectMsgValue();



LlamaGovernanceScript.sol#3160
Severity: Low
3160   error InvalidActionState(ActionState current);



LlamaGovernanceScript.sol#3160
Severity: Low
3160   error InvalidActionState(ActionState current);



LlamaGovernanceScript.sol#3163
Severity: Low
3163   error InvalidPolicyholder();



LlamaGovernanceScript.sol#3163
Severity: Low
3163   error InvalidPolicyholder();



LlamaGovernanceScript.sol#3166
Severity: Low
3166   error InvalidSignature();



LlamaGovernanceScript.sol#3166
Severity: Low
3166   error InvalidSignature();



LlamaGovernanceScript.sol#3169
Severity: Low
3169   error InvalidStrategy();



LlamaGovernanceScript.sol#3169
Severity: Low
3169   error InvalidStrategy();



LlamaGovernanceScript.sol#3172
Severity: Low
3172   error MinExecutionTimeCannotBeInThePast();



LlamaGovernanceScript.sol#3172
Severity: Low
3172   error MinExecutionTimeCannotBeInThePast();



LlamaGovernanceScript.sol#3175
Severity: Low
3175   error OnlyLlama();



LlamaGovernanceScript.sol#3175
Severity: Low
3175   error OnlyLlama();



LlamaGovernanceScript.sol#3178
Severity: Low
3178   error PolicyholderDoesNotHavePermission();



LlamaGovernanceScript.sol#3178
Severity: Low
3178   error PolicyholderDoesNotHavePermission();



LlamaGovernanceScript.sol#3181
Severity: Low
3181   error MinExecutionTimeNotReached();



LlamaGovernanceScript.sol#3181
Severity: Low
3181   error MinExecutionTimeNotReached();



LlamaGovernanceScript.sol#3184
Severity: Low
3184   error UnauthorizedStrategyLogic();



LlamaGovernanceScript.sol#3184
Severity: Low
3184   error UnauthorizedStrategyLogic();



LlamaGovernanceScript.sol#3187
Severity: Low
3187   error UnauthorizedAccountLogic();



LlamaGovernanceScript.sol#3187
Severity: Low
3187   error UnauthorizedAccountLogic();



LlamaGovernanceScript.sol#3338
Severity: Low
3338     bytes[] calldata initialStrategies,



LlamaGovernanceScript.sol#3339
Severity: Low
3339     bytes[] calldata initialAccounts



LlamaGovernanceScript.sol#3340
Severity: Low
3340   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaGovernanceScript.sol#3342
Severity: Low
3342     name = _name;



LlamaGovernanceScript.sol#3343
Severity: Low
3343     executor = new LlamaExecutor();



LlamaGovernanceScript.sol#3343
Severity: Low
3343     executor = new LlamaExecutor();



LlamaGovernanceScript.sol#3343
Severity: Low
3343     executor = new LlamaExecutor();



LlamaGovernanceScript.sol#3346
Severity: Low
3346     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaGovernanceScript.sol#3347
Severity: Low
3347     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaGovernanceScript.sol#3347
Severity: Low
3347     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaGovernanceScript.sol#3350
Severity: Low
3350     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaGovernanceScript.sol#3351
Severity: Low
3351     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaGovernanceScript.sol#3351
Severity: Low
3351     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaGovernanceScript.sol#3351
Severity: Low
3351     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaGovernanceScript.sol#3351
Severity: Low
3351     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaGovernanceScript.sol#3351
Severity: Low
3351     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaGovernanceScript.sol#3351
Severity: Low
3351     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaGovernanceScript.sol#4049
Severity: Low
4049   error CallReverted(uint256 index, bytes revertData);



LlamaGovernanceScript.sol#4049
Severity: Low
4049   error CallReverted(uint256 index, bytes revertData);



LlamaGovernanceScript.sol#4049
Severity: Low
4049   error CallReverted(uint256 index, bytes revertData);



LlamaGovernanceScript.sol#4052
Severity: Low
4052   error MismatchedArrayLengths();



LlamaGovernanceScript.sol#4052
Severity: Low
4052   error MismatchedArrayLengths();



LlamaGovernanceScript.sol#4056
Severity: Low
4056   error UnauthorizedTarget(address target);



LlamaGovernanceScript.sol#4056
Severity: Low
4056   error UnauthorizedTarget(address target);



LlamaGovernanceScript.sol#4106
Severity: Low
4106     RoleHolderData[] calldata _setRoleHolders,



LlamaGovernanceScript.sol#4107
Severity: Low
4107     RolePermissionData[] calldata _setRolePermissions



LlamaGovernanceScript.sol#4108
Severity: Low
4108   ) external onlyDelegateCall {



LlamaGovernanceScript.sol#4109
Severity: Low
4109     initializeRoles(description);



LlamaGovernanceScript.sol#4110
Severity: Low
4110     setRoleHolders(_setRoleHolders);



LlamaGovernanceScript.sol#4111
Severity: Low
4111     setRolePermissions(_setRolePermissions);



```

### LlamaPolicy.sol

```

LlamaPolicy.sol#1946
Severity: Low
1946   constructor() {



LlamaPolicy.sol#2220
Severity: Low
2220   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaPolicy.sol#2344
Severity: Low
2344   constructor(



LlamaPolicy.sol#2728
Severity: Low
2728   constructor() {



LlamaPolicy.sol#2740
Severity: Low
2740   function initialize(



LlamaPolicy.sol#3591
Severity: Low
3591   constructor() {



LlamaPolicy.sol#3600
Severity: Low
3600   function initialize(



LlamaPolicy.sol#13
Severity: Low
13     error HexLengthInsufficient();



LlamaPolicy.sol#13
Severity: Low
13     error HexLengthInsufficient();



LlamaPolicy.sol#1112
Severity: Low
1112   error UnsafeCast(uint256 n);



LlamaPolicy.sol#1112
Severity: Low
1112   error UnsafeCast(uint256 n);



LlamaPolicy.sol#1483
Severity: Low
1483     error AlreadyInitialized();



LlamaPolicy.sol#1483
Severity: Low
1483     error AlreadyInitialized();



LlamaPolicy.sol#1488
Severity: Low
1488     error NotInitializing();



LlamaPolicy.sol#1488
Severity: Low
1488     error NotInitializing();



LlamaPolicy.sol#1804
Severity: Low
1804     error ERC1167FailedCreateClone();



LlamaPolicy.sol#1804
Severity: Low
1804     error ERC1167FailedCreateClone();



LlamaPolicy.sol#1940
Severity: Low
1940   error OnlyLlamaCore();



LlamaPolicy.sol#1940
Severity: Low
1940   error OnlyLlamaCore();



LlamaPolicy.sol#2178
Severity: Low
2178   error UnauthorizedCaller();



LlamaPolicy.sol#2178
Severity: Low
2178   error UnauthorizedCaller();



LlamaPolicy.sol#2268
Severity: Low
2268   error InvalidDeployConfiguration();



LlamaPolicy.sol#2268
Severity: Low
2268   error InvalidDeployConfiguration();



LlamaPolicy.sol#2271
Severity: Low
2271   error OnlyRootLlama();



LlamaPolicy.sol#2271
Severity: Low
2271   error OnlyRootLlama();



LlamaPolicy.sol#2544
Severity: Low
2544   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaPolicy.sol#2544
Severity: Low
2544   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaPolicy.sol#2544
Severity: Low
2544   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaPolicy.sol#2547
Severity: Low
2547   error CannotSetExecutorAsTarget();



LlamaPolicy.sol#2547
Severity: Low
2547   error CannotSetExecutorAsTarget();



LlamaPolicy.sol#2550
Severity: Low
2550   error RestrictedAddress();



LlamaPolicy.sol#2550
Severity: Low
2550   error RestrictedAddress();



LlamaPolicy.sol#2553
Severity: Low
2553   error DuplicateCast();



LlamaPolicy.sol#2553
Severity: Low
2553   error DuplicateCast();



LlamaPolicy.sol#2557
Severity: Low
2557   error FailedActionExecution(bytes reason);



LlamaPolicy.sol#2557
Severity: Low
2557   error FailedActionExecution(bytes reason);



LlamaPolicy.sol#2560
Severity: Low
2560   error InfoHashMismatch();



LlamaPolicy.sol#2560
Severity: Low
2560   error InfoHashMismatch();



LlamaPolicy.sol#2563
Severity: Low
2563   error IncorrectMsgValue();



LlamaPolicy.sol#2563
Severity: Low
2563   error IncorrectMsgValue();



LlamaPolicy.sol#2567
Severity: Low
2567   error InvalidActionState(ActionState current);



LlamaPolicy.sol#2567
Severity: Low
2567   error InvalidActionState(ActionState current);



LlamaPolicy.sol#2570
Severity: Low
2570   error InvalidPolicyholder();



LlamaPolicy.sol#2570
Severity: Low
2570   error InvalidPolicyholder();



LlamaPolicy.sol#2573
Severity: Low
2573   error InvalidSignature();



LlamaPolicy.sol#2573
Severity: Low
2573   error InvalidSignature();



LlamaPolicy.sol#2576
Severity: Low
2576   error InvalidStrategy();



LlamaPolicy.sol#2576
Severity: Low
2576   error InvalidStrategy();



LlamaPolicy.sol#2579
Severity: Low
2579   error MinExecutionTimeCannotBeInThePast();



LlamaPolicy.sol#2579
Severity: Low
2579   error MinExecutionTimeCannotBeInThePast();



LlamaPolicy.sol#2582
Severity: Low
2582   error OnlyLlama();



LlamaPolicy.sol#2582
Severity: Low
2582   error OnlyLlama();



LlamaPolicy.sol#2585
Severity: Low
2585   error PolicyholderDoesNotHavePermission();



LlamaPolicy.sol#2585
Severity: Low
2585   error PolicyholderDoesNotHavePermission();



LlamaPolicy.sol#2588
Severity: Low
2588   error MinExecutionTimeNotReached();



LlamaPolicy.sol#2588
Severity: Low
2588   error MinExecutionTimeNotReached();



LlamaPolicy.sol#2591
Severity: Low
2591   error UnauthorizedStrategyLogic();



LlamaPolicy.sol#2591
Severity: Low
2591   error UnauthorizedStrategyLogic();



LlamaPolicy.sol#2594
Severity: Low
2594   error UnauthorizedAccountLogic();



LlamaPolicy.sol#2594
Severity: Low
2594   error UnauthorizedAccountLogic();



LlamaPolicy.sol#2745
Severity: Low
2745     bytes[] calldata initialStrategies,



LlamaPolicy.sol#2746
Severity: Low
2746     bytes[] calldata initialAccounts



LlamaPolicy.sol#2747
Severity: Low
2747   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaPolicy.sol#2749
Severity: Low
2749     name = _name;



LlamaPolicy.sol#2750
Severity: Low
2750     executor = new LlamaExecutor();



LlamaPolicy.sol#2750
Severity: Low
2750     executor = new LlamaExecutor();



LlamaPolicy.sol#2750
Severity: Low
2750     executor = new LlamaExecutor();



LlamaPolicy.sol#2753
Severity: Low
2753     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaPolicy.sol#2754
Severity: Low
2754     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaPolicy.sol#2754
Severity: Low
2754     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaPolicy.sol#2757
Severity: Low
2757     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaPolicy.sol#2758
Severity: Low
2758     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaPolicy.sol#2758
Severity: Low
2758     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaPolicy.sol#2758
Severity: Low
2758     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaPolicy.sol#2758
Severity: Low
2758     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaPolicy.sol#2758
Severity: Low
2758     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaPolicy.sol#2758
Severity: Low
2758     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaPolicy.sol#3496
Severity: Low
3496   error ActionCreationAtSameTimestamp();



LlamaPolicy.sol#3496
Severity: Low
3496   error ActionCreationAtSameTimestamp();



LlamaPolicy.sol#3500
Severity: Low
3500   error AddressDoesNotHoldPolicy(address userAddress);



LlamaPolicy.sol#3500
Severity: Low
3500   error AddressDoesNotHoldPolicy(address userAddress);



LlamaPolicy.sol#3503
Severity: Low
3503   error AllHoldersRole();



LlamaPolicy.sol#3503
Severity: Low
3503   error AllHoldersRole();



LlamaPolicy.sol#3510
Severity: Low
3510   error InvalidIndices();



LlamaPolicy.sol#3510
Severity: Low
3510   error InvalidIndices();



LlamaPolicy.sol#3513
Severity: Low
3513   error InvalidRoleHolderInput();



LlamaPolicy.sol#3513
Severity: Low
3513   error InvalidRoleHolderInput();



LlamaPolicy.sol#3516
Severity: Low
3516   error NonTransferableToken();



LlamaPolicy.sol#3516
Severity: Low
3516   error NonTransferableToken();



LlamaPolicy.sol#3519
Severity: Low
3519   error OnlyLlama();



LlamaPolicy.sol#3519
Severity: Low
3519   error OnlyLlama();



LlamaPolicy.sol#3522
Severity: Low
3522   error RoleNotInitialized(uint8 role);



LlamaPolicy.sol#3522
Severity: Low
3522   error RoleNotInitialized(uint8 role);



LlamaPolicy.sol#3602
Severity: Low
3602     RoleDescription[] calldata roleDescriptions,



LlamaPolicy.sol#3603
Severity: Low
3603     RoleHolderData[] calldata roleHolders,



LlamaPolicy.sol#3604
Severity: Low
3604     RolePermissionData[] calldata rolePermissions



LlamaPolicy.sol#3606
Severity: Low
3606     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaPolicy.sol#3606
Severity: Low
3606     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaPolicy.sol#3606
Severity: Low
3606     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaPolicy.sol#3606
Severity: Low
3606     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaPolicy.sol#3606
Severity: Low
3606     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaPolicy.sol#3607
Severity: Low
3607     factory = LlamaFactory(msg.sender);



LlamaPolicy.sol#3607
Severity: Low
3607     factory = LlamaFactory(msg.sender);



LlamaPolicy.sol#3608
Severity: Low
3608     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaPolicy.sol#3608
Severity: Low
3608     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaPolicy.sol#3608
Severity: Low
3608     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaPolicy.sol#3609
Severity: Low
3609       _initializeRole(roleDescriptions[i]);



LlamaPolicy.sol#3609
Severity: Low
3609       _initializeRole(roleDescriptions[i]);



```

### LlamaPolicyMetadata.sol

```

LlamaPolicyMetadata.sol#101
Severity: Low
101     error HexLengthInsufficient();



LlamaPolicyMetadata.sol#101
Severity: Low
101     error HexLengthInsufficient();



```

### LlamaPolicyMetadataParamRegistry.sol

```

LlamaPolicyMetadataParamRegistry.sol#15
Severity: Low
15   constructor() {



LlamaPolicyMetadataParamRegistry.sol#89
Severity: Low
89   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaPolicyMetadataParamRegistry.sol#9
Severity: Low
9   error OnlyLlamaCore();



LlamaPolicyMetadataParamRegistry.sol#9
Severity: Low
9   error OnlyLlamaCore();



LlamaPolicyMetadataParamRegistry.sol#47
Severity: Low
47   error UnauthorizedCaller();



LlamaPolicyMetadataParamRegistry.sol#47
Severity: Low
47   error UnauthorizedCaller();



```

### LlamaRelativeQuorum.sol

```

LlamaRelativeQuorum.sol#674
Severity: Low
674   constructor() {



LlamaRelativeQuorum.sol#2393
Severity: Low
2393   constructor() {



LlamaRelativeQuorum.sol#2402
Severity: Low
2402   function initialize(



LlamaRelativeQuorum.sol#3045
Severity: Low
3045   constructor(LlamaExecutor rootLlamaExecutor) {



LlamaRelativeQuorum.sol#3169
Severity: Low
3169   constructor(



LlamaRelativeQuorum.sol#3553
Severity: Low
3553   constructor() {



LlamaRelativeQuorum.sol#3565
Severity: Low
3565   function initialize(



LlamaRelativeQuorum.sol#4378
Severity: Low
4378   constructor() {



LlamaRelativeQuorum.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaRelativeQuorum.sol#70
Severity: Low
70     error AlreadyInitialized();



LlamaRelativeQuorum.sol#75
Severity: Low
75     error NotInitializing();



LlamaRelativeQuorum.sol#75
Severity: Low
75     error NotInitializing();



LlamaRelativeQuorum.sol#507
Severity: Low
507     error ERC1167FailedCreateClone();



LlamaRelativeQuorum.sol#507
Severity: Low
507     error ERC1167FailedCreateClone();



LlamaRelativeQuorum.sol#641
Severity: Low
641   error UnsafeCast(uint256 n);



LlamaRelativeQuorum.sol#641
Severity: Low
641   error UnsafeCast(uint256 n);



LlamaRelativeQuorum.sol#668
Severity: Low
668   error OnlyLlamaCore();



LlamaRelativeQuorum.sol#668
Severity: Low
668   error OnlyLlamaCore();



LlamaRelativeQuorum.sol#709
Severity: Low
709     error HexLengthInsufficient();



LlamaRelativeQuorum.sol#709
Severity: Low
709     error HexLengthInsufficient();



LlamaRelativeQuorum.sol#2298
Severity: Low
2298   error ActionCreationAtSameTimestamp();



LlamaRelativeQuorum.sol#2298
Severity: Low
2298   error ActionCreationAtSameTimestamp();



LlamaRelativeQuorum.sol#2302
Severity: Low
2302   error AddressDoesNotHoldPolicy(address userAddress);



LlamaRelativeQuorum.sol#2302
Severity: Low
2302   error AddressDoesNotHoldPolicy(address userAddress);



LlamaRelativeQuorum.sol#2305
Severity: Low
2305   error AllHoldersRole();



LlamaRelativeQuorum.sol#2305
Severity: Low
2305   error AllHoldersRole();



LlamaRelativeQuorum.sol#2312
Severity: Low
2312   error InvalidIndices();



LlamaRelativeQuorum.sol#2312
Severity: Low
2312   error InvalidIndices();



LlamaRelativeQuorum.sol#2315
Severity: Low
2315   error InvalidRoleHolderInput();



LlamaRelativeQuorum.sol#2315
Severity: Low
2315   error InvalidRoleHolderInput();



LlamaRelativeQuorum.sol#2318
Severity: Low
2318   error NonTransferableToken();



LlamaRelativeQuorum.sol#2318
Severity: Low
2318   error NonTransferableToken();



LlamaRelativeQuorum.sol#2321
Severity: Low
2321   error OnlyLlama();



LlamaRelativeQuorum.sol#2321
Severity: Low
2321   error OnlyLlama();



LlamaRelativeQuorum.sol#2324
Severity: Low
2324   error RoleNotInitialized(uint8 role);



LlamaRelativeQuorum.sol#2324
Severity: Low
2324   error RoleNotInitialized(uint8 role);



LlamaRelativeQuorum.sol#2404
Severity: Low
2404     RoleDescription[] calldata roleDescriptions,



LlamaRelativeQuorum.sol#2405
Severity: Low
2405     RoleHolderData[] calldata roleHolders,



LlamaRelativeQuorum.sol#2406
Severity: Low
2406     RolePermissionData[] calldata rolePermissions



LlamaRelativeQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaRelativeQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaRelativeQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaRelativeQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaRelativeQuorum.sol#2408
Severity: Low
2408     __initializeERC721MinimalProxy(_name, string.concat("LL-", LibString.replace(LibString.upper(_name), " ", "-")));



LlamaRelativeQuorum.sol#2409
Severity: Low
2409     factory = LlamaFactory(msg.sender);



LlamaRelativeQuorum.sol#2409
Severity: Low
2409     factory = LlamaFactory(msg.sender);



LlamaRelativeQuorum.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaRelativeQuorum.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaRelativeQuorum.sol#2410
Severity: Low
2410     for (uint256 i = 0; i < roleDescriptions.length; i = LlamaUtils.uncheckedIncrement(i)) {



LlamaRelativeQuorum.sol#2411
Severity: Low
2411       _initializeRole(roleDescriptions[i]);



LlamaRelativeQuorum.sol#2411
Severity: Low
2411       _initializeRole(roleDescriptions[i]);



LlamaRelativeQuorum.sol#3003
Severity: Low
3003   error UnauthorizedCaller();



LlamaRelativeQuorum.sol#3003
Severity: Low
3003   error UnauthorizedCaller();



LlamaRelativeQuorum.sol#3093
Severity: Low
3093   error InvalidDeployConfiguration();



LlamaRelativeQuorum.sol#3093
Severity: Low
3093   error InvalidDeployConfiguration();



LlamaRelativeQuorum.sol#3096
Severity: Low
3096   error OnlyRootLlama();



LlamaRelativeQuorum.sol#3096
Severity: Low
3096   error OnlyRootLlama();



LlamaRelativeQuorum.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaRelativeQuorum.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaRelativeQuorum.sol#3369
Severity: Low
3369   error CannotCastWithZeroQuantity(address policyholder, uint8 role);



LlamaRelativeQuorum.sol#3372
Severity: Low
3372   error CannotSetExecutorAsTarget();



LlamaRelativeQuorum.sol#3372
Severity: Low
3372   error CannotSetExecutorAsTarget();



LlamaRelativeQuorum.sol#3375
Severity: Low
3375   error RestrictedAddress();



LlamaRelativeQuorum.sol#3375
Severity: Low
3375   error RestrictedAddress();



LlamaRelativeQuorum.sol#3378
Severity: Low
3378   error DuplicateCast();



LlamaRelativeQuorum.sol#3378
Severity: Low
3378   error DuplicateCast();



LlamaRelativeQuorum.sol#3382
Severity: Low
3382   error FailedActionExecution(bytes reason);



LlamaRelativeQuorum.sol#3382
Severity: Low
3382   error FailedActionExecution(bytes reason);



LlamaRelativeQuorum.sol#3385
Severity: Low
3385   error InfoHashMismatch();



LlamaRelativeQuorum.sol#3385
Severity: Low
3385   error InfoHashMismatch();



LlamaRelativeQuorum.sol#3388
Severity: Low
3388   error IncorrectMsgValue();



LlamaRelativeQuorum.sol#3388
Severity: Low
3388   error IncorrectMsgValue();



LlamaRelativeQuorum.sol#3392
Severity: Low
3392   error InvalidActionState(ActionState current);



LlamaRelativeQuorum.sol#3392
Severity: Low
3392   error InvalidActionState(ActionState current);



LlamaRelativeQuorum.sol#3395
Severity: Low
3395   error InvalidPolicyholder();



LlamaRelativeQuorum.sol#3395
Severity: Low
3395   error InvalidPolicyholder();



LlamaRelativeQuorum.sol#3398
Severity: Low
3398   error InvalidSignature();



LlamaRelativeQuorum.sol#3398
Severity: Low
3398   error InvalidSignature();



LlamaRelativeQuorum.sol#3401
Severity: Low
3401   error InvalidStrategy();



LlamaRelativeQuorum.sol#3401
Severity: Low
3401   error InvalidStrategy();



LlamaRelativeQuorum.sol#3404
Severity: Low
3404   error MinExecutionTimeCannotBeInThePast();



LlamaRelativeQuorum.sol#3404
Severity: Low
3404   error MinExecutionTimeCannotBeInThePast();



LlamaRelativeQuorum.sol#3407
Severity: Low
3407   error OnlyLlama();



LlamaRelativeQuorum.sol#3407
Severity: Low
3407   error OnlyLlama();



LlamaRelativeQuorum.sol#3410
Severity: Low
3410   error PolicyholderDoesNotHavePermission();



LlamaRelativeQuorum.sol#3410
Severity: Low
3410   error PolicyholderDoesNotHavePermission();



LlamaRelativeQuorum.sol#3413
Severity: Low
3413   error MinExecutionTimeNotReached();



LlamaRelativeQuorum.sol#3413
Severity: Low
3413   error MinExecutionTimeNotReached();



LlamaRelativeQuorum.sol#3416
Severity: Low
3416   error UnauthorizedStrategyLogic();



LlamaRelativeQuorum.sol#3416
Severity: Low
3416   error UnauthorizedStrategyLogic();



LlamaRelativeQuorum.sol#3419
Severity: Low
3419   error UnauthorizedAccountLogic();



LlamaRelativeQuorum.sol#3419
Severity: Low
3419   error UnauthorizedAccountLogic();



LlamaRelativeQuorum.sol#3570
Severity: Low
3570     bytes[] calldata initialStrategies,



LlamaRelativeQuorum.sol#3571
Severity: Low
3571     bytes[] calldata initialAccounts



LlamaRelativeQuorum.sol#3572
Severity: Low
3572   ) external initializer returns (bytes32 bootstrapPermissionId) {



LlamaRelativeQuorum.sol#3574
Severity: Low
3574     name = _name;



LlamaRelativeQuorum.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaRelativeQuorum.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaRelativeQuorum.sol#3575
Severity: Low
3575     executor = new LlamaExecutor();



LlamaRelativeQuorum.sol#3578
Severity: Low
3578     ILlamaStrategy bootstrapStrategy = _deployStrategies(_llamaStrategyLogic, initialStrategies);



LlamaRelativeQuorum.sol#3579
Severity: Low
3579     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaRelativeQuorum.sol#3579
Severity: Low
3579     _deployAccounts(_llamaAccountLogic, initialAccounts);



LlamaRelativeQuorum.sol#3582
Severity: Low
3582     bytes4 selector = LlamaPolicy.setRolePermission.selector;



LlamaRelativeQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaRelativeQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaRelativeQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaRelativeQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaRelativeQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaRelativeQuorum.sol#3583
Severity: Low
3583     return keccak256(abi.encode(PermissionData(address(policy), bytes4(selector), bootstrapStrategy)));



LlamaRelativeQuorum.sol#4278
Severity: Low
4278   error CannotCancelInState(ActionState currentState);



LlamaRelativeQuorum.sol#4278
Severity: Low
4278   error CannotCancelInState(ActionState currentState);



LlamaRelativeQuorum.sol#4281
Severity: Low
4281   error DisapprovalDisabled();



LlamaRelativeQuorum.sol#4281
Severity: Low
4281   error DisapprovalDisabled();



LlamaRelativeQuorum.sol#4285
Severity: Low
4285   error InvalidMinApprovalPct(uint256 minApprovalPct);



LlamaRelativeQuorum.sol#4285
Severity: Low
4285   error InvalidMinApprovalPct(uint256 minApprovalPct);



LlamaRelativeQuorum.sol#4289
Severity: Low
4289   error InvalidRole(uint8 role);



LlamaRelativeQuorum.sol#4289
Severity: Low
4289   error InvalidRole(uint8 role);



LlamaRelativeQuorum.sol#4292
Severity: Low
4292   error OnlyActionCreator();



LlamaRelativeQuorum.sol#4292
Severity: Low
4292   error OnlyActionCreator();



LlamaRelativeQuorum.sol#4296
Severity: Low
4296   error RoleHasZeroSupply(uint8 role);



LlamaRelativeQuorum.sol#4296
Severity: Low
4296   error RoleHasZeroSupply(uint8 role);



LlamaRelativeQuorum.sol#4300
Severity: Low
4300   error RoleNotInitialized(uint8 role);



LlamaRelativeQuorum.sol#4300
Severity: Low
4300   error RoleNotInitialized(uint8 role);



```

## SOLIDITY_PRAGMAS_VERSION
Solidity source files indicate the versions of the compiler they can be compiled with.

pragma solidity ^0.4.17; // bad: compiles w 0.4.17 and above
pragma solidity 0.4.24; // good : compiles w 0.4.24 only

It is recommended to follow the latter example, as future compiler versions may handle certain language constructions in a way the developer did not foresee.


### LlamaGovernanceScript.sol

```

LlamaGovernanceScript.sol#2
Severity: Low
2 pragma solidity ^0.8.19;



```
