
# SLITHER ANALYSIS

## msg-value-loop
### Severity: High

### SafEth.sol


```
SafEth.stake() (SafEth.sol#1589-1627) use msg.value in a loop: ethAmount = (msg.value * weight) / totalWeight (SafEth.sol#1614)



    
1614             uint256 ethAmount = (msg.value * weight) / totalWeight;



```

## reentrancy-eth
### Severity: High

### SafEth.sol


```
Reentrancy in SafEth.stake() (SafEth.sol#1589-1627):
	External calls:
	- depositAmount = derivative.deposit{value: ethAmount}() (SafEth.sol#1617)
	State variables written after the call(s):
	- _mint(msg.sender,mintAmount) (SafEth.sol#1625)
		- _totalSupply += amount (SafEth.sol#1409)
	ERC20Upgradeable._totalSupply (SafEth.sol#1183) can be used in cross function reentrancies:
	- ERC20Upgradeable._burn(address,uint256) (SafEth.sol#1427-1442)
	- ERC20Upgradeable._mint(address,uint256) (SafEth.sol#1404-1414)
	- ERC20Upgradeable.totalSupply() (SafEth.sol#1241-1243)



    
1617             uint256 depositAmount = derivative.deposit{value: ethAmount}();



    
1625         _mint(msg.sender, mintAmount);



    
1409         _totalSupply += amount;



```

## divide-before-multiply
### Severity: Medium

### Reth.sol


```
Reth.deposit() (Reth.sol#1412-1460) performs a multiplication on the result of a division:
	- minOut = ((((rethPerEth * msg.value) / 10 ** 18) * ((10 ** 18 - maxSlippage))) / 10 ** 18) (Reth.sol#1429-1430)



    
1429             uint256 minOut = ((((rethPerEth * msg.value) / 10 ** 18) *
1430                 ((10 ** 18 - maxSlippage))) / 10 ** 18);



```

### SfrxEth.sol


```
SfrxEth.withdraw(uint256) (SfrxEth.sol#640-668) performs a multiplication on the result of a division:
	- minOut = (((ethPerDerivative(_amount) * _amount) / 10 ** 18) * (10 ** 18 - maxSlippage)) / 10 ** 18 (SfrxEth.sol#654-655)



    
654         uint256 minOut = (((ethPerDerivative(_amount) * _amount) / 10 ** 18) *
655             (10 ** 18 - maxSlippage)) / 10 ** 18;



```

## unchecked-lowlevel
### Severity: Medium

### Reth.sol


```
AddressUpgradeable.sendValue(address,uint256) (Reth.sol#338-343) ignores return value by (success) = recipient.call{value: amount}() (Reth.sol#341)



    
341         (bool success, ) = recipient.call{value: amount}("");



```

```
Reth.withdraw(uint256) (Reth.sol#1363-1370) ignores return value by (sent) = address(msg.sender).call{value: address(this).balance}() (Reth.sol#1366-1368)



    
1366         (bool sent, ) = address(msg.sender).call{value: address(this).balance}(
1367             ""
1368         );



```

### SafEth.sol


```
SafEth.unstake(uint256) (SafEth.sol#1634-1655) ignores return value by (sent) = address(msg.sender).call{value: ethAmountToWithdraw}() (SafEth.sol#1650-1652)



    
1650         (bool sent, ) = address(msg.sender).call{value: ethAmountToWithdraw}(
1651             ""
1652         );



```

```
AddressUpgradeable.sendValue(address,uint256) (SafEth.sol#618-623) ignores return value by (success) = recipient.call{value: amount}() (SafEth.sol#621)



    
621         (bool success, ) = recipient.call{value: amount}("");



```

### SfrxEth.sol


```
AddressUpgradeable.sendValue(address,uint256) (SfrxEth.sol#102-107) ignores return value by (success) = recipient.call{value: amount}() (SfrxEth.sol#105)



    
105         (bool success, ) = recipient.call{value: amount}("");



```

```
SfrxEth.withdraw(uint256) (SfrxEth.sol#640-668) ignores return value by (sent) = address(msg.sender).call{value: address(this).balance}() (SfrxEth.sol#664-666)



    
664         (bool sent, ) = address(msg.sender).call{value: address(this).balance}(
665             ""
666         );



```

### WstEth.sol


```
WstEth.deposit() (WstEth.sol#1071-1079) ignores return value by (sent) = WST_ETH.call{value: msg.value}() (WstEth.sol#1074)



    
1074         (bool sent, ) = WST_ETH.call{value: msg.value}("");



```

```
WstEth.withdraw(uint256) (WstEth.sol#1054-1065) ignores return value by (sent) = address(msg.sender).call{value: address(this).balance}() (WstEth.sol#1061-1063)



    
1061         (bool sent, ) = address(msg.sender).call{value: address(this).balance}(
1062             ""
1063         );



```

```
AddressUpgradeable.sendValue(address,uint256) (WstEth.sol#86-91) ignores return value by (success) = recipient.call{value: amount}() (WstEth.sol#89)



    
89         (bool success, ) = recipient.call{value: amount}("");



```

## unused-return
### Severity: Medium

### Reth.sol


```
Reth.swapExactInputSingleHop(address,address,uint24,uint256,uint256) (Reth.sol#1339-1358) ignores return value by IERC20(_tokenIn).approve(UNISWAP_ROUTER,_amountIn) (Reth.sol#1346)



    
1346         IERC20(_tokenIn).approve(UNISWAP_ROUTER, _amountIn);



```

```
Reth.poolPrice() (Reth.sol#1484-1498) ignores return value by (sqrtPriceX96) = pool.slot0() (Reth.sol#1496)



    
1496         (uint160 sqrtPriceX96, , , , , , ) = pool.slot0();



```

### SafEth.sol


```
SafEth.rebalanceToWeights() (SafEth.sol#1664-1681) ignores return value by derivatives[i_scope_0].deposit{value: ethAmount}() (SafEth.sol#1678)



    
1678             derivatives[i].deposit{value: ethAmount}();



```

### SfrxEth.sol


```
SfrxEth.withdraw(uint256) (SfrxEth.sol#640-668) ignores return value by IFrxEthEthPool(FRX_ETH_CRV_POOL_ADDRESS).exchange(1,0,frxEthBalance,minOut) (SfrxEth.sol#657-662)



    
657         IFrxEthEthPool(FRX_ETH_CRV_POOL_ADDRESS).exchange(
658             1,
659             0,
660             frxEthBalance,
661             minOut
662         );



```

```
SfrxEth.deposit() (SfrxEth.sol#674-686) ignores return value by frxETHMinterContract.submitAndDeposit{value: msg.value}(address(this)) (SfrxEth.sol#681)



    
681         frxETHMinterContract.submitAndDeposit{value: msg.value}(address(this));



```

```
SfrxEth.withdraw(uint256) (SfrxEth.sol#640-668) ignores return value by IsFrxEth(FRX_ETH_ADDRESS).approve(FRX_ETH_CRV_POOL_ADDRESS,frxEthBalance) (SfrxEth.sol#649-652)



    
649         IsFrxEth(FRX_ETH_ADDRESS).approve(
650             FRX_ETH_CRV_POOL_ADDRESS,
651             frxEthBalance
652         );



```

```
SfrxEth.withdraw(uint256) (SfrxEth.sol#640-668) ignores return value by IsFrxEth(SFRX_ETH_ADDRESS).redeem(_amount,address(this),address(this)) (SfrxEth.sol#641-645)



    
641         IsFrxEth(SFRX_ETH_ADDRESS).redeem(
642             _amount,
643             address(this),
644             address(this)
645         );



```

### WstEth.sol


