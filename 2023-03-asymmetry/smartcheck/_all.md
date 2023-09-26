
# SMARTCHECK ANALYSIS

## SOLIDITY_ADDRESS_HARDCODED
The contract contains unknown address. This address might be used for some malicious activity. Please check hardcoded address and it's usage.


### Reth.sol

```

Reth.sol#1277
Severity: Low
1277         0x1d8f8f00cfa6758d7bE78336684788Fb0ee0Fa46;



Reth.sol#1279
Severity: Low
1279         0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2;



Reth.sol#1281
Severity: Low
1281         0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45;



Reth.sol#1283
Severity: Low
1283         0x1F98431c8aD98523631AE4a59f267346ea31F984;



Reth.sol#697
Severity: Low
697         _transferOwnership(address(0));



```

### SafEth.sol

```

SafEth.sol#409
Severity: Low
409         _beforeTokenTransfer(address(0), account, amount);



SafEth.sol#418
Severity: Low
418         _afterTokenTransfer(address(0), account, amount);



SafEth.sol#435
Severity: Low
435         _beforeTokenTransfer(account, address(0), amount);



SafEth.sol#447
Severity: Low
447         _afterTokenTransfer(account, address(0), amount);



SafEth.sol#977
Severity: Low
977         _transferOwnership(address(0));



SafEth.sol#1407
Severity: Low
1407         _beforeTokenTransfer(address(0), account, amount);



SafEth.sol#1413
Severity: Low
1413         _afterTokenTransfer(address(0), account, amount);



SafEth.sol#1430
Severity: Low
1430         _beforeTokenTransfer(account, address(0), amount);



SafEth.sol#1441
Severity: Low
1441         _afterTokenTransfer(account, address(0), amount);



```

### SfrxEth.sol

```

SfrxEth.sol#595
Severity: Low
595         0xac3E018457B222d93114458476f3E3416Abbe38F;



SfrxEth.sol#597
Severity: Low
597         0x5E8422345238F34275888049021821E8E08CAa1f;



SfrxEth.sol#599
Severity: Low
599         0xa1F8A6807c402E4A15ef4EBa36528A3FED24E577;



SfrxEth.sol#601
Severity: Low
601         0xbAFA44EFE7901E04E39Dad13167D089C559c1138;



SfrxEth.sol#461
Severity: Low
461         _transferOwnership(address(0));



```

### WstEth.sol

```

WstEth.sol#1012
Severity: Low
1012         0x7f39C581F595B53c5cb19bD0b3f8dA6c935E2Ca0;



WstEth.sol#1014
Severity: Low
1014         0xDC24316b9AE028F1497c275EB9192a3Ea0f67022;



WstEth.sol#1016
Severity: Low
1016         0xae7ab96520DE3A18E5e111B5EaAb095312D7fE84;



WstEth.sol#445
Severity: Low
445         _transferOwnership(address(0));



WstEth.sol#865
Severity: Low
865         _beforeTokenTransfer(address(0), account, amount);



WstEth.sol#874
Severity: Low
874         _afterTokenTransfer(address(0), account, amount);



WstEth.sol#891
Severity: Low
891         _beforeTokenTransfer(account, address(0), amount);



WstEth.sol#903
Severity: Low
903         _afterTokenTransfer(account, address(0), amount);



```