```
WstEth.withdraw(uint256) (WstEth.sol#1054-1065) ignores return value by IStEthEthPool(LIDO_CRV_POOL).exchange(1,0,stEthBal,minOut) (WstEth.sol#1059)



    
1059         IStEthEthPool(LIDO_CRV_POOL).exchange(1, 0, stEthBal, minOut);



```

```
WstEth.withdraw(uint256) (WstEth.sol#1054-1065) ignores return value by IWStETH(WST_ETH).unwrap(_amount) (WstEth.sol#1055)



    
1055         IWStETH(WST_ETH).unwrap(_amount);



```

```
WstEth.withdraw(uint256) (WstEth.sol#1054-1065) ignores return value by IERC20(STETH_TOKEN).approve(LIDO_CRV_POOL,stEthBal) (WstEth.sol#1057)



    
1057         IERC20(STETH_TOKEN).approve(LIDO_CRV_POOL, stEthBal);



```

## incorrect-equality
### Severity: Medium

### SafEth.sol


```
SafEth.rebalanceToWeights() (SafEth.sol#1664-1681) uses a dangerous strict equality:
	- weights[i_scope_0] == 0 || ethAmountToRebalance == 0 (SafEth.sol#1674)



    
1674             if (weights[i] == 0 || ethAmountToRebalance == 0) continue;



```

## reentrancy-no-eth
### Severity: Medium

### SafEth.sol


```
Reentrancy in SafEth.unstake(uint256) (SafEth.sol#1634-1655):
	External calls:
	- derivatives[i].withdraw(derivativeAmount) (SafEth.sol#1644)
	State variables written after the call(s):
	- _burn(msg.sender,_safEthAmount) (SafEth.sol#1646)
		- _totalSupply -= amount (SafEth.sol#1437)
	ERC20Upgradeable._totalSupply (SafEth.sol#1183) can be used in cross function reentrancies:
	- ERC20Upgradeable._burn(address,uint256) (SafEth.sol#1427-1442)
	- ERC20Upgradeable._mint(address,uint256) (SafEth.sol#1404-1414)
	- ERC20Upgradeable.totalSupply() (SafEth.sol#1241-1243)



    
1644             derivatives[i].withdraw(derivativeAmount);



    
1646         _burn(msg.sender, _safEthAmount);



    
1437         _totalSupply -= amount;



```

## shadowing-local
### Severity: Low

### Reth.sol


```
Reth.initialize(address)._owner (Reth.sol#1298) shadows:
	- OwnableUpgradeable._owner (Reth.sol#652) (state variable)



    
1298     function initialize(address _owner) external initializer {



```

### SafEth.sol


```
SafEth.stake().totalSupply (SafEth.sol#1603) shadows:
	- ERC20Upgradeable.totalSupply() (SafEth.sol#1241-1243) (function)
	- IERC20Upgradeable.totalSupply() (SafEth.sol#1072) (function)



    
1603         uint256 totalSupply = totalSupply();



```

### SfrxEth.sol


```
SfrxEth.initialize(address)._owner (SfrxEth.sol#616) shadows:
	- OwnableUpgradeable._owner (SfrxEth.sol#416) (state variable)



    
616     function initialize(address _owner) external initializer {



```

### WstEth.sol


```
WstEth.initialize(address)._owner (WstEth.sol#1031) shadows:
	- OwnableUpgradeable._owner (WstEth.sol#400) (state variable)



    
1031     function initialize(address _owner) external initializer {



```

## calls-loop
### Severity: Low

### SafEth.sol


```
SafEth.rebalanceToWeights() (SafEth.sol#1664-1681) has external calls inside a loop: derivatives[i].withdraw(derivatives[i].balance()) (SafEth.sol#1668)



    
1668                 derivatives[i].withdraw(derivatives[i].balance());



```

```
SafEth.stake() (SafEth.sol#1589-1627) has external calls inside a loop: depositAmount = derivative.deposit{value: ethAmount}() (SafEth.sol#1617)



    
1617             uint256 depositAmount = derivative.deposit{value: ethAmount}();



```

```
SafEth.stake() (SafEth.sol#1589-1627) has external calls inside a loop: underlyingValue += (derivatives[i].ethPerDerivative(derivatives[i].balance()) * derivatives[i].balance()) / 10 ** 18 (SafEth.sol#1598-1601)



    
1598             underlyingValue +=
1599                 (derivatives[i].ethPerDerivative(derivatives[i].balance()) *
1600                     derivatives[i].balance()) /
1601                 10 ** 18;



```

```
SafEth.rebalanceToWeights() (SafEth.sol#1664-1681) has external calls inside a loop: derivatives[i].balance() > 0 (SafEth.sol#1667)



    
1667             if (derivatives[i].balance() > 0)



```

```
SafEth.rebalanceToWeights() (SafEth.sol#1664-1681) has external calls inside a loop: derivatives[i_scope_0].deposit{value: ethAmount}() (SafEth.sol#1678)



    
1678             derivatives[i].deposit{value: ethAmount}();



```

```
SafEth.unstake(uint256) (SafEth.sol#1634-1655) has external calls inside a loop: derivatives[i].withdraw(derivativeAmount) (SafEth.sol#1644)



    
1644             derivatives[i].withdraw(derivativeAmount);



```

```
SafEth.stake() (SafEth.sol#1589-1627) has external calls inside a loop: derivativeReceivedEthValue = (derivative.ethPerDerivative(depositAmount) * depositAmount) / 10 ** 18 (SafEth.sol#1618-1620)



    
1618             uint derivativeReceivedEthValue = (derivative.ethPerDerivative(
1619                 depositAmount
1620             ) * depositAmount) / 10 ** 18;



```

```
SafEth.unstake(uint256) (SafEth.sol#1634-1655) has external calls inside a loop: derivativeAmount = (derivatives[i].balance() * _safEthAmount) / safEthTotalSupply (SafEth.sol#1641-1642)



    
1641             uint256 derivativeAmount = (derivatives[i].balance() *
1642                 _safEthAmount) / safEthTotalSupply;



```

## reentrancy-benign
### Severity: Low

### SafEth.sol


```
Reentrancy in SafEth.unstake(uint256) (SafEth.sol#1634-1655):
	External calls:
	- derivatives[i].withdraw(derivativeAmount) (SafEth.sol#1644)
	State variables written after the call(s):
	- _burn(msg.sender,_safEthAmount) (SafEth.sol#1646)
		- _balances[account] = accountBalance - amount (SafEth.sol#1435)



    
1644             derivatives[i].withdraw(derivativeAmount);



    
1644             derivatives[i].withdraw(derivativeAmount);



    
1646         _burn(msg.sender, _safEthAmount);



    
1435             _balances[account] = accountBalance - amount;



```

```
Reentrancy in SafEth.stake() (SafEth.sol#1589-1627):
	External calls:
	- depositAmount = derivative.deposit{value: ethAmount}() (SafEth.sol#1617)
	State variables written after the call(s):
	- _mint(msg.sender,mintAmount) (SafEth.sol#1625)
		- _balances[account] += amount (SafEth.sol#1410)



    
1617             uint256 depositAmount = derivative.deposit{value: ethAmount}();



    
1625         _mint(msg.sender, mintAmount);



    
1410         _balances[account] += amount;



```

## reentrancy-events
### Severity: Low

### SafEth.sol


```
Reentrancy in SafEth.unstake(uint256) (SafEth.sol#1634-1655):
	External calls:
	- derivatives[i].withdraw(derivativeAmount) (SafEth.sol#1644)
	- (sent) = address(msg.sender).call{value: ethAmountToWithdraw}() (SafEth.sol#1650-1652)
	External calls sending eth:
	- (sent) = address(msg.sender).call{value: ethAmountToWithdraw}() (SafEth.sol#1650-1652)
	Event emitted after the call(s):
	- Unstaked(msg.sender,ethAmountToWithdraw,_safEthAmount) (SafEth.sol#1654)



    
1644             derivatives[i].withdraw(derivativeAmount);



    
1650         (bool sent, ) = address(msg.sender).call{value: ethAmountToWithdraw}(
1651             ""
1652         );



    
1650         (bool sent, ) = address(msg.sender).call{value: ethAmountToWithdraw}(
1651             ""
1652         );



    
1654         emit Unstaked(msg.sender, ethAmountToWithdraw, _safEthAmount);



```

```
Reentrancy in SafEth.stake() (SafEth.sol#1589-1627):
	External calls:
	- depositAmount = derivative.deposit{value: ethAmount}() (SafEth.sol#1617)
	Event emitted after the call(s):
	- Staked(msg.sender,msg.value,mintAmount) (SafEth.sol#1626)
	- Transfer(address(0),account,amount) (SafEth.sol#1411)
		- _mint(msg.sender,mintAmount) (SafEth.sol#1625)



    
1617             uint256 depositAmount = derivative.deposit{value: ethAmount}();



    
1626         emit Staked(msg.sender, msg.value, mintAmount);



    
1411         emit Transfer(address(0), account, amount);



    
1625         _mint(msg.sender, mintAmount);



```

```
Reentrancy in SafEth.unstake(uint256) (SafEth.sol#1634-1655):
	External calls:
	- derivatives[i].withdraw(derivativeAmount) (SafEth.sol#1644)
	Event emitted after the call(s):
	- Transfer(account,address(0),amount) (SafEth.sol#1439)
		- _burn(msg.sender,_safEthAmount) (SafEth.sol#1646)



    
1644             derivatives[i].withdraw(derivativeAmount);



    
1439         emit Transfer(account, address(0), amount);



    
1646         _burn(msg.sender, _safEthAmount);



```

```
Reentrancy in SafEth.rebalanceToWeights() (SafEth.sol#1664-1681):
	External calls:
	- derivatives[i].withdraw(derivatives[i].balance()) (SafEth.sol#1668)
	- derivatives[i_scope_0].deposit{value: ethAmount}() (SafEth.sol#1678)
	External calls sending eth:
	- derivatives[i_scope_0].deposit{value: ethAmount}() (SafEth.sol#1678)
	Event emitted after the call(s):
	- Rebalanced() (SafEth.sol#1680)



    
1668                 derivatives[i].withdraw(derivatives[i].balance());



    
1678             derivatives[i].deposit{value: ethAmount}();



    
1678             derivatives[i].deposit{value: ethAmount}();



    
1680         emit Rebalanced();



```

```
Reentrancy in SafEth.setMaxSlippage(uint256,uint256) (SafEth.sol#1728-1734):
	External calls:
	- derivatives[_derivativeIndex].setMaxSlippage(_slippage) (SafEth.sol#1732)
	Event emitted after the call(s):
	- SetMaxSlippage(_derivativeIndex,_slippage) (SafEth.sol#1733)



    
1732         derivatives[_derivativeIndex].setMaxSlippage(_slippage);



    
1733         emit SetMaxSlippage(_derivativeIndex, _slippage);



```

## assembly
### Severity: Informational

### Reth.sol


```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (Reth.sol#452-472) uses assembly
	- INLINE ASM (Reth.sol#464-467)



    
464                 assembly {
465                     let returndata_size := mload(returndata)
466                     revert(add(32, returndata), returndata_size)
467                 }



```

### SafEth.sol


```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (SafEth.sol#732-752) uses assembly
	- INLINE ASM (SafEth.sol#744-747)



    
744                 assembly {
745                     let returndata_size := mload(returndata)
746                     revert(add(32, returndata), returndata_size)
747                 }



```

### SfrxEth.sol


```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (SfrxEth.sol#216-236) uses assembly
	- INLINE ASM (SfrxEth.sol#228-231)



    
228                 assembly {
229                     let returndata_size := mload(returndata)
230                     revert(add(32, returndata), returndata_size)
231                 }



```

### WstEth.sol


```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (WstEth.sol#200-220) uses assembly
	- INLINE ASM (WstEth.sol#212-215)



    
212                 assembly {
213                     let returndata_size := mload(returndata)
214                     revert(add(32, returndata), returndata_size)
215                 }



```

## dead-code
### Severity: Informational

### Reth.sol


```
ContextUpgradeable._msgData() (Reth.sol#627-629) is never used and should be removed



    
627     function _msgData() internal view virtual returns (bytes calldata) {
628         return msg.data;
629     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256) (Reth.sol#392-398) is never used and should be removed



    
392     function functionCallWithValue(
393         address target,
394         bytes memory data,
395         uint256 value
396     ) internal returns (bytes memory) {
397         return functionCallWithValue(target, data, value, "Address: low-level call with value failed");
398     }



```

```
AddressUpgradeable.functionCall(address,bytes) (Reth.sol#363-365) is never used and should be removed



    
363     function functionCall(address target, bytes memory data) internal returns (bytes memory) {
364         return functionCall(target, data, "Address: low-level call failed");
365     }



```

```
ContextUpgradeable.__Context_init_unchained() (Reth.sol#621-622) is never used and should be removed



    
621     function __Context_init_unchained() internal onlyInitializing {
622     }



```

```
AddressUpgradeable.functionCall(address,bytes,string) (Reth.sol#373-379) is never used and should be removed



    
373     function functionCall(
374         address target,
375         bytes memory data,
376         string memory errorMessage
377     ) internal returns (bytes memory) {
378         return functionCallWithValue(target, data, 0, errorMessage);
379     }



```

```
AddressUpgradeable.sendValue(address,uint256) (Reth.sol#338-343) is never used and should be removed



    
338     function sendValue(address payable recipient, uint256 amount) internal {
339         require(address(this).balance >= amount, "Address: insufficient balance");
340 
341         (bool success, ) = recipient.call{value: amount}("");
342         require(success, "Address: unable to send value, recipient may have reverted");
343     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes) (Reth.sol#425-427) is never used and should be removed



    
425     function functionStaticCall(address target, bytes memory data) internal view returns (bytes memory) {
426         return functionStaticCall(target, data, "Address: low-level static call failed");
427     }



```

```
OwnableUpgradeable.__Ownable_init() (Reth.sol#659-661) is never used and should be removed



    
659     function __Ownable_init() internal onlyInitializing {
660         __Ownable_init_unchained();
661     }



```

```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (Reth.sol#452-472) is never used and should be removed



    
452     function verifyCallResult(
453         bool success,
454         bytes memory returndata,
455         string memory errorMessage
456     ) internal pure returns (bytes memory) {
457         if (success) {
458             return returndata;
459         } else {
460             // Look for revert reason and bubble it up if present
461             if (returndata.length > 0) {
462                 // The easiest way to bubble the revert reason is using memory via assembly
463                 /// @solidity memory-safe-assembly
464                 assembly {
465                     let returndata_size := mload(returndata)
466                     revert(add(32, returndata), returndata_size)
467                 }
468             } else {
469                 revert(errorMessage);
470             }
471         }
472     }



```

```
OwnableUpgradeable.__Ownable_init_unchained() (Reth.sol#663-665) is never used and should be removed



    
663     function __Ownable_init_unchained() internal onlyInitializing {
664         _transferOwnership(_msgSender());
665     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes,string) (Reth.sol#435-444) is never used and should be removed



    
435     function functionStaticCall(
436         address target,
437         bytes memory data,
438         string memory errorMessage
439     ) internal view returns (bytes memory) {
440         require(isContract(target), "Address: static call to non-contract");
441 
442         (bool success, bytes memory returndata) = target.staticcall(data);
443         return verifyCallResult(success, returndata, errorMessage);
444     }



```