## SOLIDITY_DIV_MUL
Solidity operates only with integers. Thus, if the division is done before the  multiplication, the rounding errors can increase dramatically.
[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#arithmetic)
Precision issues.


### Reth.sol

```

Reth.sol#1429
Severity: Medium
1429             uint256 minOut = ((((rethPerEth * msg.value) / 10 ** 18) *



```

### SfrxEth.sol

```

SfrxEth.sol#654
Severity: Medium
654         uint256 minOut = (((ethPerDerivative(_amount) * _amount) / 10 ** 18) *



```

## SOLIDITY_LOCKED_MONEY
Contracts programmed to receive ether should implement a way to withdraw it, i.e., call ```transfer``` (recommended), ```send```, or ```call.value``` at least once.


### Reth.sol

```

Reth.sol#1275
Severity: High
1275 contract Reth is IDerivative, Initializable, OwnableUpgradeable {



```

### SafEth.sol

```

SafEth.sol#1541
Severity: High
1541 contract SafEth is



```

### SfrxEth.sol

```

SfrxEth.sol#593
Severity: High
593 contract SfrxEth is IDerivative, Initializable, OwnableUpgradeable {



```

### WstEth.sol

```

WstEth.sol#1010
Severity: High
1010 contract WstEth is IDerivative, Initializable, OwnableUpgradeable {



```

## SOLIDITY_OVERPOWERED_ROLE
This function is callable only from one address. Therefore, the system depends heavily on this address. In this case, there are scenarios that may lead to undesirable consequences for investors, e.g. if the private key of this address becomes compromised.

[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#trust)

Overpowered owner


### Reth.sol

```

Reth.sol#1314
Severity: Medium
1314     function setMaxSlippage(uint256 _slippage) external onlyOwner {



```

### SafEth.sol

```

SafEth.sol#1728
Severity: Medium
1728     function setMaxSlippage(



SafEth.sol#1740
Severity: Medium
1740     function setMinAmount(uint256 _minAmount) external onlyOwner {



SafEth.sol#1749
Severity: Medium
1749     function setMaxAmount(uint256 _maxAmount) external onlyOwner {



SafEth.sol#1758
Severity: Medium
1758     function setPauseStaking(bool _pause) external onlyOwner {



SafEth.sol#1767
Severity: Medium
1767     function setPauseUnstaking(bool _pause) external onlyOwner {



```

### SfrxEth.sol

```

SfrxEth.sol#631
Severity: Medium
631     function setMaxSlippage(uint256 _slippage) external onlyOwner {



```

### WstEth.sol

```

WstEth.sol#1046
Severity: Medium
1046     function setMaxSlippage(uint256 _slippage) external onlyOwner {



```

## SOLIDITY_PRAGMAS_VERSION
Solidity source files indicate the versions of the compiler they can be compiled with.

pragma solidity ^0.4.17; // bad: compiles w 0.4.17 and above
pragma solidity 0.4.24; // good : compiles w 0.4.24 only

It is recommended to follow the latter example, as future compiler versions may handle certain language constructions in a way the developer did not foresee.


### Reth.sol

```

Reth.sol#2
Severity: Low
2 pragma solidity ^0.8.13;



```

### SafEth.sol

```

SafEth.sol#2
Severity: Low
2 pragma solidity ^0.8.13;



```

### SfrxEth.sol

```

SfrxEth.sol#2
Severity: Low
2 pragma solidity ^0.8.13;



```

### WstEth.sol

```

WstEth.sol#2
Severity: Low
2 pragma solidity ^0.8.13;



```

## SOLIDITY_PRIVATE_MODIFIER_DONT_HIDE_DATA
Contrary to a popular misconception, the ```private``` modifier does not make a variable invisible. Miners have access to all contractsâ€™ code and data. Developers must account for the lack of privacy in Ethereum.

[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#privacy)

Privacy.


### Reth.sol

```

Reth.sol#529
Severity: Low
529     uint8 private _initialized;



Reth.sol#534
Severity: Low
534     bool private _initializing;



Reth.sol#636
Severity: Low
636     uint256[50] private __gap;



Reth.sol#652
Severity: Low
652     address private _owner;



Reth.sol#724
Severity: Low
724     uint256[49] private __gap;



```

### SafEth.sol

```

SafEth.sol#183
Severity: Low
183     mapping(address => uint256) private _balances;



SafEth.sol#185
Severity: Low
185     mapping(address => mapping(address => uint256)) private _allowances;



SafEth.sol#187
Severity: Low
187     uint256 private _totalSupply;



SafEth.sol#189
Severity: Low
189     string private _name;



SafEth.sol#190
Severity: Low
190     string private _symbol;



SafEth.sol#809
Severity: Low
809     uint8 private _initialized;



SafEth.sol#814
Severity: Low
814     bool private _initializing;



SafEth.sol#916
Severity: Low
916     uint256[50] private __gap;



SafEth.sol#932
Severity: Low
932     address private _owner;



SafEth.sol#1004
Severity: Low
1004     uint256[49] private __gap;



SafEth.sol#1179
Severity: Low
1179     mapping(address => uint256) private _balances;



SafEth.sol#1181
Severity: Low
1181     mapping(address => mapping(address => uint256)) private _allowances;



SafEth.sol#1183
Severity: Low
1183     uint256 private _totalSupply;



SafEth.sol#1185
Severity: Low
1185     string private _name;



SafEth.sol#1186
Severity: Low
1186     string private _symbol;



SafEth.sol#1536
Severity: Low
1536     uint256[45] private __gap;



```

### SfrxEth.sol

```

SfrxEth.sol#293
Severity: Low
293     uint8 private _initialized;



SfrxEth.sol#298
Severity: Low
298     bool private _initializing;



SfrxEth.sol#400
Severity: Low
400     uint256[50] private __gap;



SfrxEth.sol#416
Severity: Low
416     address private _owner;



SfrxEth.sol#488
Severity: Low
488     uint256[49] private __gap;



```

### WstEth.sol

```

WstEth.sol#277
Severity: Low
277     uint8 private _initialized;



WstEth.sol#282
Severity: Low
282     bool private _initializing;



WstEth.sol#384
Severity: Low
384     uint256[50] private __gap;



WstEth.sol#400
Severity: Low
400     address private _owner;



WstEth.sol#472
Severity: Low
472     uint256[49] private __gap;



WstEth.sol#639
Severity: Low
639     mapping(address => uint256) private _balances;



WstEth.sol#641
Severity: Low
641     mapping(address => mapping(address => uint256)) private _allowances;



WstEth.sol#643
Severity: Low
643     uint256 private _totalSupply;



WstEth.sol#645
Severity: Low
645     string private _name;



WstEth.sol#646
Severity: Low
646     string private _symbol;



```

## SOLIDITY_SHOULD_RETURN_STRUCT
Consider using struct instead of multiple return values for ```internal``` or ```private``` functions. It can improve code readability.


### Reth.sol

```

Reth.sol#856
Severity: Low
856         returns (



Reth.sol#879
Severity: Low
879         returns (uint128 token0, uint128 token1);



Reth.sol#904
Severity: Low
904         returns (



Reth.sol#930
Severity: Low
930         returns (



Reth.sol#951
Severity: Low
951         returns (



Reth.sol#978
Severity: Low
978         returns (



Reth.sol#998
Severity: Low
998         returns (



Reth.sol#1030
Severity: Low
1030     ) external returns (uint256 amount0, uint256 amount1);



Reth.sol#1050
Severity: Low
1050     ) external returns (uint128 amount0, uint128 amount1);



Reth.sol#1064
Severity: Low
1064     ) external returns (uint256 amount0, uint256 amount1);



Reth.sol#1082
Severity: Low
1082     ) external returns (int256 amount0, int256 amount1);



Reth.sol#1126
Severity: Low
1126     ) external returns (uint128 amount0, uint128 amount1);



```

## SOLIDITY_UPGRADE_TO_050
Prepare your code for Solidity 0.5.0 release.


### Reth.sol

```

Reth.sol#627
Severity: Low
627     function _msgData() internal view virtual returns (bytes calldata) {



```

### SafEth.sol

```

SafEth.sol#152
Severity: Low
152     function _msgData() internal view virtual returns (bytes calldata) {



SafEth.sol#907
Severity: Low
907     function _msgData() internal view virtual returns (bytes calldata) {



```

### SfrxEth.sol

```

SfrxEth.sol#391
Severity: Low
391     function _msgData() internal view virtual returns (bytes calldata) {



```

### WstEth.sol

```

WstEth.sol#375
Severity: Low
375     function _msgData() internal view virtual returns (bytes calldata) {



WstEth.sol#608
Severity: Low
608     function _msgData() internal view virtual returns (bytes calldata) {



```

## SOLIDITY_VISIBILITY
The default function visibility level in contracts is ```public```, in interfaces - ```external```, state variable default visibility level is ```internal```.

In contracts, the fallback function can be ```external``` or ```public```. In interfaces, all the functions should be declared as ```external```. Explicitly define function visibility to prevent confusion.


### Reth.sol

```

Reth.sol#338
Severity: Low
338     function sendValue(address payable recipient, uint256 amount) internal {



Reth.sol#1289
Severity: Low
1289     constructor() {



Reth.sol#338
Severity: Low
338     function sendValue(address payable recipient, uint256 amount) internal {



Reth.sol#338
Severity: Low
338     function sendValue(address payable recipient, uint256 amount) internal {



Reth.sol#339
Severity: Low
339         require(address(this).balance >= amount, "Address: insufficient balance");



Reth.sol#339
Severity: Low
339         require(address(this).balance >= amount, "Address: insufficient balance");



Reth.sol#339
Severity: Low
339         require(address(this).balance >= amount, "Address: insufficient balance");



Reth.sol#339
Severity: Low
339         require(address(this).balance >= amount, "Address: insufficient balance");



Reth.sol#341
Severity: Low
341         (bool success, ) = recipient.call{value: amount}("");



Reth.sol#341
Severity: Low
341         (bool success, ) = recipient.call{value: amount}("");



Reth.sol#341
Severity: Low
341         (bool success, ) = recipient.call{value: amount}("");



Reth.sol#1500
Severity: Low
1500     receive() external payable {}



```

### SafEth.sol

```

SafEth.sol#201
Severity: Low
201     constructor(string memory name_, string memory symbol_) {



SafEth.sol#618
Severity: Low
618     function sendValue(address payable recipient, uint256 amount) internal {



SafEth.sol#1564
Severity: Low
1564     constructor() {



SafEth.sol#618
Severity: Low
618     function sendValue(address payable recipient, uint256 amount) internal {



SafEth.sol#618
Severity: Low
618     function sendValue(address payable recipient, uint256 amount) internal {



SafEth.sol#619
Severity: Low
619         require(address(this).balance >= amount, "Address: insufficient balance");



SafEth.sol#619
Severity: Low
619         require(address(this).balance >= amount, "Address: insufficient balance");



SafEth.sol#619
Severity: Low
619         require(address(this).balance >= amount, "Address: insufficient balance");



SafEth.sol#619
Severity: Low
619         require(address(this).balance >= amount, "Address: insufficient balance");



SafEth.sol#621
Severity: Low
621         (bool success, ) = recipient.call{value: amount}("");



SafEth.sol#621
Severity: Low
621         (bool success, ) = recipient.call{value: amount}("");



SafEth.sol#621
Severity: Low
621         (bool success, ) = recipient.call{value: amount}("");



SafEth.sol#1772
Severity: Low
1772     receive() external payable {}



```

### SfrxEth.sol

```

SfrxEth.sol#102
Severity: Low
102     function sendValue(address payable recipient, uint256 amount) internal {



SfrxEth.sol#607
Severity: Low
607     constructor() {



SfrxEth.sol#102
Severity: Low
102     function sendValue(address payable recipient, uint256 amount) internal {



SfrxEth.sol#102
Severity: Low
102     function sendValue(address payable recipient, uint256 amount) internal {



SfrxEth.sol#103
Severity: Low
103         require(address(this).balance >= amount, "Address: insufficient balance");



SfrxEth.sol#103
Severity: Low
103         require(address(this).balance >= amount, "Address: insufficient balance");



SfrxEth.sol#103
Severity: Low
103         require(address(this).balance >= amount, "Address: insufficient balance");



SfrxEth.sol#103
Severity: Low
103         require(address(this).balance >= amount, "Address: insufficient balance");



SfrxEth.sol#105
Severity: Low
105         (bool success, ) = recipient.call{value: amount}("");



SfrxEth.sol#105
Severity: Low
105         (bool success, ) = recipient.call{value: amount}("");



SfrxEth.sol#105
Severity: Low
105         (bool success, ) = recipient.call{value: amount}("");



SfrxEth.sol#706
Severity: Low
706     receive() external payable {}



```

### WstEth.sol

```

WstEth.sol#86
Severity: Low
86     function sendValue(address payable recipient, uint256 amount) internal {



WstEth.sol#657
Severity: Low
657     constructor(string memory name_, string memory symbol_) {



WstEth.sol#1022
Severity: Low
1022     constructor() {



WstEth.sol#86
Severity: Low
86     function sendValue(address payable recipient, uint256 amount) internal {



WstEth.sol#86
Severity: Low
86     function sendValue(address payable recipient, uint256 amount) internal {



WstEth.sol#87
Severity: Low
87         require(address(this).balance >= amount, "Address: insufficient balance");



WstEth.sol#87
Severity: Low
87         require(address(this).balance >= amount, "Address: insufficient balance");



WstEth.sol#87
Severity: Low
87         require(address(this).balance >= amount, "Address: insufficient balance");



WstEth.sol#87
Severity: Low
87         require(address(this).balance >= amount, "Address: insufficient balance");



WstEth.sol#89
Severity: Low
89         (bool success, ) = recipient.call{value: amount}("");



WstEth.sol#89
Severity: Low
89         (bool success, ) = recipient.call{value: amount}("");



WstEth.sol#89
Severity: Low
89         (bool success, ) = recipient.call{value: amount}("");



WstEth.sol#1095
Severity: Low
1095     receive() external payable {}



```

## SOLIDITY_ERC20_APPROVE
The ```approve``` function of ERC-20 is vulnerable. Using front-running attack one can spend approved tokens before change of ```allowance``` value.


### SafEth.sol

```

SafEth.sol#283
Severity: Medium
283     function approve(address spender, uint256 amount) public virtual override returns (bool) {



SafEth.sol#1283
Severity: Medium
1283     function approve(address spender, uint256 amount) public virtual override returns (bool) {



```

### WstEth.sol

```

WstEth.sol#739
Severity: Medium
739     function approve(address spender, uint256 amount) public virtual override returns (bool) {



```