```
ContextUpgradeable.__Context_init() (Reth.sol#618-619) is never used and should be removed



    
618     function __Context_init() internal onlyInitializing {
619     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (Reth.sol#406-417) is never used and should be removed



    
406     function functionCallWithValue(
407         address target,
408         bytes memory data,
409         uint256 value,
410         string memory errorMessage
411     ) internal returns (bytes memory) {
412         require(address(this).balance >= value, "Address: insufficient balance for call");
413         require(isContract(target), "Address: call to non-contract");
414 
415         (bool success, bytes memory returndata) = target.call{value: value}(data);
416         return verifyCallResult(success, returndata, errorMessage);
417     }



```

### SafEth.sol


```
ContextUpgradeable._msgData() (SafEth.sol#907-909) is never used and should be removed



    
907     function _msgData() internal view virtual returns (bytes calldata) {
908         return msg.data;
909     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256) (SafEth.sol#672-678) is never used and should be removed



    
672     function functionCallWithValue(
673         address target,
674         bytes memory data,
675         uint256 value
676     ) internal returns (bytes memory) {
677         return functionCallWithValue(target, data, value, "Address: low-level call with value failed");
678     }



```

```
AddressUpgradeable.functionCall(address,bytes) (SafEth.sol#643-645) is never used and should be removed



    
643     function functionCall(address target, bytes memory data) internal returns (bytes memory) {
644         return functionCall(target, data, "Address: low-level call failed");
645     }



```

```
ContextUpgradeable.__Context_init_unchained() (SafEth.sol#901-902) is never used and should be removed



    
901     function __Context_init_unchained() internal onlyInitializing {
902     }



```

```
AddressUpgradeable.functionCall(address,bytes,string) (SafEth.sol#653-659) is never used and should be removed



    
653     function functionCall(
654         address target,
655         bytes memory data,
656         string memory errorMessage
657     ) internal returns (bytes memory) {
658         return functionCallWithValue(target, data, 0, errorMessage);
659     }



```

```
AddressUpgradeable.sendValue(address,uint256) (SafEth.sol#618-623) is never used and should be removed



    
618     function sendValue(address payable recipient, uint256 amount) internal {
619         require(address(this).balance >= amount, "Address: insufficient balance");
620 
621         (bool success, ) = recipient.call{value: amount}("");
622         require(success, "Address: unable to send value, recipient may have reverted");
623     }



```

```
ERC20._burn(address,uint256) (SafEth.sol#432-448) is never used and should be removed



    
432     function _burn(address account, uint256 amount) internal virtual {
433         require(account != address(0), "ERC20: burn from the zero address");
434 
435         _beforeTokenTransfer(account, address(0), amount);
436 
437         uint256 accountBalance = _balances[account];
438         require(accountBalance >= amount, "ERC20: burn amount exceeds balance");
439         unchecked {
440             _balances[account] = accountBalance - amount;
441             // Overflow not possible: amount <= accountBalance <= totalSupply.
442             _totalSupply -= amount;
443         }
444 
445         emit Transfer(account, address(0), amount);
446 
447         _afterTokenTransfer(account, address(0), amount);
448     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes) (SafEth.sol#705-707) is never used and should be removed



    
705     function functionStaticCall(address target, bytes memory data) internal view returns (bytes memory) {
706         return functionStaticCall(target, data, "Address: low-level static call failed");
707     }



```

```
OwnableUpgradeable.__Ownable_init() (SafEth.sol#939-941) is never used and should be removed



    
939     function __Ownable_init() internal onlyInitializing {
940         __Ownable_init_unchained();
941     }



```

```
Context._msgData() (SafEth.sol#152-154) is never used and should be removed



    
152     function _msgData() internal view virtual returns (bytes calldata) {
153         return msg.data;
154     }



```

```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (SafEth.sol#732-752) is never used and should be removed



    
732     function verifyCallResult(
733         bool success,
734         bytes memory returndata,
735         string memory errorMessage
736     ) internal pure returns (bytes memory) {
737         if (success) {
738             return returndata;
739         } else {
740             // Look for revert reason and bubble it up if present
741             if (returndata.length > 0) {
742                 // The easiest way to bubble the revert reason is using memory via assembly
743                 /// @solidity memory-safe-assembly
744                 assembly {
745                     let returndata_size := mload(returndata)
746                     revert(add(32, returndata), returndata_size)
747                 }
748             } else {
749                 revert(errorMessage);
750             }
751         }
752     }



```

```
OwnableUpgradeable.__Ownable_init_unchained() (SafEth.sol#943-945) is never used and should be removed



    
943     function __Ownable_init_unchained() internal onlyInitializing {
944         _transferOwnership(_msgSender());
945     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes,string) (SafEth.sol#715-724) is never used and should be removed



    
715     function functionStaticCall(
716         address target,
717         bytes memory data,
718         string memory errorMessage
719     ) internal view returns (bytes memory) {
720         require(isContract(target), "Address: static call to non-contract");
721 
722         (bool success, bytes memory returndata) = target.staticcall(data);
723         return verifyCallResult(success, returndata, errorMessage);
724     }



```

```
ERC20._mint(address,uint256) (SafEth.sol#406-419) is never used and should be removed



    
406     function _mint(address account, uint256 amount) internal virtual {
407         require(account != address(0), "ERC20: mint to the zero address");
408 
409         _beforeTokenTransfer(address(0), account, amount);
410 
411         _totalSupply += amount;
412         unchecked {
413             // Overflow not possible: balance + amount is at most totalSupply + amount, which is checked above.
414             _balances[account] += amount;
415         }
416         emit Transfer(address(0), account, amount);
417 
418         _afterTokenTransfer(address(0), account, amount);
419     }



```

```
ContextUpgradeable.__Context_init() (SafEth.sol#898-899) is never used and should be removed



    
898     function __Context_init() internal onlyInitializing {
899     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (SafEth.sol#686-697) is never used and should be removed



    
686     function functionCallWithValue(
687         address target,
688         bytes memory data,
689         uint256 value,
690         string memory errorMessage
691     ) internal returns (bytes memory) {
692         require(address(this).balance >= value, "Address: insufficient balance for call");
693         require(isContract(target), "Address: call to non-contract");
694 
695         (bool success, bytes memory returndata) = target.call{value: value}(data);
696         return verifyCallResult(success, returndata, errorMessage);
697     }



```

### SfrxEth.sol


```
ContextUpgradeable._msgData() (SfrxEth.sol#391-393) is never used and should be removed



    
391     function _msgData() internal view virtual returns (bytes calldata) {
392         return msg.data;
393     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256) (SfrxEth.sol#156-162) is never used and should be removed



    
156     function functionCallWithValue(
157         address target,
158         bytes memory data,
159         uint256 value
160     ) internal returns (bytes memory) {
161         return functionCallWithValue(target, data, value, "Address: low-level call with value failed");
162     }



```

```
AddressUpgradeable.functionCall(address,bytes) (SfrxEth.sol#127-129) is never used and should be removed



    
127     function functionCall(address target, bytes memory data) internal returns (bytes memory) {
128         return functionCall(target, data, "Address: low-level call failed");
129     }



```

```
ContextUpgradeable.__Context_init_unchained() (SfrxEth.sol#385-386) is never used and should be removed



    
385     function __Context_init_unchained() internal onlyInitializing {
386     }



```

```
AddressUpgradeable.functionCall(address,bytes,string) (SfrxEth.sol#137-143) is never used and should be removed



    
137     function functionCall(
138         address target,
139         bytes memory data,
140         string memory errorMessage
141     ) internal returns (bytes memory) {
142         return functionCallWithValue(target, data, 0, errorMessage);
143     }



```

```
AddressUpgradeable.sendValue(address,uint256) (SfrxEth.sol#102-107) is never used and should be removed



    
102     function sendValue(address payable recipient, uint256 amount) internal {
103         require(address(this).balance >= amount, "Address: insufficient balance");
104 
105         (bool success, ) = recipient.call{value: amount}("");
106         require(success, "Address: unable to send value, recipient may have reverted");
107     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes) (SfrxEth.sol#189-191) is never used and should be removed



    
189     function functionStaticCall(address target, bytes memory data) internal view returns (bytes memory) {
190         return functionStaticCall(target, data, "Address: low-level static call failed");
191     }



```

```
OwnableUpgradeable.__Ownable_init() (SfrxEth.sol#423-425) is never used and should be removed



    
423     function __Ownable_init() internal onlyInitializing {
424         __Ownable_init_unchained();
425     }



```

```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (SfrxEth.sol#216-236) is never used and should be removed



    
216     function verifyCallResult(
217         bool success,
218         bytes memory returndata,
219         string memory errorMessage
220     ) internal pure returns (bytes memory) {
221         if (success) {
222             return returndata;
223         } else {
224             // Look for revert reason and bubble it up if present
225             if (returndata.length > 0) {
226                 // The easiest way to bubble the revert reason is using memory via assembly
227                 /// @solidity memory-safe-assembly
228                 assembly {
229                     let returndata_size := mload(returndata)
230                     revert(add(32, returndata), returndata_size)
231                 }
232             } else {
233                 revert(errorMessage);
234             }
235         }
236     }



```

```
OwnableUpgradeable.__Ownable_init_unchained() (SfrxEth.sol#427-429) is never used and should be removed



    
427     function __Ownable_init_unchained() internal onlyInitializing {
428         _transferOwnership(_msgSender());
429     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes,string) (SfrxEth.sol#199-208) is never used and should be removed



    
199     function functionStaticCall(
200         address target,
201         bytes memory data,
202         string memory errorMessage
203     ) internal view returns (bytes memory) {
204         require(isContract(target), "Address: static call to non-contract");
205 
206         (bool success, bytes memory returndata) = target.staticcall(data);
207         return verifyCallResult(success, returndata, errorMessage);
208     }



```

```
ContextUpgradeable.__Context_init() (SfrxEth.sol#382-383) is never used and should be removed



    
382     function __Context_init() internal onlyInitializing {
383     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (SfrxEth.sol#170-181) is never used and should be removed



    
170     function functionCallWithValue(
171         address target,
172         bytes memory data,
173         uint256 value,
174         string memory errorMessage
175     ) internal returns (bytes memory) {
176         require(address(this).balance >= value, "Address: insufficient balance for call");
177         require(isContract(target), "Address: call to non-contract");
178 
179         (bool success, bytes memory returndata) = target.call{value: value}(data);
180         return verifyCallResult(success, returndata, errorMessage);
181     }



```

### WstEth.sol


```
ContextUpgradeable._msgData() (WstEth.sol#375-377) is never used and should be removed



    
375     function _msgData() internal view virtual returns (bytes calldata) {
376         return msg.data;
377     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256) (WstEth.sol#140-146) is never used and should be removed



    
140     function functionCallWithValue(
141         address target,
142         bytes memory data,
143         uint256 value
144     ) internal returns (bytes memory) {
145         return functionCallWithValue(target, data, value, "Address: low-level call with value failed");
146     }



```

```
AddressUpgradeable.functionCall(address,bytes) (WstEth.sol#111-113) is never used and should be removed



    
111     function functionCall(address target, bytes memory data) internal returns (bytes memory) {
112         return functionCall(target, data, "Address: low-level call failed");
113     }



```

```
ContextUpgradeable.__Context_init_unchained() (WstEth.sol#369-370) is never used and should be removed



    
369     function __Context_init_unchained() internal onlyInitializing {
370     }



```

```
AddressUpgradeable.functionCall(address,bytes,string) (WstEth.sol#121-127) is never used and should be removed



    
121     function functionCall(
122         address target,
123         bytes memory data,
124         string memory errorMessage
125     ) internal returns (bytes memory) {
126         return functionCallWithValue(target, data, 0, errorMessage);
127     }



```

```
AddressUpgradeable.sendValue(address,uint256) (WstEth.sol#86-91) is never used and should be removed



    
86     function sendValue(address payable recipient, uint256 amount) internal {
87         require(address(this).balance >= amount, "Address: insufficient balance");
88 
89         (bool success, ) = recipient.call{value: amount}("");
90         require(success, "Address: unable to send value, recipient may have reverted");
91     }



```

```
ERC20._burn(address,uint256) (WstEth.sol#888-904) is never used and should be removed



    
888     function _burn(address account, uint256 amount) internal virtual {
889         require(account != address(0), "ERC20: burn from the zero address");
890 
891         _beforeTokenTransfer(account, address(0), amount);
892 
893         uint256 accountBalance = _balances[account];
894         require(accountBalance >= amount, "ERC20: burn amount exceeds balance");
895         unchecked {
896             _balances[account] = accountBalance - amount;
897             // Overflow not possible: amount <= accountBalance <= totalSupply.
898             _totalSupply -= amount;
899         }
900 
901         emit Transfer(account, address(0), amount);
902 
903         _afterTokenTransfer(account, address(0), amount);
904     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes) (WstEth.sol#173-175) is never used and should be removed



    
173     function functionStaticCall(address target, bytes memory data) internal view returns (bytes memory) {
174         return functionStaticCall(target, data, "Address: low-level static call failed");
175     }



```

```
OwnableUpgradeable.__Ownable_init() (WstEth.sol#407-409) is never used and should be removed



    
407     function __Ownable_init() internal onlyInitializing {
408         __Ownable_init_unchained();
409     }



```

```
Context._msgData() (WstEth.sol#608-610) is never used and should be removed



    
608     function _msgData() internal view virtual returns (bytes calldata) {
609         return msg.data;
610     }



```

```
AddressUpgradeable.verifyCallResult(bool,bytes,string) (WstEth.sol#200-220) is never used and should be removed



    
200     function verifyCallResult(
201         bool success,
202         bytes memory returndata,
203         string memory errorMessage
204     ) internal pure returns (bytes memory) {
205         if (success) {
206             return returndata;
207         } else {
208             // Look for revert reason and bubble it up if present
209             if (returndata.length > 0) {
210                 // The easiest way to bubble the revert reason is using memory via assembly
211                 /// @solidity memory-safe-assembly
212                 assembly {
213                     let returndata_size := mload(returndata)
214                     revert(add(32, returndata), returndata_size)
215                 }
216             } else {
217                 revert(errorMessage);
218             }
219         }
220     }



```

```
OwnableUpgradeable.__Ownable_init_unchained() (WstEth.sol#411-413) is never used and should be removed



    
411     function __Ownable_init_unchained() internal onlyInitializing {
412         _transferOwnership(_msgSender());
413     }



```

```
AddressUpgradeable.functionStaticCall(address,bytes,string) (WstEth.sol#183-192) is never used and should be removed



    
183     function functionStaticCall(
184         address target,
185         bytes memory data,
186         string memory errorMessage
187     ) internal view returns (bytes memory) {
188         require(isContract(target), "Address: static call to non-contract");
189 
190         (bool success, bytes memory returndata) = target.staticcall(data);
191         return verifyCallResult(success, returndata, errorMessage);
192     }



```

```
ERC20._mint(address,uint256) (WstEth.sol#862-875) is never used and should be removed



    
862     function _mint(address account, uint256 amount) internal virtual {
863         require(account != address(0), "ERC20: mint to the zero address");
864 
865         _beforeTokenTransfer(address(0), account, amount);
866 
867         _totalSupply += amount;
868         unchecked {
869             // Overflow not possible: balance + amount is at most totalSupply + amount, which is checked above.
870             _balances[account] += amount;
871         }
872         emit Transfer(address(0), account, amount);
873 
874         _afterTokenTransfer(address(0), account, amount);
875     }



```

```
ContextUpgradeable.__Context_init() (WstEth.sol#366-367) is never used and should be removed



    
366     function __Context_init() internal onlyInitializing {
367     }



```

```
AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (WstEth.sol#154-165) is never used and should be removed



    
154     function functionCallWithValue(
155         address target,
156         bytes memory data,
157         uint256 value,
158         string memory errorMessage
159     ) internal returns (bytes memory) {
160         require(address(this).balance >= value, "Address: insufficient balance for call");
161         require(isContract(target), "Address: call to non-contract");
162 
163         (bool success, bytes memory returndata) = target.call{value: value}(data);
164         return verifyCallResult(success, returndata, errorMessage);
165     }



```

## solc-version
### Severity: Informational

### Reth.sol


```
Pragma version^0.8.13 (Reth.sol#2) allows old versions



    
2 pragma solidity ^0.8.13;



```

```
solc-0.8.13 is not recommended for deployment



```

### SafEth.sol


```
Pragma version^0.8.13 (SafEth.sol#2) allows old versions



    
2 pragma solidity ^0.8.13;



```

```
solc-0.8.13 is not recommended for deployment



```

### SfrxEth.sol


```
Pragma version^0.8.13 (SfrxEth.sol#2) allows old versions



    
2 pragma solidity ^0.8.13;



```

```
solc-0.8.13 is not recommended for deployment



```

### WstEth.sol


```
Pragma version^0.8.13 (WstEth.sol#2) allows old versions



    
2 pragma solidity ^0.8.13;



```

```
solc-0.8.13 is not recommended for deployment



```

## low-level-calls
### Severity: Informational

### Reth.sol


```
Low level call in AddressUpgradeable.sendValue(address,uint256) (Reth.sol#338-343):
	- (success) = recipient.call{value: amount}() (Reth.sol#341)



    
341         (bool success, ) = recipient.call{value: amount}("");



```

```
Low level call in Reth.withdraw(uint256) (Reth.sol#1363-1370):
	- (sent) = address(msg.sender).call{value: address(this).balance}() (Reth.sol#1366-1368)



    
1366         (bool sent, ) = address(msg.sender).call{value: address(this).balance}(
1367             ""
1368         );



```

```
Low level call in AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (Reth.sol#406-417):
	- (success,returndata) = target.call{value: value}(data) (Reth.sol#415)



    
415         (bool success, bytes memory returndata) = target.call{value: value}(data);



```

```
Low level call in AddressUpgradeable.functionStaticCall(address,bytes,string) (Reth.sol#435-444):
	- (success,returndata) = target.staticcall(data) (Reth.sol#442)



    
442         (bool success, bytes memory returndata) = target.staticcall(data);



```

### SafEth.sol


```
Low level call in AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (SafEth.sol#686-697):
	- (success,returndata) = target.call{value: value}(data) (SafEth.sol#695)



    
695         (bool success, bytes memory returndata) = target.call{value: value}(data);



```

```
Low level call in AddressUpgradeable.functionStaticCall(address,bytes,string) (SafEth.sol#715-724):
	- (success,returndata) = target.staticcall(data) (SafEth.sol#722)



    
722         (bool success, bytes memory returndata) = target.staticcall(data);



```

```
Low level call in AddressUpgradeable.sendValue(address,uint256) (SafEth.sol#618-623):
	- (success) = recipient.call{value: amount}() (SafEth.sol#621)



    
621         (bool success, ) = recipient.call{value: amount}("");



```

```
Low level call in SafEth.unstake(uint256) (SafEth.sol#1634-1655):
	- (sent) = address(msg.sender).call{value: ethAmountToWithdraw}() (SafEth.sol#1650-1652)



    
1650         (bool sent, ) = address(msg.sender).call{value: ethAmountToWithdraw}(
1651             ""
1652         );



```

### SfrxEth.sol


```
Low level call in AddressUpgradeable.functionStaticCall(address,bytes,string) (SfrxEth.sol#199-208):
	- (success,returndata) = target.staticcall(data) (SfrxEth.sol#206)



    
206         (bool success, bytes memory returndata) = target.staticcall(data);



```

```
Low level call in AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (SfrxEth.sol#170-181):
	- (success,returndata) = target.call{value: value}(data) (SfrxEth.sol#179)



    
179         (bool success, bytes memory returndata) = target.call{value: value}(data);



```

```
Low level call in SfrxEth.withdraw(uint256) (SfrxEth.sol#640-668):
	- (sent) = address(msg.sender).call{value: address(this).balance}() (SfrxEth.sol#664-666)



    
664         (bool sent, ) = address(msg.sender).call{value: address(this).balance}(
665             ""
666         );



```

```
Low level call in AddressUpgradeable.sendValue(address,uint256) (SfrxEth.sol#102-107):
	- (success) = recipient.call{value: amount}() (SfrxEth.sol#105)



    
105         (bool success, ) = recipient.call{value: amount}("");



```

### WstEth.sol


```
Low level call in WstEth.deposit() (WstEth.sol#1071-1079):
	- (sent) = WST_ETH.call{value: msg.value}() (WstEth.sol#1074)



    
1074         (bool sent, ) = WST_ETH.call{value: msg.value}("");



```

```
Low level call in AddressUpgradeable.sendValue(address,uint256) (WstEth.sol#86-91):
	- (success) = recipient.call{value: amount}() (WstEth.sol#89)



    
89         (bool success, ) = recipient.call{value: amount}("");



```

```
Low level call in AddressUpgradeable.functionStaticCall(address,bytes,string) (WstEth.sol#183-192):
	- (success,returndata) = target.staticcall(data) (WstEth.sol#190)



    
190         (bool success, bytes memory returndata) = target.staticcall(data);



```

```
Low level call in AddressUpgradeable.functionCallWithValue(address,bytes,uint256,string) (WstEth.sol#154-165):
	- (success,returndata) = target.call{value: value}(data) (WstEth.sol#163)



    
163         (bool success, bytes memory returndata) = target.call{value: value}(data);



```

```
Low level call in WstEth.withdraw(uint256) (WstEth.sol#1054-1065):
	- (sent) = address(msg.sender).call{value: address(this).balance}() (WstEth.sol#1061-1063)



    
1061         (bool sent, ) = address(msg.sender).call{value: address(this).balance}(
1062             ""
1063         );



```

## naming-convention
### Severity: Informational

### Reth.sol


```
Parameter Reth.swapExactInputSingleHop(address,address,uint24,uint256,uint256)._minOut (Reth.sol#1344) is not in mixedCase



    
1344         uint256 _minOut



```

```
Parameter Reth.poolCanDeposit(uint256)._amount (Reth.sol#1376) is not in mixedCase



    
1376     function poolCanDeposit(uint256 _amount) private view returns (bool) {



```

```
Parameter Reth.swapExactInputSingleHop(address,address,uint24,uint256,uint256)._poolFee (Reth.sol#1342) is not in mixedCase



    
1342         uint24 _poolFee,



```

```
Variable ContextUpgradeable.__gap (Reth.sol#636) is not in mixedCase



    
636     uint256[50] private __gap;



```

```
Function OwnableUpgradeable.__Ownable_init() (Reth.sol#659-661) is not in mixedCase



    
659     function __Ownable_init() internal onlyInitializing {
660         __Ownable_init_unchained();
661     }



```

```
Variable OwnableUpgradeable.__gap (Reth.sol#724) is not in mixedCase



    
724     uint256[49] private __gap;



```

```
Parameter Reth.initialize(address)._owner (Reth.sol#1298) is not in mixedCase



    
1298     function initialize(address _owner) external initializer {



```

```
Parameter Reth.setMaxSlippage(uint256)._slippage (Reth.sol#1314) is not in mixedCase



    
1314     function setMaxSlippage(uint256 _slippage) external onlyOwner {



```

```
Function ContextUpgradeable.__Context_init_unchained() (Reth.sol#621-622) is not in mixedCase



    
621     function __Context_init_unchained() internal onlyInitializing {
622     }



```

```
Parameter Reth.ethPerDerivative(uint256)._amount (Reth.sol#1467) is not in mixedCase



    
1467     function ethPerDerivative(uint256 _amount) public view returns (uint256) {



```

```
Function OwnableUpgradeable.__Ownable_init_unchained() (Reth.sol#663-665) is not in mixedCase



    
663     function __Ownable_init_unchained() internal onlyInitializing {
664         _transferOwnership(_msgSender());
665     }



```

```
Parameter Reth.swapExactInputSingleHop(address,address,uint24,uint256,uint256)._tokenOut (Reth.sol#1341) is not in mixedCase



    
1341         address _tokenOut,



```

```
Parameter Reth.swapExactInputSingleHop(address,address,uint24,uint256,uint256)._tokenIn (Reth.sol#1340) is not in mixedCase



    
1340         address _tokenIn,



```

```
Function ContextUpgradeable.__Context_init() (Reth.sol#618-619) is not in mixedCase



    
618     function __Context_init() internal onlyInitializing {
619     }



```

```
Parameter Reth.swapExactInputSingleHop(address,address,uint24,uint256,uint256)._amountIn (Reth.sol#1343) is not in mixedCase



    
1343         uint256 _amountIn,



```

### SafEth.sol


```
Parameter SafEth.setPauseUnstaking(bool)._pause (SafEth.sol#1767) is not in mixedCase



    
1767     function setPauseUnstaking(bool _pause) external onlyOwner {



```

```
Parameter SafEth.setPauseStaking(bool)._pause (SafEth.sol#1758) is not in mixedCase



    
1758     function setPauseStaking(bool _pause) external onlyOwner {



```

```
Variable ContextUpgradeable.__gap (SafEth.sol#916) is not in mixedCase



    
916     uint256[50] private __gap;



```

```
Function OwnableUpgradeable.__Ownable_init() (SafEth.sol#939-941) is not in mixedCase



    
939     function __Ownable_init() internal onlyInitializing {
940         __Ownable_init_unchained();
941     }



```

```
Parameter SafEth.setMaxAmount(uint256)._maxAmount (SafEth.sol#1749) is not in mixedCase



    
1749     function setMaxAmount(uint256 _maxAmount) external onlyOwner {



```

```
Variable OwnableUpgradeable.__gap (SafEth.sol#1004) is not in mixedCase



    
1004     uint256[49] private __gap;



```

```
Function ERC20Upgradeable.__ERC20_init_unchained(string,string) (SafEth.sol#1201-1204) is not in mixedCase



    
1201     function __ERC20_init_unchained(string memory name_, string memory symbol_) internal onlyInitializing {
1202         _name = name_;
1203         _symbol = symbol_;
1204     }



```

```
Parameter SafEth.initialize(string,string)._tokenName (SafEth.sol#1575) is not in mixedCase



    
1575         string memory _tokenName,



```

```
Function ERC20Upgradeable.__ERC20_init(string,string) (SafEth.sol#1197-1199) is not in mixedCase



    
1197     function __ERC20_init(string memory name_, string memory symbol_) internal onlyInitializing {
1198         __ERC20_init_unchained(name_, symbol_);
1199     }



```

```
Parameter SafEth.adjustWeight(uint256,uint256)._weight (SafEth.sol#1693) is not in mixedCase



    
1693         uint256 _weight



```

```
Function ContextUpgradeable.__Context_init_unchained() (SafEth.sol#901-902) is not in mixedCase



    
901     function __Context_init_unchained() internal onlyInitializing {
902     }



```

```
Parameter SafEth.addDerivative(address,uint256)._contractAddress (SafEth.sol#1709) is not in mixedCase



    
1709         address _contractAddress,



```

```
Variable ERC20Upgradeable.__gap (SafEth.sol#1536) is not in mixedCase



    
1536     uint256[45] private __gap;



```

```
Parameter SafEth.adjustWeight(uint256,uint256)._derivativeIndex (SafEth.sol#1692) is not in mixedCase



    
1692         uint256 _derivativeIndex,



```

```
Parameter SafEth.addDerivative(address,uint256)._weight (SafEth.sol#1710) is not in mixedCase



    
1710         uint256 _weight



```

```
Function OwnableUpgradeable.__Ownable_init_unchained() (SafEth.sol#943-945) is not in mixedCase



    
943     function __Ownable_init_unchained() internal onlyInitializing {
944         _transferOwnership(_msgSender());
945     }



```

```
Parameter SafEth.setMinAmount(uint256)._minAmount (SafEth.sol#1740) is not in mixedCase



    
1740     function setMinAmount(uint256 _minAmount) external onlyOwner {



```

```
Parameter SafEth.unstake(uint256)._safEthAmount (SafEth.sol#1634) is not in mixedCase



    
1634     function unstake(uint256 _safEthAmount) external {



```

```
Parameter SafEth.setMaxSlippage(uint256,uint256)._slippage (SafEth.sol#1730) is not in mixedCase



    
1730         uint _slippage



```

```
Parameter SafEth.setMaxSlippage(uint256,uint256)._derivativeIndex (SafEth.sol#1729) is not in mixedCase



    
1729         uint _derivativeIndex,



```

```
Function ContextUpgradeable.__Context_init() (SafEth.sol#898-899) is not in mixedCase



    
898     function __Context_init() internal onlyInitializing {
899     }



```

```
Parameter SafEth.initialize(string,string)._tokenSymbol (SafEth.sol#1576) is not in mixedCase



    
1576         string memory _tokenSymbol



```

### SfrxEth.sol


```
Variable ContextUpgradeable.__gap (SfrxEth.sol#400) is not in mixedCase



    
400     uint256[50] private __gap;



```

```
Parameter IFrxEthEthPool.exchange(int128,int128,uint256,uint256).min_dy (SfrxEth.sol#577) is not in mixedCase



    
577         uint256 min_dy



```

```
Parameter SfrxEth.withdraw(uint256)._amount (SfrxEth.sol#640) is not in mixedCase



    
640     function withdraw(uint256 _amount) external onlyOwner {



```

```
Function OwnableUpgradeable.__Ownable_init() (SfrxEth.sol#423-425) is not in mixedCase



    
423     function __Ownable_init() internal onlyInitializing {
424         __Ownable_init_unchained();
425     }



```

```
Variable OwnableUpgradeable.__gap (SfrxEth.sol#488) is not in mixedCase



    
488     uint256[49] private __gap;



```

```
Parameter SfrxEth.setMaxSlippage(uint256)._slippage (SfrxEth.sol#631) is not in mixedCase



    
631     function setMaxSlippage(uint256 _slippage) external onlyOwner {



```

```
Parameter SfrxEth.initialize(address)._owner (SfrxEth.sol#616) is not in mixedCase



    
616     function initialize(address _owner) external initializer {



```

```
Function ContextUpgradeable.__Context_init_unchained() (SfrxEth.sol#385-386) is not in mixedCase



    
385     function __Context_init_unchained() internal onlyInitializing {
386     }



```

```
Function OwnableUpgradeable.__Ownable_init_unchained() (SfrxEth.sol#427-429) is not in mixedCase



    
427     function __Ownable_init_unchained() internal onlyInitializing {
428         _transferOwnership(_msgSender());
429     }



```

```
Function IFrxEthEthPool.price_oracle() (SfrxEth.sol#580) is not in mixedCase



    
580     function price_oracle() external view returns (uint256);



```

```
Function ContextUpgradeable.__Context_init() (SfrxEth.sol#382-383) is not in mixedCase



    
382     function __Context_init() internal onlyInitializing {
383     }



```

### WstEth.sol


```
Parameter WstEth.setMaxSlippage(uint256)._slippage (WstEth.sol#1046) is not in mixedCase



    
1046     function setMaxSlippage(uint256 _slippage) external onlyOwner {



```

```
Variable ContextUpgradeable.__gap (WstEth.sol#384) is not in mixedCase



    
384     uint256[50] private __gap;



```

```
Function OwnableUpgradeable.__Ownable_init() (WstEth.sol#407-409) is not in mixedCase



    
407     function __Ownable_init() internal onlyInitializing {
408         __Ownable_init_unchained();
409     }



```

```
Variable OwnableUpgradeable.__gap (WstEth.sol#472) is not in mixedCase



    
472     uint256[49] private __gap;



```

```
Function ContextUpgradeable.__Context_init_unchained() (WstEth.sol#369-370) is not in mixedCase



    
369     function __Context_init_unchained() internal onlyInitializing {
370     }



```

```
Parameter WstEth.initialize(address)._owner (WstEth.sol#1031) is not in mixedCase



    
1031     function initialize(address _owner) external initializer {



```

```
Parameter IStEthEthPool.exchange(int128,int128,uint256,uint256).min_dy (WstEth.sol#561) is not in mixedCase



    
561         uint256 min_dy



```

```
Function OwnableUpgradeable.__Ownable_init_unchained() (WstEth.sol#411-413) is not in mixedCase



    
411     function __Ownable_init_unchained() internal onlyInitializing {
412         _transferOwnership(_msgSender());
413     }



```

```
Function ContextUpgradeable.__Context_init() (WstEth.sol#366-367) is not in mixedCase



    
366     function __Context_init() internal onlyInitializing {
367     }



```

```
Parameter WstEth.withdraw(uint256)._amount (WstEth.sol#1054) is not in mixedCase



    
1054     function withdraw(uint256 _amount) external onlyOwner {



```

## similar-names
### Severity: Informational

### Reth.sol


```
Variable IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount0Requested (Reth.sol#1048) is too similar to IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount1Requested (Reth.sol#1049)



    
1048         uint128 amount0Requested,



```

```
Variable Reth.deposit().rethBalance1 (Reth.sol#1453) is too similar to Reth.deposit().rethBalance2 (Reth.sol#1455)



    
1453             uint256 rethBalance1 = rocketTokenRETH.balanceOf(address(this));



```

```
Variable IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount0Requested (Reth.sol#1124) is too similar to IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount1Requested (Reth.sol#1125)



    
1124         uint128 amount0Requested,



```

```
Variable IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount0Requested (Reth.sol#1048) is too similar to IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount1Requested (Reth.sol#1125)



    
1048         uint128 amount0Requested,



```

```
Variable IUniswapV3PoolState.positions(bytes32).tokensOwed0 (Reth.sol#934) is too similar to IUniswapV3PoolState.positions(bytes32).tokensOwed1 (Reth.sol#935)



    
934             uint128 tokensOwed0,



```

```
Variable IUniswapV3PoolState.positions(bytes32).feeGrowthInside0LastX128 (Reth.sol#932) is too similar to IUniswapV3PoolState.positions(bytes32).feeGrowthInside1LastX128 (Reth.sol#933)



    
932             uint256 feeGrowthInside0LastX128,



```

```
Variable IUniswapV3PoolState.ticks(int24).feeGrowthOutside0X128 (Reth.sol#907) is too similar to IUniswapV3PoolState.ticks(int24).feeGrowthOutside1X128 (Reth.sol#908)



    
907             uint256 feeGrowthOutside0X128,



```

```
Variable IUniswapV3PoolOwnerActions.setFeeProtocol(uint8,uint8).feeProtocol0 (Reth.sol#1114) is too similar to IUniswapV3PoolOwnerActions.setFeeProtocol(uint8,uint8).feeProtocol1 (Reth.sol#1114)



    
1114     function setFeeProtocol(uint8 feeProtocol0, uint8 feeProtocol1) external;



```

```
Variable IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount0Requested (Reth.sol#1124) is too similar to IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount1Requested (Reth.sol#1049)



    
1124         uint128 amount0Requested,



```

## boolean-equal
### Severity: Informational

### SafEth.sol


```
SafEth.stake() (SafEth.sol#1589-1627) compares to a boolean constant:
	-require(bool,string)(pauseStaking == false,staking is paused) (SafEth.sol#1590)



    
1590         require(pauseStaking == false, "staking is paused");



```

```
SafEth.unstake(uint256) (SafEth.sol#1634-1655) compares to a boolean constant:
	-require(bool,string)(pauseUnstaking == false,unstaking is paused) (SafEth.sol#1635)



    
1635         require(pauseUnstaking == false, "unstaking is paused");



```

## unimplemented-functions
### Severity: Informational

### SafEth.sol


```
IWStETH (SafEth.sol#538-550) does not implement functions:
	- IWStETH.getStETHByWstETH(uint256) (SafEth.sol#545-547)
	- IWStETH.getWstETHByStETH(uint256) (SafEth.sol#541-543)
	- IWStETH.stEthPerToken() (SafEth.sol#549)
	- IWStETH.unwrap(uint256) (SafEth.sol#539)



    
538 abstract contract IWStETH is ERC20 {
539     function unwrap(uint256 _wstETHAmount) external virtual returns (uint256);
540 
541     function getWstETHByStETH(
542         uint256 _stETHAmount
543     ) external view virtual returns (uint256);
544 
545     function getStETHByWstETH(
546         uint256 _wstETHAmount
547     ) external view virtual returns (uint256);
548 
549     function stEthPerToken() external view virtual returns (uint256);
550 }



```

```
IStETH (SafEth.sol#552-554) does not implement functions:
	- IStETH.getTotalShares() (SafEth.sol#553)



    
552 abstract contract IStETH is ERC20 {
553     function getTotalShares() external view virtual returns (uint256);
554 }



```

### WstEth.sol


```
IWStETH (WstEth.sol#994-1006) does not implement functions:
	- IWStETH.getStETHByWstETH(uint256) (WstEth.sol#1001-1003)
	- IWStETH.getWstETHByStETH(uint256) (WstEth.sol#997-999)
	- IWStETH.stEthPerToken() (WstEth.sol#1005)
	- IWStETH.unwrap(uint256) (WstEth.sol#995)



    
994 abstract contract IWStETH is ERC20 {
995     function unwrap(uint256 _wstETHAmount) external virtual returns (uint256);
996 
997     function getWstETHByStETH(
998         uint256 _stETHAmount
999     ) external view virtual returns (uint256);
1000 
1001     function getStETHByWstETH(
1002         uint256 _wstETHAmount
1003     ) external view virtual returns (uint256);
1004 
1005     function stEthPerToken() external view virtual returns (uint256);
1006 }



```
