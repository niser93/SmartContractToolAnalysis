
# SLITHER ANALYSIS

## arbitrary-send-eth
### Severity: High

### JBXBuybackDelegate.sol


```
JBXBuybackDelegate._mint(JBDidPayData,uint256) (JBXBuybackDelegate.sol#3806-3824) sends eth to arbitrary user
	Dangerous calls:
	- jbxTerminal.addToBalanceOf{value: _data.amount.value}(_data.projectId,_data.amount.value,JBTokens.ETH,,new bytes(0)) (JBXBuybackDelegate.sol#3819-3821)



    
3819         jbxTerminal.addToBalanceOf{value: _data.amount.value}(
3820             _data.projectId, _data.amount.value, JBTokens.ETH, "", new bytes(0)
3821         );



```

## unchecked-transfer
### Severity: High

### JBXBuybackDelegate.sol


```
JBXBuybackDelegate.uniswapV3SwapCallback(int256,int256,bytes) (JBXBuybackDelegate.sol#3690-3706) ignores return value by weth.transfer(address(pool),_amountToSend) (JBXBuybackDelegate.sol#3705)



    
3705         weth.transfer(address(pool), _amountToSend);



```

```
JBXBuybackDelegate._swap(JBDidPayData,uint256,uint256) (JBXBuybackDelegate.sol#3731-3798) ignores return value by projectToken.transfer(_data.beneficiary,_nonReservedToken) (JBXBuybackDelegate.sol#3759)



    
3759         if (_nonReservedToken != 0) projectToken.transfer(_data.beneficiary, _nonReservedToken);



```

## divide-before-multiply
### Severity: Medium

### JBXBuybackDelegate.sol


```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse *= 2 - denominator * inverse (JBXBuybackDelegate.sol#2616)



    
2594                 denominator := div(denominator, lpotdod)



    
2616             inverse *= 2 - denominator * inverse; // inverse mod 2^64



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse *= 2 - denominator * inverse (JBXBuybackDelegate.sol#2618)



    
2594                 denominator := div(denominator, lpotdod)



    
2618             inverse *= 2 - denominator * inverse; // inverse mod 2^256



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- prod0 = prod0 / lpotdod (JBXBuybackDelegate.sol#2597)
	- result = prod0 * inverse (JBXBuybackDelegate.sol#2624)



    
2597                 prod0 := div(prod0, lpotdod)



    
2624             result = prod0 * inverse;



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse *= 2 - denominator * inverse (JBXBuybackDelegate.sol#2615)



    
2594                 denominator := div(denominator, lpotdod)



    
2615             inverse *= 2 - denominator * inverse; // inverse mod 2^32



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse *= 2 - denominator * inverse (JBXBuybackDelegate.sol#2614)



    
2594                 denominator := div(denominator, lpotdod)



    
2614             inverse *= 2 - denominator * inverse; // inverse mod 2^16



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse *= 2 - denominator * inverse (JBXBuybackDelegate.sol#2617)



    
2594                 denominator := div(denominator, lpotdod)



    
2617             inverse *= 2 - denominator * inverse; // inverse mod 2^128



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse *= 2 - denominator * inverse (JBXBuybackDelegate.sol#2613)



    
2594                 denominator := div(denominator, lpotdod)



    
2613             inverse *= 2 - denominator * inverse; // inverse mod 2^8



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) performs a multiplication on the result of a division:
	- denominator = denominator / lpotdod (JBXBuybackDelegate.sol#2594)
	- inverse = (3 * denominator) ^ 2 (JBXBuybackDelegate.sol#2609)



    
2594                 denominator := div(denominator, lpotdod)



    
2609             uint256 inverse = (3 * denominator) ^ 2;



```

## unused-return
### Severity: Medium

### JBXBuybackDelegate.sol


```
JBXBuybackDelegate._mint(JBDidPayData,uint256) (JBXBuybackDelegate.sol#3806-3824) ignores return value by IJBController(jbxTerminal.directory().controllerOf(_data.projectId)).mintTokensOf(_data.projectId,_amount,_data.beneficiary,_data.memo,_data.preferClaimedTokens,true) (JBXBuybackDelegate.sol#3809-3816)



    
3809         IJBController(jbxTerminal.directory().controllerOf(_data.projectId)).mintTokensOf({
3810             _projectId: _data.projectId,
3811             _tokenCount: _amount,
3812             _beneficiary: _data.beneficiary,
3813             _memo: _data.memo,
3814             _preferClaimedTokens: _data.preferClaimedTokens,
3815             _useReservedRate: true
3816         });



```

```
JBXBuybackDelegate._swap(JBDidPayData,uint256,uint256) (JBXBuybackDelegate.sol#3731-3798) ignores return value by controller.mintTokensOf(_data.projectId,_amountReceived,address(this),_data.memo,false,true) (JBXBuybackDelegate.sol#3775-3782)



    
3775             controller.mintTokensOf({
3776                 _projectId: _data.projectId,
3777                 _tokenCount: _amountReceived,
3778                 _beneficiary: address(this),
3779                 _memo: _data.memo,
3780                 _preferClaimedTokens: false,
3781                 _useReservedRate: true
3782             });



```

## shadowing-local
### Severity: Low

### JBXBuybackDelegate.sol


```
IUniswapV3PoolState.positions(bytes32).liquidity (JBXBuybackDelegate.sol#2921) shadows:
	- IUniswapV3PoolState.liquidity() (JBXBuybackDelegate.sol#2877) (function)



    
2921             uint128 liquidity,



```

## reentrancy-events
### Severity: Low

### JBXBuybackDelegate.sol


```
Reentrancy in JBXBuybackDelegate._swap(JBDidPayData,uint256,uint256) (JBXBuybackDelegate.sol#3731-3798):
	External calls:
	- projectToken.transfer(_data.beneficiary,_nonReservedToken) (JBXBuybackDelegate.sol#3759)
	- controller.burnTokensOf(address(this),_data.projectId,_reservedToken,,true) (JBXBuybackDelegate.sol#3766-3772)
	- controller.mintTokensOf(_data.projectId,_amountReceived,address(this),_data.memo,false,true) (JBXBuybackDelegate.sol#3775-3782)
	- controller.burnTokensOf(address(this),_data.projectId,_nonReservedToken,,false) (JBXBuybackDelegate.sol#3787-3793)
	- (amount0,amount1) = pool.swap(address(this),! _projectTokenIsZero,int256(_data.amount.value),TickMath.MAX_SQRT_RATIO - 1,abi.encode(_minimumReceivedFromSwap)) (JBXBuybackDelegate.sol#3736-3748)
	- (amount0,amount1) = pool.swap(address(this),! _projectTokenIsZero,int256(_data.amount.value),TickMath.MIN_SQRT_RATIO + 1,abi.encode(_minimumReceivedFromSwap)) (JBXBuybackDelegate.sol#3736-3748)
	Event emitted after the call(s):
	- JBXBuybackDelegate_Swap(_data.projectId,_data.amount.value,_amountReceived) (JBXBuybackDelegate.sol#3797)



    
3759         if (_nonReservedToken != 0) projectToken.transfer(_data.beneficiary, _nonReservedToken);



    
3766             controller.burnTokensOf({
3767                 _holder: address(this),
3768                 _projectId: _data.projectId,
3769                 _tokenCount: _reservedToken,
3770                 _memo: "",
3771                 _preferClaimedTokens: true
3772             });



    
3775             controller.mintTokensOf({
3776                 _projectId: _data.projectId,
3777                 _tokenCount: _amountReceived,
3778                 _beneficiary: address(this),
3779                 _memo: _data.memo,
3780                 _preferClaimedTokens: false,
3781                 _useReservedRate: true
3782             });



    
3787                 controller.burnTokensOf({
3788                     _holder: address(this),
3789                     _projectId: _data.projectId,
3790                     _tokenCount: _nonReservedToken,
3791                     _memo: "",
3792                     _preferClaimedTokens: false
3793                 });



    
3736         try pool.swap({
3737             recipient: address(this),
3738             zeroForOne: !_projectTokenIsZero,
3739             amountSpecified: int256(_data.amount.value),
3740             sqrtPriceLimitX96: _projectTokenIsZero ? TickMath.MAX_SQRT_RATIO - 1 : TickMath.MIN_SQRT_RATIO + 1,
3741             data: abi.encode(_minimumReceivedFromSwap)
3742         }) returns (int256 amount0, int256 amount1) {
3743             // Swap succeded, take note of the amount of projectToken received (negative as it is an exact input)
3744             _amountReceived = uint256(-(_projectTokenIsZero ? amount0 : amount1));
3745         } catch {
3746             // implies _amountReceived = 0 -> will later mint when back in didPay
3747             return _amountReceived;
3748         }



    
3736         try pool.swap({
3737             recipient: address(this),
3738             zeroForOne: !_projectTokenIsZero,
3739             amountSpecified: int256(_data.amount.value),
3740             sqrtPriceLimitX96: _projectTokenIsZero ? TickMath.MAX_SQRT_RATIO - 1 : TickMath.MIN_SQRT_RATIO + 1,
3741             data: abi.encode(_minimumReceivedFromSwap)
3742         }) returns (int256 amount0, int256 amount1) {
3743             // Swap succeded, take note of the amount of projectToken received (negative as it is an exact input)
3744             _amountReceived = uint256(-(_projectTokenIsZero ? amount0 : amount1));
3745         } catch {
3746             // implies _amountReceived = 0 -> will later mint when back in didPay
3747             return _amountReceived;
3748         }



    
3797         emit JBXBuybackDelegate_Swap(_data.projectId, _data.amount.value, _amountReceived);



```

```
Reentrancy in JBXBuybackDelegate.didPay(JBDidPayData) (JBXBuybackDelegate.sol#3656-3683):
	External calls:
	- _swap(_data,_minimumReceivedFromSwap,_reservedRate) == 0 (JBXBuybackDelegate.sol#3679)
		- projectToken.transfer(_data.beneficiary,_nonReservedToken) (JBXBuybackDelegate.sol#3759)
		- controller.burnTokensOf(address(this),_data.projectId,_reservedToken,,true) (JBXBuybackDelegate.sol#3766-3772)
		- controller.mintTokensOf(_data.projectId,_amountReceived,address(this),_data.memo,false,true) (JBXBuybackDelegate.sol#3775-3782)
		- controller.burnTokensOf(address(this),_data.projectId,_nonReservedToken,,false) (JBXBuybackDelegate.sol#3787-3793)
		- (amount0,amount1) = pool.swap(address(this),! _projectTokenIsZero,int256(_data.amount.value),TickMath.MAX_SQRT_RATIO - 1,abi.encode(_minimumReceivedFromSwap)) (JBXBuybackDelegate.sol#3736-3748)
		- (amount0,amount1) = pool.swap(address(this),! _projectTokenIsZero,int256(_data.amount.value),TickMath.MIN_SQRT_RATIO + 1,abi.encode(_minimumReceivedFromSwap)) (JBXBuybackDelegate.sol#3736-3748)
	- _mint(_data,_tokenCount) (JBXBuybackDelegate.sol#3679)
		- IJBController(jbxTerminal.directory().controllerOf(_data.projectId)).mintTokensOf(_data.projectId,_amount,_data.beneficiary,_data.memo,_data.preferClaimedTokens,true) (JBXBuybackDelegate.sol#3809-3816)
		- jbxTerminal.addToBalanceOf{value: _data.amount.value}(_data.projectId,_data.amount.value,JBTokens.ETH,,new bytes(0)) (JBXBuybackDelegate.sol#3819-3821)
	External calls sending eth:
	- _mint(_data,_tokenCount) (JBXBuybackDelegate.sol#3679)
		- jbxTerminal.addToBalanceOf{value: _data.amount.value}(_data.projectId,_data.amount.value,JBTokens.ETH,,new bytes(0)) (JBXBuybackDelegate.sol#3819-3821)
	Event emitted after the call(s):
	- JBXBuybackDelegate_Mint(_data.projectId) (JBXBuybackDelegate.sol#3823)
		- _mint(_data,_tokenCount) (JBXBuybackDelegate.sol#3679)



    
3679             if (_swap(_data, _minimumReceivedFromSwap, _reservedRate)== 0) _mint(_data, _tokenCount);



    
3759         if (_nonReservedToken != 0) projectToken.transfer(_data.beneficiary, _nonReservedToken);



    
3766             controller.burnTokensOf({
3767                 _holder: address(this),
3768                 _projectId: _data.projectId,
3769                 _tokenCount: _reservedToken,
3770                 _memo: "",
3771                 _preferClaimedTokens: true
3772             });



    
3775             controller.mintTokensOf({
3776                 _projectId: _data.projectId,
3777                 _tokenCount: _amountReceived,
3778                 _beneficiary: address(this),
3779                 _memo: _data.memo,
3780                 _preferClaimedTokens: false,
3781                 _useReservedRate: true
3782             });



    
3787                 controller.burnTokensOf({
3788                     _holder: address(this),
3789                     _projectId: _data.projectId,
3790                     _tokenCount: _nonReservedToken,
3791                     _memo: "",
3792                     _preferClaimedTokens: false
3793                 });



    
3736         try pool.swap({
3737             recipient: address(this),
3738             zeroForOne: !_projectTokenIsZero,
3739             amountSpecified: int256(_data.amount.value),
3740             sqrtPriceLimitX96: _projectTokenIsZero ? TickMath.MAX_SQRT_RATIO - 1 : TickMath.MIN_SQRT_RATIO + 1,
3741             data: abi.encode(_minimumReceivedFromSwap)
3742         }) returns (int256 amount0, int256 amount1) {
3743             // Swap succeded, take note of the amount of projectToken received (negative as it is an exact input)
3744             _amountReceived = uint256(-(_projectTokenIsZero ? amount0 : amount1));
3745         } catch {
3746             // implies _amountReceived = 0 -> will later mint when back in didPay
3747             return _amountReceived;
3748         }



    
3736         try pool.swap({
3737             recipient: address(this),
3738             zeroForOne: !_projectTokenIsZero,
3739             amountSpecified: int256(_data.amount.value),
3740             sqrtPriceLimitX96: _projectTokenIsZero ? TickMath.MAX_SQRT_RATIO - 1 : TickMath.MIN_SQRT_RATIO + 1,
3741             data: abi.encode(_minimumReceivedFromSwap)
3742         }) returns (int256 amount0, int256 amount1) {
3743             // Swap succeded, take note of the amount of projectToken received (negative as it is an exact input)
3744             _amountReceived = uint256(-(_projectTokenIsZero ? amount0 : amount1));
3745         } catch {
3746             // implies _amountReceived = 0 -> will later mint when back in didPay
3747             return _amountReceived;
3748         }



    
3679             if (_swap(_data, _minimumReceivedFromSwap, _reservedRate)== 0) _mint(_data, _tokenCount);



    
3809         IJBController(jbxTerminal.directory().controllerOf(_data.projectId)).mintTokensOf({
3810             _projectId: _data.projectId,
3811             _tokenCount: _amount,
3812             _beneficiary: _data.beneficiary,
3813             _memo: _data.memo,
3814             _preferClaimedTokens: _data.preferClaimedTokens,
3815             _useReservedRate: true
3816         });



    
3819         jbxTerminal.addToBalanceOf{value: _data.amount.value}(
3820             _data.projectId, _data.amount.value, JBTokens.ETH, "", new bytes(0)
3821         );



    
3679             if (_swap(_data, _minimumReceivedFromSwap, _reservedRate)== 0) _mint(_data, _tokenCount);



    
3819         jbxTerminal.addToBalanceOf{value: _data.amount.value}(
3820             _data.projectId, _data.amount.value, JBTokens.ETH, "", new bytes(0)
3821         );



    
3823         emit JBXBuybackDelegate_Mint(_data.projectId);



    
3679             if (_swap(_data, _minimumReceivedFromSwap, _reservedRate)== 0) _mint(_data, _tokenCount);



```

```
Reentrancy in JBXBuybackDelegate._mint(JBDidPayData,uint256) (JBXBuybackDelegate.sol#3806-3824):
	External calls:
	- IJBController(jbxTerminal.directory().controllerOf(_data.projectId)).mintTokensOf(_data.projectId,_amount,_data.beneficiary,_data.memo,_data.preferClaimedTokens,true) (JBXBuybackDelegate.sol#3809-3816)
	- jbxTerminal.addToBalanceOf{value: _data.amount.value}(_data.projectId,_data.amount.value,JBTokens.ETH,,new bytes(0)) (JBXBuybackDelegate.sol#3819-3821)
	External calls sending eth:
	- jbxTerminal.addToBalanceOf{value: _data.amount.value}(_data.projectId,_data.amount.value,JBTokens.ETH,,new bytes(0)) (JBXBuybackDelegate.sol#3819-3821)
	Event emitted after the call(s):
	- JBXBuybackDelegate_Mint(_data.projectId) (JBXBuybackDelegate.sol#3823)



    
3809         IJBController(jbxTerminal.directory().controllerOf(_data.projectId)).mintTokensOf({
3810             _projectId: _data.projectId,
3811             _tokenCount: _amount,
3812             _beneficiary: _data.beneficiary,
3813             _memo: _data.memo,
3814             _preferClaimedTokens: _data.preferClaimedTokens,
3815             _useReservedRate: true
3816         });



    
3819         jbxTerminal.addToBalanceOf{value: _data.amount.value}(
3820             _data.projectId, _data.amount.value, JBTokens.ETH, "", new bytes(0)
3821         );



    
3819         jbxTerminal.addToBalanceOf{value: _data.amount.value}(
3820             _data.projectId, _data.amount.value, JBTokens.ETH, "", new bytes(0)
3821         );



    
3823         emit JBXBuybackDelegate_Mint(_data.projectId);



```

## assembly
### Severity: Informational

### JBXBuybackDelegate.sol


```
TickMath.getTickAtSqrtRatio(uint160) (JBXBuybackDelegate.sol#3342-3487) uses assembly
	- INLINE ASM (JBXBuybackDelegate.sol#3351-3355)
	- INLINE ASM (JBXBuybackDelegate.sol#3356-3360)
	- INLINE ASM (JBXBuybackDelegate.sol#3361-3365)
	- INLINE ASM (JBXBuybackDelegate.sol#3366-3370)
	- INLINE ASM (JBXBuybackDelegate.sol#3371-3375)
	- INLINE ASM (JBXBuybackDelegate.sol#3376-3380)
	- INLINE ASM (JBXBuybackDelegate.sol#3381-3385)
	- INLINE ASM (JBXBuybackDelegate.sol#3386-3389)
	- INLINE ASM (JBXBuybackDelegate.sol#3396-3401)
	- INLINE ASM (JBXBuybackDelegate.sol#3402-3407)
	- INLINE ASM (JBXBuybackDelegate.sol#3408-3413)
	- INLINE ASM (JBXBuybackDelegate.sol#3414-3419)
	- INLINE ASM (JBXBuybackDelegate.sol#3420-3425)
	- INLINE ASM (JBXBuybackDelegate.sol#3426-3431)
	- INLINE ASM (JBXBuybackDelegate.sol#3432-3437)
	- INLINE ASM (JBXBuybackDelegate.sol#3438-3443)
	- INLINE ASM (JBXBuybackDelegate.sol#3444-3449)
	- INLINE ASM (JBXBuybackDelegate.sol#3450-3455)
	- INLINE ASM (JBXBuybackDelegate.sol#3456-3461)
	- INLINE ASM (JBXBuybackDelegate.sol#3462-3467)
	- INLINE ASM (JBXBuybackDelegate.sol#3468-3473)
	- INLINE ASM (JBXBuybackDelegate.sol#3474-3478)



    
3351             assembly {
3352                 let f := shl(7, gt(r, 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF))
3353                 msb := or(msb, f)
3354                 r := shr(f, r)
3355             }



    
3356             assembly {
3357                 let f := shl(6, gt(r, 0xFFFFFFFFFFFFFFFF))
3358                 msb := or(msb, f)
3359                 r := shr(f, r)
3360             }



    
3361             assembly {
3362                 let f := shl(5, gt(r, 0xFFFFFFFF))
3363                 msb := or(msb, f)
3364                 r := shr(f, r)
3365             }



    
3366             assembly {
3367                 let f := shl(4, gt(r, 0xFFFF))
3368                 msb := or(msb, f)
3369                 r := shr(f, r)
3370             }



    
3371             assembly {
3372                 let f := shl(3, gt(r, 0xFF))
3373                 msb := or(msb, f)
3374                 r := shr(f, r)
3375             }



    
3376             assembly {
3377                 let f := shl(2, gt(r, 0xF))
3378                 msb := or(msb, f)
3379                 r := shr(f, r)
3380             }



    
3381             assembly {
3382                 let f := shl(1, gt(r, 0x3))
3383                 msb := or(msb, f)
3384                 r := shr(f, r)
3385             }



    
3386             assembly {
3387                 let f := gt(r, 0x1)
3388                 msb := or(msb, f)
3389             }



    
3396             assembly {
3397                 r := shr(127, mul(r, r))
3398                 let f := shr(128, r)
3399                 log_2 := or(log_2, shl(63, f))
3400                 r := shr(f, r)
3401             }



    
3402             assembly {
3403                 r := shr(127, mul(r, r))
3404                 let f := shr(128, r)
3405                 log_2 := or(log_2, shl(62, f))
3406                 r := shr(f, r)
3407             }



    
3408             assembly {
3409                 r := shr(127, mul(r, r))
3410                 let f := shr(128, r)
3411                 log_2 := or(log_2, shl(61, f))
3412                 r := shr(f, r)
3413             }



    
3414             assembly {
3415                 r := shr(127, mul(r, r))
3416                 let f := shr(128, r)
3417                 log_2 := or(log_2, shl(60, f))
3418                 r := shr(f, r)
3419             }



    
3420             assembly {
3421                 r := shr(127, mul(r, r))
3422                 let f := shr(128, r)
3423                 log_2 := or(log_2, shl(59, f))
3424                 r := shr(f, r)
3425             }



    
3426             assembly {
3427                 r := shr(127, mul(r, r))
3428                 let f := shr(128, r)
3429                 log_2 := or(log_2, shl(58, f))
3430                 r := shr(f, r)
3431             }



    
3432             assembly {
3433                 r := shr(127, mul(r, r))
3434                 let f := shr(128, r)
3435                 log_2 := or(log_2, shl(57, f))
3436                 r := shr(f, r)
3437             }



    
3438             assembly {
3439                 r := shr(127, mul(r, r))
3440                 let f := shr(128, r)
3441                 log_2 := or(log_2, shl(56, f))
3442                 r := shr(f, r)
3443             }



    
3444             assembly {
3445                 r := shr(127, mul(r, r))
3446                 let f := shr(128, r)
3447                 log_2 := or(log_2, shl(55, f))
3448                 r := shr(f, r)
3449             }



    
3450             assembly {
3451                 r := shr(127, mul(r, r))
3452                 let f := shr(128, r)
3453                 log_2 := or(log_2, shl(54, f))
3454                 r := shr(f, r)
3455             }



    
3456             assembly {
3457                 r := shr(127, mul(r, r))
3458                 let f := shr(128, r)
3459                 log_2 := or(log_2, shl(53, f))
3460                 r := shr(f, r)
3461             }



    
3462             assembly {
3463                 r := shr(127, mul(r, r))
3464                 let f := shr(128, r)
3465                 log_2 := or(log_2, shl(52, f))
3466                 r := shr(f, r)
3467             }



    
3468             assembly {
3469                 r := shr(127, mul(r, r))
3470                 let f := shr(128, r)
3471                 log_2 := or(log_2, shl(51, f))
3472                 r := shr(f, r)
3473             }



    
3474             assembly {
3475                 r := shr(127, mul(r, r))
3476                 let f := shr(128, r)
3477                 log_2 := or(log_2, shl(50, f))
3478             }



```

```
PRBMath.mulDivSigned(int256,int256,int256) (JBXBuybackDelegate.sol#2700-2738) uses assembly
	- INLINE ASM (JBXBuybackDelegate.sol#2729-2733)



    
2729         assembly {
2730             sx := sgt(x, sub(0, 1))
2731             sy := sgt(y, sub(0, 1))
2732             sd := sgt(denominator, sub(0, 1))
2733         }



```

```
PRBMath.mulDiv(uint256,uint256,uint256) (JBXBuybackDelegate.sol#2543-2627) uses assembly
	- INLINE ASM (JBXBuybackDelegate.sol#2553-2557)
	- INLINE ASM (JBXBuybackDelegate.sol#2578-2585)
	- INLINE ASM (JBXBuybackDelegate.sol#2592-2601)



    
2553         assembly {
2554             let mm := mulmod(x, y, not(0))
2555             prod0 := mul(x, y)
2556             prod1 := sub(sub(mm, prod0), lt(mm, prod0))
2557         }



    
2578         assembly {
2579             // Compute remainder using mulmod.
2580             remainder := mulmod(x, y, denominator)
2581 
2582             // Subtract 256 bit number from 512 bit number.
2583             prod1 := sub(prod1, gt(remainder, prod0))
2584             prod0 := sub(prod0, remainder)
2585         }



    
2592             assembly {
2593                 // Divide denominator by lpotdod.
2594                 denominator := div(denominator, lpotdod)
2595 
2596                 // Divide [prod1 prod0] by lpotdod.
2597                 prod0 := div(prod0, lpotdod)
2598 
2599                 // Flip lpotdod such that it is 2^256 / lpotdod. If lpotdod is zero, then it becomes one.
2600                 lpotdod := add(div(sub(0, lpotdod), lpotdod), 1)
2601             }



```

```
PRBMath.mulDivFixedPoint(uint256,uint256) (JBXBuybackDelegate.sol#2647-2686) uses assembly
	- INLINE ASM (JBXBuybackDelegate.sol#2650-2654)
	- INLINE ASM (JBXBuybackDelegate.sol#2662-2665)
	- INLINE ASM (JBXBuybackDelegate.sol#2674-2685)



    
2650         assembly {
2651             let mm := mulmod(x, y, not(0))
2652             prod0 := mul(x, y)
2653             prod1 := sub(sub(mm, prod0), lt(mm, prod0))
2654         }



    
2662         assembly {
2663             remainder := mulmod(x, y, SCALE)
2664             roundUpUnit := gt(remainder, 499999999999999999)
2665         }



    
2674         assembly {
2675             result := add(
2676                 mul(
2677                     or(
2678                         div(sub(prod0, remainder), SCALE_LPOTD),
2679                         mul(sub(prod1, gt(remainder, prod0)), add(div(sub(0, SCALE_LPOTD), SCALE_LPOTD), 1))
2680                     ),
2681                     SCALE_INVERSE
2682                 ),
2683                 roundUpUnit
2684             )
2685         }



```

## cyclomatic-complexity
### Severity: Informational

### JBXBuybackDelegate.sol


```
TickMath.getSqrtRatioAtTick(int24) (JBXBuybackDelegate.sol#3300-3335) has a high cyclomatic complexity (25).



    
3300     function getSqrtRatioAtTick(int24 tick) internal pure returns (uint160 sqrtPriceX96) {
3301         unchecked {
3302             uint256 absTick = tick < 0 ? uint256(-int256(tick)) : uint256(int256(tick));
3303             if (absTick > uint256(int256(MAX_TICK))) revert T();
3304 
3305             uint256 ratio = absTick & 0x1 != 0
3306                 ? 0xfffcb933bd6fad37aa2d162d1a594001
3307                 : 0x100000000000000000000000000000000;
3308             if (absTick & 0x2 != 0) ratio = (ratio * 0xfff97272373d413259a46990580e213a) >> 128;
3309             if (absTick & 0x4 != 0) ratio = (ratio * 0xfff2e50f5f656932ef12357cf3c7fdcc) >> 128;
3310             if (absTick & 0x8 != 0) ratio = (ratio * 0xffe5caca7e10e4e61c3624eaa0941cd0) >> 128;
3311             if (absTick & 0x10 != 0) ratio = (ratio * 0xffcb9843d60f6159c9db58835c926644) >> 128;
3312             if (absTick & 0x20 != 0) ratio = (ratio * 0xff973b41fa98c081472e6896dfb254c0) >> 128;
3313             if (absTick & 0x40 != 0) ratio = (ratio * 0xff2ea16466c96a3843ec78b326b52861) >> 128;
3314             if (absTick & 0x80 != 0) ratio = (ratio * 0xfe5dee046a99a2a811c461f1969c3053) >> 128;
3315             if (absTick & 0x100 != 0) ratio = (ratio * 0xfcbe86c7900a88aedcffc83b479aa3a4) >> 128;
3316             if (absTick & 0x200 != 0) ratio = (ratio * 0xf987a7253ac413176f2b074cf7815e54) >> 128;
3317             if (absTick & 0x400 != 0) ratio = (ratio * 0xf3392b0822b70005940c7a398e4b70f3) >> 128;
3318             if (absTick & 0x800 != 0) ratio = (ratio * 0xe7159475a2c29b7443b29c7fa6e889d9) >> 128;
3319             if (absTick & 0x1000 != 0) ratio = (ratio * 0xd097f3bdfd2022b8845ad8f792aa5825) >> 128;
3320             if (absTick & 0x2000 != 0) ratio = (ratio * 0xa9f746462d870fdf8a65dc1f90e061e5) >> 128;
3321             if (absTick & 0x4000 != 0) ratio = (ratio * 0x70d869a156d2a1b890bb3df62baf32f7) >> 128;
3322             if (absTick & 0x8000 != 0) ratio = (ratio * 0x31be135f97d08fd981231505542fcfa6) >> 128;
3323             if (absTick & 0x10000 != 0) ratio = (ratio * 0x9aa508b5b7a84e1c677de54f3e99bc9) >> 128;
3324             if (absTick & 0x20000 != 0) ratio = (ratio * 0x5d6af8dedb81196699c329225ee604) >> 128;
3325             if (absTick & 0x40000 != 0) ratio = (ratio * 0x2216e584f5fa1ea926041bedfe98) >> 128;
3326             if (absTick & 0x80000 != 0) ratio = (ratio * 0x48a170391f7dc42444e8fa2) >> 128;
3327 
3328             if (tick > 0) ratio = type(uint256).max / ratio;
3329 
3330             // this divides by 1<<32 rounding up to go from a Q128.128 to a Q128.96.
3331             // we then downcast because we know the result always fits within 160 bits due to our tick input constraint
3332             // we round up in the division so getTickAtSqrtRatio of the output price is always consistent
3333             sqrtPriceX96 = uint160((ratio >> 32) + (ratio % (1 << 32) == 0 ? 0 : 1));
3334         }
3335     }



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) has a high cyclomatic complexity (65).



    
2276     function exp2(uint256 x) internal pure returns (uint256 result) {
2277         unchecked {
2278             // Start from 0.5 in the 192.64-bit fixed-point format.
2279             result = 0x800000000000000000000000000000000000000000000000;
2280 
2281             // Multiply the result by root(2, 2^-i) when the bit at position i is 1. None of the intermediary results overflows
2282             // because the initial result is 2^191 and all magic factors are less than 2^65.
2283             if (x & 0x8000000000000000 > 0) {
2284                 result = (result * 0x16A09E667F3BCC909) >> 64;
2285             }
2286             if (x & 0x4000000000000000 > 0) {
2287                 result = (result * 0x1306FE0A31B7152DF) >> 64;
2288             }
2289             if (x & 0x2000000000000000 > 0) {
2290                 result = (result * 0x1172B83C7D517ADCE) >> 64;
2291             }
2292             if (x & 0x1000000000000000 > 0) {
2293                 result = (result * 0x10B5586CF9890F62A) >> 64;
2294             }
2295             if (x & 0x800000000000000 > 0) {
2296                 result = (result * 0x1059B0D31585743AE) >> 64;
2297             }
2298             if (x & 0x400000000000000 > 0) {
2299                 result = (result * 0x102C9A3E778060EE7) >> 64;
2300             }
2301             if (x & 0x200000000000000 > 0) {
2302                 result = (result * 0x10163DA9FB33356D8) >> 64;
2303             }
2304             if (x & 0x100000000000000 > 0) {
2305                 result = (result * 0x100B1AFA5ABCBED61) >> 64;
2306             }
2307             if (x & 0x80000000000000 > 0) {
2308                 result = (result * 0x10058C86DA1C09EA2) >> 64;
2309             }
2310             if (x & 0x40000000000000 > 0) {
2311                 result = (result * 0x1002C605E2E8CEC50) >> 64;
2312             }
2313             if (x & 0x20000000000000 > 0) {
2314                 result = (result * 0x100162F3904051FA1) >> 64;
2315             }
2316             if (x & 0x10000000000000 > 0) {
2317                 result = (result * 0x1000B175EFFDC76BA) >> 64;
2318             }
2319             if (x & 0x8000000000000 > 0) {
2320                 result = (result * 0x100058BA01FB9F96D) >> 64;
2321             }
2322             if (x & 0x4000000000000 > 0) {
2323                 result = (result * 0x10002C5CC37DA9492) >> 64;
2324             }
2325             if (x & 0x2000000000000 > 0) {
2326                 result = (result * 0x1000162E525EE0547) >> 64;
2327             }
2328             if (x & 0x1000000000000 > 0) {
2329                 result = (result * 0x10000B17255775C04) >> 64;
2330             }
2331             if (x & 0x800000000000 > 0) {
2332                 result = (result * 0x1000058B91B5BC9AE) >> 64;
2333             }
2334             if (x & 0x400000000000 > 0) {
2335                 result = (result * 0x100002C5C89D5EC6D) >> 64;
2336             }
2337             if (x & 0x200000000000 > 0) {
2338                 result = (result * 0x10000162E43F4F831) >> 64;
2339             }
2340             if (x & 0x100000000000 > 0) {
2341                 result = (result * 0x100000B1721BCFC9A) >> 64;
2342             }
2343             if (x & 0x80000000000 > 0) {
2344                 result = (result * 0x10000058B90CF1E6E) >> 64;
2345             }
2346             if (x & 0x40000000000 > 0) {
2347                 result = (result * 0x1000002C5C863B73F) >> 64;
2348             }
2349             if (x & 0x20000000000 > 0) {
2350                 result = (result * 0x100000162E430E5A2) >> 64;
2351             }
2352             if (x & 0x10000000000 > 0) {
2353                 result = (result * 0x1000000B172183551) >> 64;
2354             }
2355             if (x & 0x8000000000 > 0) {
2356                 result = (result * 0x100000058B90C0B49) >> 64;
2357             }
2358             if (x & 0x4000000000 > 0) {
2359                 result = (result * 0x10000002C5C8601CC) >> 64;
2360             }
2361             if (x & 0x2000000000 > 0) {
2362                 result = (result * 0x1000000162E42FFF0) >> 64;
2363             }
2364             if (x & 0x1000000000 > 0) {
2365                 result = (result * 0x10000000B17217FBB) >> 64;
2366             }
2367             if (x & 0x800000000 > 0) {
2368                 result = (result * 0x1000000058B90BFCE) >> 64;
2369             }
2370             if (x & 0x400000000 > 0) {
2371                 result = (result * 0x100000002C5C85FE3) >> 64;
2372             }
2373             if (x & 0x200000000 > 0) {
2374                 result = (result * 0x10000000162E42FF1) >> 64;
2375             }
2376             if (x & 0x100000000 > 0) {
2377                 result = (result * 0x100000000B17217F8) >> 64;
2378             }
2379             if (x & 0x80000000 > 0) {
2380                 result = (result * 0x10000000058B90BFC) >> 64;
2381             }
2382             if (x & 0x40000000 > 0) {
2383                 result = (result * 0x1000000002C5C85FE) >> 64;
2384             }
2385             if (x & 0x20000000 > 0) {
2386                 result = (result * 0x100000000162E42FF) >> 64;
2387             }
2388             if (x & 0x10000000 > 0) {
2389                 result = (result * 0x1000000000B17217F) >> 64;
2390             }
2391             if (x & 0x8000000 > 0) {
2392                 result = (result * 0x100000000058B90C0) >> 64;
2393             }
2394             if (x & 0x4000000 > 0) {
2395                 result = (result * 0x10000000002C5C860) >> 64;
2396             }
2397             if (x & 0x2000000 > 0) {
2398                 result = (result * 0x1000000000162E430) >> 64;
2399             }
2400             if (x & 0x1000000 > 0) {
2401                 result = (result * 0x10000000000B17218) >> 64;
2402             }
2403             if (x & 0x800000 > 0) {
2404                 result = (result * 0x1000000000058B90C) >> 64;
2405             }
2406             if (x & 0x400000 > 0) {
2407                 result = (result * 0x100000000002C5C86) >> 64;
2408             }
2409             if (x & 0x200000 > 0) {
2410                 result = (result * 0x10000000000162E43) >> 64;
2411             }
2412             if (x & 0x100000 > 0) {
2413                 result = (result * 0x100000000000B1721) >> 64;
2414             }
2415             if (x & 0x80000 > 0) {
2416                 result = (result * 0x10000000000058B91) >> 64;
2417             }
2418             if (x & 0x40000 > 0) {
2419                 result = (result * 0x1000000000002C5C8) >> 64;
2420             }
2421             if (x & 0x20000 > 0) {
2422                 result = (result * 0x100000000000162E4) >> 64;
2423             }
2424             if (x & 0x10000 > 0) {
2425                 result = (result * 0x1000000000000B172) >> 64;
2426             }
2427             if (x & 0x8000 > 0) {
2428                 result = (result * 0x100000000000058B9) >> 64;
2429             }
2430             if (x & 0x4000 > 0) {
2431                 result = (result * 0x10000000000002C5D) >> 64;
2432             }
2433             if (x & 0x2000 > 0) {
2434                 result = (result * 0x1000000000000162E) >> 64;
2435             }
2436             if (x & 0x1000 > 0) {
2437                 result = (result * 0x10000000000000B17) >> 64;
2438             }
2439             if (x & 0x800 > 0) {
2440                 result = (result * 0x1000000000000058C) >> 64;
2441             }
2442             if (x & 0x400 > 0) {
2443                 result = (result * 0x100000000000002C6) >> 64;
2444             }
2445             if (x & 0x200 > 0) {
2446                 result = (result * 0x10000000000000163) >> 64;
2447             }
2448             if (x & 0x100 > 0) {
2449                 result = (result * 0x100000000000000B1) >> 64;
2450             }
2451             if (x & 0x80 > 0) {
2452                 result = (result * 0x10000000000000059) >> 64;
2453             }
2454             if (x & 0x40 > 0) {
2455                 result = (result * 0x1000000000000002C) >> 64;
2456             }
2457             if (x & 0x20 > 0) {
2458                 result = (result * 0x10000000000000016) >> 64;
2459             }
2460             if (x & 0x10 > 0) {
2461                 result = (result * 0x1000000000000000B) >> 64;
2462             }
2463             if (x & 0x8 > 0) {
2464                 result = (result * 0x10000000000000006) >> 64;
2465             }
2466             if (x & 0x4 > 0) {
2467                 result = (result * 0x10000000000000003) >> 64;
2468             }
2469             if (x & 0x2 > 0) {
2470                 result = (result * 0x10000000000000001) >> 64;
2471             }
2472             if (x & 0x1 > 0) {
2473                 result = (result * 0x10000000000000001) >> 64;
2474             }
2475 
2476             // We're doing two things at the same time:
2477             //
2478             //   1. Multiply the result by 2^n + 1, where "2^n" is the integer part and the one is added to account for
2479             //      the fact that we initially set the result to 0.5. This is accomplished by subtracting from 191
2480             //      rather than 192.
2481             //   2. Convert the result to the unsigned 60.18-decimal fixed-point format.
2482             //
2483             // This works because 2^(191-ip) = 2^ip / 2^191, where "ip" is the integer part "2^n".
2484             result *= SCALE;
2485             result >>= (191 - (x >> 64));
2486         }
2487     }



```

```
JBFundingCycleMetadataResolver.packFundingCycleMetadata(JBFundingCycleMetadata) (JBXBuybackDelegate.sol#1876-1923) has a high cyclomatic complexity (13).



    
1876   function packFundingCycleMetadata(JBFundingCycleMetadata memory _metadata)
1877     internal
1878     pure
1879     returns (uint256 packed)
1880   {
1881     // version 1 in the bits 0-7 (8 bits).
1882     packed = 1;
1883     // global metadta in bits 8-23 (16 bits).
1884     packed |=
1885       JBGlobalFundingCycleMetadataResolver.packFundingCycleGlobalMetadata(_metadata.global) <<
1886       8;
1887     // reserved rate in bits 24-39 (16 bits).
1888     packed |= _metadata.reservedRate << 24;
1889     // redemption rate in bits 40-55 (16 bits).
1890     // redemption rate is a number 0-10000. Store the reverse so the most common case of 100% results in no storage needs.
1891     packed |= (JBConstants.MAX_REDEMPTION_RATE - _metadata.redemptionRate) << 40;
1892     // ballot redemption rate rate in bits 56-71 (16 bits).
1893     // ballot redemption rate is a number 0-10000. Store the reverse so the most common case of 100% results in no storage needs.
1894     packed |= (JBConstants.MAX_REDEMPTION_RATE - _metadata.ballotRedemptionRate) << 56;
1895     // pause pay in bit 72.
1896     if (_metadata.pausePay) packed |= 1 << 72;
1897     // pause tap in bit 73.
1898     if (_metadata.pauseDistributions) packed |= 1 << 73;
1899     // pause redeem in bit 74.
1900     if (_metadata.pauseRedeem) packed |= 1 << 74;
1901     // pause burn in bit 75.
1902     if (_metadata.pauseBurn) packed |= 1 << 75;
1903     // allow minting in bit 76.
1904     if (_metadata.allowMinting) packed |= 1 << 76;
1905     // allow terminal migration in bit 77.
1906     if (_metadata.allowTerminalMigration) packed |= 1 << 77;
1907     // allow controller migration in bit 78.
1908     if (_metadata.allowControllerMigration) packed |= 1 << 78;
1909     // hold fees in bit 79.
1910     if (_metadata.holdFees) packed |= 1 << 79;
1911     // prefer claimed token override in bit 80.
1912     if (_metadata.preferClaimedTokenOverride) packed |= 1 << 80;
1913     // useTotalOverflowForRedemptions in bit 81.
1914     if (_metadata.useTotalOverflowForRedemptions) packed |= 1 << 81;
1915     // use pay data source in bit 82.
1916     if (_metadata.useDataSourceForPay) packed |= 1 << 82;
1917     // use redeem data source in bit 83.
1918     if (_metadata.useDataSourceForRedeem) packed |= 1 << 83;
1919     // data source address in bits 84-243.
1920     packed |= uint256(uint160(address(_metadata.dataSource))) << 84;
1921     // metadata in bits 244-252 (8 bits).
1922     packed |= _metadata.metadata << 244;
1923   }



```

## dead-code
### Severity: Informational

### JBXBuybackDelegate.sol


```
TickMath.getSqrtRatioAtTick(int24) (JBXBuybackDelegate.sol#3300-3335) is never used and should be removed



    
3300     function getSqrtRatioAtTick(int24 tick) internal pure returns (uint160 sqrtPriceX96) {
3301         unchecked {
3302             uint256 absTick = tick < 0 ? uint256(-int256(tick)) : uint256(int256(tick));
3303             if (absTick > uint256(int256(MAX_TICK))) revert T();
3304 
3305             uint256 ratio = absTick & 0x1 != 0
3306                 ? 0xfffcb933bd6fad37aa2d162d1a594001
3307                 : 0x100000000000000000000000000000000;
3308             if (absTick & 0x2 != 0) ratio = (ratio * 0xfff97272373d413259a46990580e213a) >> 128;
3309             if (absTick & 0x4 != 0) ratio = (ratio * 0xfff2e50f5f656932ef12357cf3c7fdcc) >> 128;
3310             if (absTick & 0x8 != 0) ratio = (ratio * 0xffe5caca7e10e4e61c3624eaa0941cd0) >> 128;
3311             if (absTick & 0x10 != 0) ratio = (ratio * 0xffcb9843d60f6159c9db58835c926644) >> 128;
3312             if (absTick & 0x20 != 0) ratio = (ratio * 0xff973b41fa98c081472e6896dfb254c0) >> 128;
3313             if (absTick & 0x40 != 0) ratio = (ratio * 0xff2ea16466c96a3843ec78b326b52861) >> 128;
3314             if (absTick & 0x80 != 0) ratio = (ratio * 0xfe5dee046a99a2a811c461f1969c3053) >> 128;
3315             if (absTick & 0x100 != 0) ratio = (ratio * 0xfcbe86c7900a88aedcffc83b479aa3a4) >> 128;
3316             if (absTick & 0x200 != 0) ratio = (ratio * 0xf987a7253ac413176f2b074cf7815e54) >> 128;
3317             if (absTick & 0x400 != 0) ratio = (ratio * 0xf3392b0822b70005940c7a398e4b70f3) >> 128;
3318             if (absTick & 0x800 != 0) ratio = (ratio * 0xe7159475a2c29b7443b29c7fa6e889d9) >> 128;
3319             if (absTick & 0x1000 != 0) ratio = (ratio * 0xd097f3bdfd2022b8845ad8f792aa5825) >> 128;
3320             if (absTick & 0x2000 != 0) ratio = (ratio * 0xa9f746462d870fdf8a65dc1f90e061e5) >> 128;
3321             if (absTick & 0x4000 != 0) ratio = (ratio * 0x70d869a156d2a1b890bb3df62baf32f7) >> 128;
3322             if (absTick & 0x8000 != 0) ratio = (ratio * 0x31be135f97d08fd981231505542fcfa6) >> 128;
3323             if (absTick & 0x10000 != 0) ratio = (ratio * 0x9aa508b5b7a84e1c677de54f3e99bc9) >> 128;
3324             if (absTick & 0x20000 != 0) ratio = (ratio * 0x5d6af8dedb81196699c329225ee604) >> 128;
3325             if (absTick & 0x40000 != 0) ratio = (ratio * 0x2216e584f5fa1ea926041bedfe98) >> 128;
3326             if (absTick & 0x80000 != 0) ratio = (ratio * 0x48a170391f7dc42444e8fa2) >> 128;
3327 
3328             if (tick > 0) ratio = type(uint256).max / ratio;
3329 
3330             // this divides by 1<<32 rounding up to go from a Q128.128 to a Q128.96.
3331             // we then downcast because we know the result always fits within 160 bits due to our tick input constraint
3332             // we round up in the division so getTickAtSqrtRatio of the output price is always consistent
3333             sqrtPriceX96 = uint160((ratio >> 32) + (ratio % (1 << 32) == 0 ? 0 : 1));
3334         }
3335     }



```

```
JBFundingCycleMetadataResolver.shouldHoldFees(JBFundingCycle) (JBXBuybackDelegate.sol#1828-1830) is never used and should be removed



    
1828   function shouldHoldFees(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1829     return ((_fundingCycle.metadata >> 79) & 1) == 1;
1830   }



```

```
JBGlobalFundingCycleMetadataResolver.transfersPaused(uint8) (JBXBuybackDelegate.sol#1718-1720) is never used and should be removed



    
1718   function transfersPaused(uint8 _data) internal pure returns (bool) {
1719     return ((_data >> 2) & 1) == 1;
1720   }



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) is never used and should be removed



    
2276     function exp2(uint256 x) internal pure returns (uint256 result) {
2277         unchecked {
2278             // Start from 0.5 in the 192.64-bit fixed-point format.
2279             result = 0x800000000000000000000000000000000000000000000000;
2280 
2281             // Multiply the result by root(2, 2^-i) when the bit at position i is 1. None of the intermediary results overflows
2282             // because the initial result is 2^191 and all magic factors are less than 2^65.
2283             if (x & 0x8000000000000000 > 0) {
2284                 result = (result * 0x16A09E667F3BCC909) >> 64;
2285             }
2286             if (x & 0x4000000000000000 > 0) {
2287                 result = (result * 0x1306FE0A31B7152DF) >> 64;
2288             }
2289             if (x & 0x2000000000000000 > 0) {
2290                 result = (result * 0x1172B83C7D517ADCE) >> 64;
2291             }
2292             if (x & 0x1000000000000000 > 0) {
2293                 result = (result * 0x10B5586CF9890F62A) >> 64;
2294             }
2295             if (x & 0x800000000000000 > 0) {
2296                 result = (result * 0x1059B0D31585743AE) >> 64;
2297             }
2298             if (x & 0x400000000000000 > 0) {
2299                 result = (result * 0x102C9A3E778060EE7) >> 64;
2300             }
2301             if (x & 0x200000000000000 > 0) {
2302                 result = (result * 0x10163DA9FB33356D8) >> 64;
2303             }
2304             if (x & 0x100000000000000 > 0) {
2305                 result = (result * 0x100B1AFA5ABCBED61) >> 64;
2306             }
2307             if (x & 0x80000000000000 > 0) {
2308                 result = (result * 0x10058C86DA1C09EA2) >> 64;
2309             }
2310             if (x & 0x40000000000000 > 0) {
2311                 result = (result * 0x1002C605E2E8CEC50) >> 64;
2312             }
2313             if (x & 0x20000000000000 > 0) {
2314                 result = (result * 0x100162F3904051FA1) >> 64;
2315             }
2316             if (x & 0x10000000000000 > 0) {
2317                 result = (result * 0x1000B175EFFDC76BA) >> 64;
2318             }
2319             if (x & 0x8000000000000 > 0) {
2320                 result = (result * 0x100058BA01FB9F96D) >> 64;
2321             }
2322             if (x & 0x4000000000000 > 0) {
2323                 result = (result * 0x10002C5CC37DA9492) >> 64;
2324             }
2325             if (x & 0x2000000000000 > 0) {
2326                 result = (result * 0x1000162E525EE0547) >> 64;
2327             }
2328             if (x & 0x1000000000000 > 0) {
2329                 result = (result * 0x10000B17255775C04) >> 64;
2330             }
2331             if (x & 0x800000000000 > 0) {
2332                 result = (result * 0x1000058B91B5BC9AE) >> 64;
2333             }
2334             if (x & 0x400000000000 > 0) {
2335                 result = (result * 0x100002C5C89D5EC6D) >> 64;
2336             }
2337             if (x & 0x200000000000 > 0) {
2338                 result = (result * 0x10000162E43F4F831) >> 64;
2339             }
2340             if (x & 0x100000000000 > 0) {
2341                 result = (result * 0x100000B1721BCFC9A) >> 64;
2342             }
2343             if (x & 0x80000000000 > 0) {
2344                 result = (result * 0x10000058B90CF1E6E) >> 64;
2345             }
2346             if (x & 0x40000000000 > 0) {
2347                 result = (result * 0x1000002C5C863B73F) >> 64;
2348             }
2349             if (x & 0x20000000000 > 0) {
2350                 result = (result * 0x100000162E430E5A2) >> 64;
2351             }
2352             if (x & 0x10000000000 > 0) {
2353                 result = (result * 0x1000000B172183551) >> 64;
2354             }
2355             if (x & 0x8000000000 > 0) {
2356                 result = (result * 0x100000058B90C0B49) >> 64;
2357             }
2358             if (x & 0x4000000000 > 0) {
2359                 result = (result * 0x10000002C5C8601CC) >> 64;
2360             }
2361             if (x & 0x2000000000 > 0) {
2362                 result = (result * 0x1000000162E42FFF0) >> 64;
2363             }
2364             if (x & 0x1000000000 > 0) {
2365                 result = (result * 0x10000000B17217FBB) >> 64;
2366             }
2367             if (x & 0x800000000 > 0) {
2368                 result = (result * 0x1000000058B90BFCE) >> 64;
2369             }
2370             if (x & 0x400000000 > 0) {
2371                 result = (result * 0x100000002C5C85FE3) >> 64;
2372             }
2373             if (x & 0x200000000 > 0) {
2374                 result = (result * 0x10000000162E42FF1) >> 64;
2375             }
2376             if (x & 0x100000000 > 0) {
2377                 result = (result * 0x100000000B17217F8) >> 64;
2378             }
2379             if (x & 0x80000000 > 0) {
2380                 result = (result * 0x10000000058B90BFC) >> 64;
2381             }
2382             if (x & 0x40000000 > 0) {
2383                 result = (result * 0x1000000002C5C85FE) >> 64;
2384             }
2385             if (x & 0x20000000 > 0) {
2386                 result = (result * 0x100000000162E42FF) >> 64;
2387             }
2388             if (x & 0x10000000 > 0) {
2389                 result = (result * 0x1000000000B17217F) >> 64;
2390             }
2391             if (x & 0x8000000 > 0) {
2392                 result = (result * 0x100000000058B90C0) >> 64;
2393             }
2394             if (x & 0x4000000 > 0) {
2395                 result = (result * 0x10000000002C5C860) >> 64;
2396             }
2397             if (x & 0x2000000 > 0) {
2398                 result = (result * 0x1000000000162E430) >> 64;
2399             }
2400             if (x & 0x1000000 > 0) {
2401                 result = (result * 0x10000000000B17218) >> 64;
2402             }
2403             if (x & 0x800000 > 0) {
2404                 result = (result * 0x1000000000058B90C) >> 64;
2405             }
2406             if (x & 0x400000 > 0) {
2407                 result = (result * 0x100000000002C5C86) >> 64;
2408             }
2409             if (x & 0x200000 > 0) {
2410                 result = (result * 0x10000000000162E43) >> 64;
2411             }
2412             if (x & 0x100000 > 0) {
2413                 result = (result * 0x100000000000B1721) >> 64;
2414             }
2415             if (x & 0x80000 > 0) {
2416                 result = (result * 0x10000000000058B91) >> 64;
2417             }
2418             if (x & 0x40000 > 0) {
2419                 result = (result * 0x1000000000002C5C8) >> 64;
2420             }
2421             if (x & 0x20000 > 0) {
2422                 result = (result * 0x100000000000162E4) >> 64;
2423             }
2424             if (x & 0x10000 > 0) {
2425                 result = (result * 0x1000000000000B172) >> 64;
2426             }
2427             if (x & 0x8000 > 0) {
2428                 result = (result * 0x100000000000058B9) >> 64;
2429             }
2430             if (x & 0x4000 > 0) {
2431                 result = (result * 0x10000000000002C5D) >> 64;
2432             }
2433             if (x & 0x2000 > 0) {
2434                 result = (result * 0x1000000000000162E) >> 64;
2435             }
2436             if (x & 0x1000 > 0) {
2437                 result = (result * 0x10000000000000B17) >> 64;
2438             }
2439             if (x & 0x800 > 0) {
2440                 result = (result * 0x1000000000000058C) >> 64;
2441             }
2442             if (x & 0x400 > 0) {
2443                 result = (result * 0x100000000000002C6) >> 64;
2444             }
2445             if (x & 0x200 > 0) {
2446                 result = (result * 0x10000000000000163) >> 64;
2447             }
2448             if (x & 0x100 > 0) {
2449                 result = (result * 0x100000000000000B1) >> 64;
2450             }
2451             if (x & 0x80 > 0) {
2452                 result = (result * 0x10000000000000059) >> 64;
2453             }
2454             if (x & 0x40 > 0) {
2455                 result = (result * 0x1000000000000002C) >> 64;
2456             }
2457             if (x & 0x20 > 0) {
2458                 result = (result * 0x10000000000000016) >> 64;
2459             }
2460             if (x & 0x10 > 0) {
2461                 result = (result * 0x1000000000000000B) >> 64;
2462             }
2463             if (x & 0x8 > 0) {
2464                 result = (result * 0x10000000000000006) >> 64;
2465             }
2466             if (x & 0x4 > 0) {
2467                 result = (result * 0x10000000000000003) >> 64;
2468             }
2469             if (x & 0x2 > 0) {
2470                 result = (result * 0x10000000000000001) >> 64;
2471             }
2472             if (x & 0x1 > 0) {
2473                 result = (result * 0x10000000000000001) >> 64;
2474             }
2475 
2476             // We're doing two things at the same time:
2477             //
2478             //   1. Multiply the result by 2^n + 1, where "2^n" is the integer part and the one is added to account for
2479             //      the fact that we initially set the result to 0.5. This is accomplished by subtracting from 191
2480             //      rather than 192.
2481             //   2. Convert the result to the unsigned 60.18-decimal fixed-point format.
2482             //
2483             // This works because 2^(191-ip) = 2^ip / 2^191, where "ip" is the integer part "2^n".
2484             result *= SCALE;
2485             result >>= (191 - (x >> 64));
2486         }
2487     }



```

```
JBFundingCycleMetadataResolver.burnPaused(JBFundingCycle) (JBXBuybackDelegate.sol#1804-1806) is never used and should be removed



    
1804   function burnPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1805     return ((_fundingCycle.metadata >> 75) & 1) == 1;
1806   }



```

```
JBGlobalFundingCycleMetadataResolver.packFundingCycleGlobalMetadata(JBGlobalFundingCycleMetadata) (JBXBuybackDelegate.sol#1730-1741) is never used and should be removed



    
1730   function packFundingCycleGlobalMetadata(JBGlobalFundingCycleMetadata memory _metadata)
1731     internal
1732     pure
1733     returns (uint256 packed)
1734   {
1735     // allow set terminals in bit 0.
1736     if (_metadata.allowSetTerminals) packed |= 1;
1737     // allow set controller in bit 1.
1738     if (_metadata.allowSetController) packed |= 1 << 1;
1739     // pause transfers in bit 2.
1740     if (_metadata.pauseTransfers) packed |= 1 << 2;
1741   }



```

```
JBFundingCycleMetadataResolver.payPaused(JBFundingCycle) (JBXBuybackDelegate.sol#1792-1794) is never used and should be removed



    
1792   function payPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1793     return ((_fundingCycle.metadata >> 72) & 1) == 1;
1794   }



```

```
JBFundingCycleMetadataResolver.controllerMigrationAllowed(JBFundingCycle) (JBXBuybackDelegate.sol#1820-1826) is never used and should be removed



    
1820   function controllerMigrationAllowed(JBFundingCycle memory _fundingCycle)
1821     internal
1822     pure
1823     returns (bool)
1824   {
1825     return ((_fundingCycle.metadata >> 78) & 1) == 1;
1826   }



```

```
JBGlobalFundingCycleMetadataResolver.setControllerAllowed(uint8) (JBXBuybackDelegate.sol#1714-1716) is never used and should be removed



    
1714   function setControllerAllowed(uint8 _data) internal pure returns (bool) {
1715     return ((_data >> 1) & 1) == 1;
1716   }



```

```
JBFundingCycleMetadataResolver.distributionsPaused(JBFundingCycle) (JBXBuybackDelegate.sol#1796-1798) is never used and should be removed



    
1796   function distributionsPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1797     return ((_fundingCycle.metadata >> 73) & 1) == 1;
1798   }



```

```
JBGlobalFundingCycleMetadataResolver.expandMetadata(uint8) (JBXBuybackDelegate.sol#1751-1762) is never used and should be removed



    
1751   function expandMetadata(uint8 _packedMetadata)
1752     internal
1753     pure
1754     returns (JBGlobalFundingCycleMetadata memory metadata)
1755   {
1756     return
1757       JBGlobalFundingCycleMetadata(
1758         setTerminalsAllowed(_packedMetadata),
1759         setControllerAllowed(_packedMetadata),
1760         transfersPaused(_packedMetadata)
1761       );
1762   }



```

```
PRBMath.sqrt(uint256) (JBXBuybackDelegate.sol#2748-2796) is never used and should be removed



    
2748     function sqrt(uint256 x) internal pure returns (uint256 result) {
2749         if (x == 0) {
2750             return 0;
2751         }
2752 
2753         // Set the initial guess to the least power of two that is greater than or equal to sqrt(x).
2754         uint256 xAux = uint256(x);
2755         result = 1;
2756         if (xAux >= 0x100000000000000000000000000000000) {
2757             xAux >>= 128;
2758             result <<= 64;
2759         }
2760         if (xAux >= 0x10000000000000000) {
2761             xAux >>= 64;
2762             result <<= 32;
2763         }
2764         if (xAux >= 0x100000000) {
2765             xAux >>= 32;
2766             result <<= 16;
2767         }
2768         if (xAux >= 0x10000) {
2769             xAux >>= 16;
2770             result <<= 8;
2771         }
2772         if (xAux >= 0x100) {
2773             xAux >>= 8;
2774             result <<= 4;
2775         }
2776         if (xAux >= 0x10) {
2777             xAux >>= 4;
2778             result <<= 2;
2779         }
2780         if (xAux >= 0x8) {
2781             result <<= 1;
2782         }
2783 
2784         // The operations can never overflow because the result is max 2^127 when it enters this block.
2785         unchecked {
2786             result = (result + x / result) >> 1;
2787             result = (result + x / result) >> 1;
2788             result = (result + x / result) >> 1;
2789             result = (result + x / result) >> 1;
2790             result = (result + x / result) >> 1;
2791             result = (result + x / result) >> 1;
2792             result = (result + x / result) >> 1; // Seven iterations should be enough
2793             uint256 roundedDownResult = x / result;
2794             return result >= roundedDownResult ? roundedDownResult : result;
2795         }
2796     }



```

```
PRBMath.mulDivFixedPoint(uint256,uint256) (JBXBuybackDelegate.sol#2647-2686) is never used and should be removed



    
2647     function mulDivFixedPoint(uint256 x, uint256 y) internal pure returns (uint256 result) {
2648         uint256 prod0;
2649         uint256 prod1;
2650         assembly {
2651             let mm := mulmod(x, y, not(0))
2652             prod0 := mul(x, y)
2653             prod1 := sub(sub(mm, prod0), lt(mm, prod0))
2654         }
2655 
2656         if (prod1 >= SCALE) {
2657             revert PRBMath__MulDivFixedPointOverflow(prod1);
2658         }
2659 
2660         uint256 remainder;
2661         uint256 roundUpUnit;
2662         assembly {
2663             remainder := mulmod(x, y, SCALE)
2664             roundUpUnit := gt(remainder, 499999999999999999)
2665         }
2666 
2667         if (prod1 == 0) {
2668             unchecked {
2669                 result = (prod0 / SCALE) + roundUpUnit;
2670                 return result;
2671             }
2672         }
2673 
2674         assembly {
2675             result := add(
2676                 mul(
2677                     or(
2678                         div(sub(prod0, remainder), SCALE_LPOTD),
2679                         mul(sub(prod1, gt(remainder, prod0)), add(div(sub(0, SCALE_LPOTD), SCALE_LPOTD), 1))
2680                     ),
2681                     SCALE_INVERSE
2682                 ),
2683                 roundUpUnit
2684             )
2685         }
2686     }



```

```
JBFundingCycleMetadataResolver.reservedRate(JBFundingCycle) (JBXBuybackDelegate.sol#1774-1776) is never used and should be removed



    
1774   function reservedRate(JBFundingCycle memory _fundingCycle) internal pure returns (uint256) {
1775     return uint256(uint16(_fundingCycle.metadata >> 24));
1776   }



```

```
JBFundingCycleMetadataResolver.useDataSourceForRedeem(JBFundingCycle) (JBXBuybackDelegate.sol#1852-1858) is never used and should be removed



    
1852   function useDataSourceForRedeem(JBFundingCycle memory _fundingCycle)
1853     internal
1854     pure
1855     returns (bool)
1856   {
1857     return (_fundingCycle.metadata >> 83) & 1 == 1;
1858   }



```

```
JBFundingCycleMetadataResolver.useTotalOverflowForRedemptions(JBFundingCycle) (JBXBuybackDelegate.sol#1840-1846) is never used and should be removed



    
1840   function useTotalOverflowForRedemptions(JBFundingCycle memory _fundingCycle)
1841     internal
1842     pure
1843     returns (bool)
1844   {
1845     return ((_fundingCycle.metadata >> 81) & 1) == 1;
1846   }



```

```
JBFundingCycleMetadataResolver.metadata(JBFundingCycle) (JBXBuybackDelegate.sol#1864-1866) is never used and should be removed



    
1864   function metadata(JBFundingCycle memory _fundingCycle) internal pure returns (uint256) {
1865     return uint256(uint8(_fundingCycle.metadata >> 244));
1866   }



```

```
JBGlobalFundingCycleMetadataResolver.setTerminalsAllowed(uint8) (JBXBuybackDelegate.sol#1710-1712) is never used and should be removed



    
1710   function setTerminalsAllowed(uint8 _data) internal pure returns (bool) {
1711     return (_data & 1) == 1;
1712   }



```

```
TickMath.getTickAtSqrtRatio(uint160) (JBXBuybackDelegate.sol#3342-3487) is never used and should be removed



    
3342     function getTickAtSqrtRatio(uint160 sqrtPriceX96) internal pure returns (int24 tick) {
3343         unchecked {
3344             // second inequality must be < because the price can never reach the price at the max tick
3345             if (!(sqrtPriceX96 >= MIN_SQRT_RATIO && sqrtPriceX96 < MAX_SQRT_RATIO)) revert R();
3346             uint256 ratio = uint256(sqrtPriceX96) << 32;
3347 
3348             uint256 r = ratio;
3349             uint256 msb = 0;
3350 
3351             assembly {
3352                 let f := shl(7, gt(r, 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF))
3353                 msb := or(msb, f)
3354                 r := shr(f, r)
3355             }
3356             assembly {
3357                 let f := shl(6, gt(r, 0xFFFFFFFFFFFFFFFF))
3358                 msb := or(msb, f)
3359                 r := shr(f, r)
3360             }
3361             assembly {
3362                 let f := shl(5, gt(r, 0xFFFFFFFF))
3363                 msb := or(msb, f)
3364                 r := shr(f, r)
3365             }
3366             assembly {
3367                 let f := shl(4, gt(r, 0xFFFF))
3368                 msb := or(msb, f)
3369                 r := shr(f, r)
3370             }
3371             assembly {
3372                 let f := shl(3, gt(r, 0xFF))
3373                 msb := or(msb, f)
3374                 r := shr(f, r)
3375             }
3376             assembly {
3377                 let f := shl(2, gt(r, 0xF))
3378                 msb := or(msb, f)
3379                 r := shr(f, r)
3380             }
3381             assembly {
3382                 let f := shl(1, gt(r, 0x3))
3383                 msb := or(msb, f)
3384                 r := shr(f, r)
3385             }
3386             assembly {
3387                 let f := gt(r, 0x1)
3388                 msb := or(msb, f)
3389             }
3390 
3391             if (msb >= 128) r = ratio >> (msb - 127);
3392             else r = ratio << (127 - msb);
3393 
3394             int256 log_2 = (int256(msb) - 128) << 64;
3395 
3396             assembly {
3397                 r := shr(127, mul(r, r))
3398                 let f := shr(128, r)
3399                 log_2 := or(log_2, shl(63, f))
3400                 r := shr(f, r)
3401             }
3402             assembly {
3403                 r := shr(127, mul(r, r))
3404                 let f := shr(128, r)
3405                 log_2 := or(log_2, shl(62, f))
3406                 r := shr(f, r)
3407             }
3408             assembly {
3409                 r := shr(127, mul(r, r))
3410                 let f := shr(128, r)
3411                 log_2 := or(log_2, shl(61, f))
3412                 r := shr(f, r)
3413             }
3414             assembly {
3415                 r := shr(127, mul(r, r))
3416                 let f := shr(128, r)
3417                 log_2 := or(log_2, shl(60, f))
3418                 r := shr(f, r)
3419             }
3420             assembly {
3421                 r := shr(127, mul(r, r))
3422                 let f := shr(128, r)
3423                 log_2 := or(log_2, shl(59, f))
3424                 r := shr(f, r)
3425             }
3426             assembly {
3427                 r := shr(127, mul(r, r))
3428                 let f := shr(128, r)
3429                 log_2 := or(log_2, shl(58, f))
3430                 r := shr(f, r)
3431             }
3432             assembly {
3433                 r := shr(127, mul(r, r))
3434                 let f := shr(128, r)
3435                 log_2 := or(log_2, shl(57, f))
3436                 r := shr(f, r)
3437             }
3438             assembly {
3439                 r := shr(127, mul(r, r))
3440                 let f := shr(128, r)
3441                 log_2 := or(log_2, shl(56, f))
3442                 r := shr(f, r)
3443             }
3444             assembly {
3445                 r := shr(127, mul(r, r))
3446                 let f := shr(128, r)
3447                 log_2 := or(log_2, shl(55, f))
3448                 r := shr(f, r)
3449             }
3450             assembly {
3451                 r := shr(127, mul(r, r))
3452                 let f := shr(128, r)
3453                 log_2 := or(log_2, shl(54, f))
3454                 r := shr(f, r)
3455             }
3456             assembly {
3457                 r := shr(127, mul(r, r))
3458                 let f := shr(128, r)
3459                 log_2 := or(log_2, shl(53, f))
3460                 r := shr(f, r)
3461             }
3462             assembly {
3463                 r := shr(127, mul(r, r))
3464                 let f := shr(128, r)
3465                 log_2 := or(log_2, shl(52, f))
3466                 r := shr(f, r)
3467             }
3468             assembly {
3469                 r := shr(127, mul(r, r))
3470                 let f := shr(128, r)
3471                 log_2 := or(log_2, shl(51, f))
3472                 r := shr(f, r)
3473             }
3474             assembly {
3475                 r := shr(127, mul(r, r))
3476                 let f := shr(128, r)
3477                 log_2 := or(log_2, shl(50, f))
3478             }
3479 
3480             int256 log_sqrt10001 = log_2 * 255738958999603826347141; // 128.128 number
3481 
3482             int24 tickLow = int24((log_sqrt10001 - 3402992956809132418596140100660247210) >> 128);
3483             int24 tickHi = int24((log_sqrt10001 + 291339464771989622907027621153398088495) >> 128);
3484 
3485             tick = tickLow == tickHi ? tickLow : getSqrtRatioAtTick(tickHi) <= sqrtPriceX96 ? tickHi : tickLow;
3486         }
3487     }



```

```
JBFundingCycleMetadataResolver.packFundingCycleMetadata(JBFundingCycleMetadata) (JBXBuybackDelegate.sol#1876-1923) is never used and should be removed



    
1876   function packFundingCycleMetadata(JBFundingCycleMetadata memory _metadata)
1877     internal
1878     pure
1879     returns (uint256 packed)
1880   {
1881     // version 1 in the bits 0-7 (8 bits).
1882     packed = 1;
1883     // global metadta in bits 8-23 (16 bits).
1884     packed |=
1885       JBGlobalFundingCycleMetadataResolver.packFundingCycleGlobalMetadata(_metadata.global) <<
1886       8;
1887     // reserved rate in bits 24-39 (16 bits).
1888     packed |= _metadata.reservedRate << 24;
1889     // redemption rate in bits 40-55 (16 bits).
1890     // redemption rate is a number 0-10000. Store the reverse so the most common case of 100% results in no storage needs.
1891     packed |= (JBConstants.MAX_REDEMPTION_RATE - _metadata.redemptionRate) << 40;
1892     // ballot redemption rate rate in bits 56-71 (16 bits).
1893     // ballot redemption rate is a number 0-10000. Store the reverse so the most common case of 100% results in no storage needs.
1894     packed |= (JBConstants.MAX_REDEMPTION_RATE - _metadata.ballotRedemptionRate) << 56;
1895     // pause pay in bit 72.
1896     if (_metadata.pausePay) packed |= 1 << 72;
1897     // pause tap in bit 73.
1898     if (_metadata.pauseDistributions) packed |= 1 << 73;
1899     // pause redeem in bit 74.
1900     if (_metadata.pauseRedeem) packed |= 1 << 74;
1901     // pause burn in bit 75.
1902     if (_metadata.pauseBurn) packed |= 1 << 75;
1903     // allow minting in bit 76.
1904     if (_metadata.allowMinting) packed |= 1 << 76;
1905     // allow terminal migration in bit 77.
1906     if (_metadata.allowTerminalMigration) packed |= 1 << 77;
1907     // allow controller migration in bit 78.
1908     if (_metadata.allowControllerMigration) packed |= 1 << 78;
1909     // hold fees in bit 79.
1910     if (_metadata.holdFees) packed |= 1 << 79;
1911     // prefer claimed token override in bit 80.
1912     if (_metadata.preferClaimedTokenOverride) packed |= 1 << 80;
1913     // useTotalOverflowForRedemptions in bit 81.
1914     if (_metadata.useTotalOverflowForRedemptions) packed |= 1 << 81;
1915     // use pay data source in bit 82.
1916     if (_metadata.useDataSourceForPay) packed |= 1 << 82;
1917     // use redeem data source in bit 83.
1918     if (_metadata.useDataSourceForRedeem) packed |= 1 << 83;
1919     // data source address in bits 84-243.
1920     packed |= uint256(uint160(address(_metadata.dataSource))) << 84;
1921     // metadata in bits 244-252 (8 bits).
1922     packed |= _metadata.metadata << 244;
1923   }



```

```
PRBMath.mulDivSigned(int256,int256,int256) (JBXBuybackDelegate.sol#2700-2738) is never used and should be removed



    
2700     function mulDivSigned(
2701         int256 x,
2702         int256 y,
2703         int256 denominator
2704     ) internal pure returns (int256 result) {
2705         if (x == type(int256).min || y == type(int256).min || denominator == type(int256).min) {
2706             revert PRBMath__MulDivSignedInputTooSmall();
2707         }
2708 
2709         // Get hold of the absolute values of x, y and the denominator.
2710         uint256 ax;
2711         uint256 ay;
2712         uint256 ad;
2713         unchecked {
2714             ax = x < 0 ? uint256(-x) : uint256(x);
2715             ay = y < 0 ? uint256(-y) : uint256(y);
2716             ad = denominator < 0 ? uint256(-denominator) : uint256(denominator);
2717         }
2718 
2719         // Compute the absolute value of (x*y)÷denominator. The result must fit within int256.
2720         uint256 rAbs = mulDiv(ax, ay, ad);
2721         if (rAbs > uint256(type(int256).max)) {
2722             revert PRBMath__MulDivSignedOverflow(rAbs);
2723         }
2724 
2725         // Get the signs of x, y and the denominator.
2726         uint256 sx;
2727         uint256 sy;
2728         uint256 sd;
2729         assembly {
2730             sx := sgt(x, sub(0, 1))
2731             sy := sgt(y, sub(0, 1))
2732             sd := sgt(denominator, sub(0, 1))
2733         }
2734 
2735         // XOR over sx, sy and sd. This is checking whether there are one or three negative signs in the inputs.
2736         // If yes, the result should be negative.
2737         result = sx ^ sy ^ sd == 0 ? -int256(rAbs) : int256(rAbs);
2738     }



```

```
JBFundingCycleMetadataResolver.mintingAllowed(JBFundingCycle) (JBXBuybackDelegate.sol#1808-1810) is never used and should be removed



    
1808   function mintingAllowed(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1809     return ((_fundingCycle.metadata >> 76) & 1) == 1;
1810   }



```

```
Context._msgData() (JBXBuybackDelegate.sol#1989-1991) is never used and should be removed



    
1989     function _msgData() internal view virtual returns (bytes calldata) {
1990         return msg.data;
1991     }



```

```
JBFundingCycleMetadataResolver.expandMetadata(JBFundingCycle) (JBXBuybackDelegate.sol#1933-1959) is never used and should be removed



    
1933   function expandMetadata(JBFundingCycle memory _fundingCycle)
1934     internal
1935     pure
1936     returns (JBFundingCycleMetadata memory)
1937   {
1938     return
1939       JBFundingCycleMetadata(
1940         global(_fundingCycle),
1941         reservedRate(_fundingCycle),
1942         redemptionRate(_fundingCycle),
1943         ballotRedemptionRate(_fundingCycle),
1944         payPaused(_fundingCycle),
1945         distributionsPaused(_fundingCycle),
1946         redeemPaused(_fundingCycle),
1947         burnPaused(_fundingCycle),
1948         mintingAllowed(_fundingCycle),
1949         terminalMigrationAllowed(_fundingCycle),
1950         controllerMigrationAllowed(_fundingCycle),
1951         shouldHoldFees(_fundingCycle),
1952         preferClaimedTokenOverride(_fundingCycle),
1953         useTotalOverflowForRedemptions(_fundingCycle),
1954         useDataSourceForPay(_fundingCycle),
1955         useDataSourceForRedeem(_fundingCycle),
1956         dataSource(_fundingCycle),
1957         metadata(_fundingCycle)
1958       );
1959   }



```

```
JBFundingCycleMetadataResolver.preferClaimedTokenOverride(JBFundingCycle) (JBXBuybackDelegate.sol#1832-1838) is never used and should be removed



    
1832   function preferClaimedTokenOverride(JBFundingCycle memory _fundingCycle)
1833     internal
1834     pure
1835     returns (bool)
1836   {
1837     return ((_fundingCycle.metadata >> 80) & 1) == 1;
1838   }



```

```
JBFundingCycleMetadataResolver.ballotRedemptionRate(JBFundingCycle) (JBXBuybackDelegate.sol#1783-1790) is never used and should be removed



    
1783   function ballotRedemptionRate(JBFundingCycle memory _fundingCycle)
1784     internal
1785     pure
1786     returns (uint256)
1787   {
1788     // Redemption rate is a number 0-10000. It's inverse was stored so the most common case of 100% results in no storage needs.
1789     return JBConstants.MAX_REDEMPTION_RATE - uint256(uint16(_fundingCycle.metadata >> 56));
1790   }



```

```
JBFundingCycleMetadataResolver.useDataSourceForPay(JBFundingCycle) (JBXBuybackDelegate.sol#1848-1850) is never used and should be removed



    
1848   function useDataSourceForPay(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1849     return (_fundingCycle.metadata >> 82) & 1 == 1;
1850   }



```

```
PRBMath.mostSignificantBit(uint256) (JBXBuybackDelegate.sol#2493-2526) is never used and should be removed



    
2493     function mostSignificantBit(uint256 x) internal pure returns (uint256 msb) {
2494         if (x >= 2**128) {
2495             x >>= 128;
2496             msb += 128;
2497         }
2498         if (x >= 2**64) {
2499             x >>= 64;
2500             msb += 64;
2501         }
2502         if (x >= 2**32) {
2503             x >>= 32;
2504             msb += 32;
2505         }
2506         if (x >= 2**16) {
2507             x >>= 16;
2508             msb += 16;
2509         }
2510         if (x >= 2**8) {
2511             x >>= 8;
2512             msb += 8;
2513         }
2514         if (x >= 2**4) {
2515             x >>= 4;
2516             msb += 4;
2517         }
2518         if (x >= 2**2) {
2519             x >>= 2;
2520             msb += 2;
2521         }
2522         if (x >= 2**1) {
2523             // No need to shift x any more.
2524             msb += 1;
2525         }
2526     }



```

```
JBFundingCycleMetadataResolver.redeemPaused(JBFundingCycle) (JBXBuybackDelegate.sol#1800-1802) is never used and should be removed



    
1800   function redeemPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {
1801     return ((_fundingCycle.metadata >> 74) & 1) == 1;
1802   }



```

```
JBFundingCycleMetadataResolver.global(JBFundingCycle) (JBXBuybackDelegate.sol#1766-1772) is never used and should be removed



    
1766   function global(JBFundingCycle memory _fundingCycle)
1767     internal
1768     pure
1769     returns (JBGlobalFundingCycleMetadata memory)
1770   {
1771     return JBGlobalFundingCycleMetadataResolver.expandMetadata(uint8(_fundingCycle.metadata >> 8));
1772   }



```

```
JBFundingCycleMetadataResolver.terminalMigrationAllowed(JBFundingCycle) (JBXBuybackDelegate.sol#1812-1818) is never used and should be removed



    
1812   function terminalMigrationAllowed(JBFundingCycle memory _fundingCycle)
1813     internal
1814     pure
1815     returns (bool)
1816   {
1817     return ((_fundingCycle.metadata >> 77) & 1) == 1;
1818   }



```

```
JBFundingCycleMetadataResolver.dataSource(JBFundingCycle) (JBXBuybackDelegate.sol#1860-1862) is never used and should be removed



    
1860   function dataSource(JBFundingCycle memory _fundingCycle) internal pure returns (address) {
1861     return address(uint160(_fundingCycle.metadata >> 84));
1862   }



```

```
JBFundingCycleMetadataResolver.redemptionRate(JBFundingCycle) (JBXBuybackDelegate.sol#1778-1781) is never used and should be removed



    
1778   function redemptionRate(JBFundingCycle memory _fundingCycle) internal pure returns (uint256) {
1779     // Redemption rate is a number 0-10000. It's inverse was stored so the most common case of 100% results in no storage needs.
1780     return JBConstants.MAX_REDEMPTION_RATE - uint256(uint16(_fundingCycle.metadata >> 40));
1781   }



```

## solc-version
### Severity: Informational

### JBXBuybackDelegate.sol


```
solc-0.8.16 is not recommended for deployment



```

```
Pragma version^0.8.16 (JBXBuybackDelegate.sol#2) allows old versions



    
2 pragma solidity ^0.8.16;



```

## naming-convention
### Severity: Informational

### JBXBuybackDelegate.sol


```
Parameter JBFundingCycleMetadataResolver.global(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1766) is not in mixedCase



    
1766   function global(JBFundingCycle memory _fundingCycle)



```

```
Parameter JBFundingCycleMetadataResolver.shouldHoldFees(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1828) is not in mixedCase



    
1828   function shouldHoldFees(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Parameter JBFundingCycleMetadataResolver.ballotRedemptionRate(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1783) is not in mixedCase



    
1783   function ballotRedemptionRate(JBFundingCycle memory _fundingCycle)



```

```
Parameter JBFundingCycleMetadataResolver.useDataSourceForPay(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1848) is not in mixedCase



    
1848   function useDataSourceForPay(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Parameter JBXBuybackDelegate.payParams(JBPayParamsData)._data (JBXBuybackDelegate.sol#3617) is not in mixedCase



    
3617     function payParams(JBPayParamsData calldata _data)



```

```
Contract IJBPayoutTerminal3_1 (JBXBuybackDelegate.sol#1371-1380) is not in CapWords



    
1371 interface IJBPayoutTerminal3_1 {
1372   function distributePayoutsOf(
1373     uint256 _projectId,
1374     uint256 _amount,
1375     uint256 _currency,
1376     address _token,
1377     uint256 _minReturnedTokens,
1378     bytes calldata _metadata
1379   ) external returns (uint256 netLeftoverDistributionAmount);
1380 }



```

```
Parameter JBGlobalFundingCycleMetadataResolver.transfersPaused(uint8)._data (JBXBuybackDelegate.sol#1718) is not in mixedCase



    
1718   function transfersPaused(uint8 _data) internal pure returns (bool) {



```

```
Parameter JBFundingCycleMetadataResolver.expandMetadata(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1933) is not in mixedCase



    
1933   function expandMetadata(JBFundingCycle memory _fundingCycle)



```

```
Event JBXBuybackDelegate.JBXBuybackDelegate_Swap(uint256,uint256,uint256) (JBXBuybackDelegate.sol#3526) is not in CapWords



    
3526     event JBXBuybackDelegate_Swap(uint256 projectId, uint256 amountEth, uint256 amountOut);



```

```
Parameter JBFundingCycleMetadataResolver.terminalMigrationAllowed(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1812) is not in mixedCase



    
1812   function terminalMigrationAllowed(JBFundingCycle memory _fundingCycle)



```

```
Parameter JBFundingCycleMetadataResolver.distributionsPaused(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1796) is not in mixedCase



    
1796   function distributionsPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Parameter JBFundingCycleMetadataResolver.packFundingCycleMetadata(JBFundingCycleMetadata)._metadata (JBXBuybackDelegate.sol#1876) is not in mixedCase



    
1876   function packFundingCycleMetadata(JBFundingCycleMetadata memory _metadata)



```

```
Parameter JBXBuybackDelegate.didPay(JBDidPayData)._data (JBXBuybackDelegate.sol#3656) is not in mixedCase



    
3656     function didPay(JBDidPayData calldata _data) external payable override {



```

```
Parameter JBFundingCycleMetadataResolver.useTotalOverflowForRedemptions(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1840) is not in mixedCase



    
1840   function useTotalOverflowForRedemptions(JBFundingCycle memory _fundingCycle)



```

```
Parameter JBFundingCycleMetadataResolver.burnPaused(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1804) is not in mixedCase



    
1804   function burnPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Parameter JBFundingCycleMetadataResolver.redeemPaused(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1800) is not in mixedCase



    
1800   function redeemPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Parameter JBXBuybackDelegate.supportsInterface(bytes4)._interfaceId (JBXBuybackDelegate.sol#3830) is not in mixedCase



    
3830     function supportsInterface(bytes4 _interfaceId) external pure override returns (bool) {



```

```
Parameter JBFundingCycleMetadataResolver.mintingAllowed(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1808) is not in mixedCase



    
1808   function mintingAllowed(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Contract IJBController3_1 (JBXBuybackDelegate.sol#906-1055) is not in CapWords



    
906 interface IJBController3_1 is IJBController3_0_1, IERC165 {
907   event LaunchProject(uint256 configuration, uint256 projectId, string memo, address caller);
908 
909   event LaunchFundingCycles(uint256 configuration, uint256 projectId, string memo, address caller);
910 
911   event ReconfigureFundingCycles(
912     uint256 configuration,
913     uint256 projectId,
914     string memo,
915     address caller
916   );
917 
918   event DistributeReservedTokens(
919     uint256 indexed fundingCycleConfiguration,
920     uint256 indexed fundingCycleNumber,
921     uint256 indexed projectId,
922     address beneficiary,
923     uint256 tokenCount,
924     uint256 beneficiaryTokenCount,
925     string memo,
926     address caller
927   );
928 
929   event DistributeToReservedTokenSplit(
930     uint256 indexed projectId,
931     uint256 indexed domain,
932     uint256 indexed group,
933     JBSplit split,
934     uint256 tokenCount,
935     address caller
936   );
937 
938   event MintTokens(
939     address indexed beneficiary,
940     uint256 indexed projectId,
941     uint256 tokenCount,
942     uint256 beneficiaryTokenCount,
943     string memo,
944     uint256 reservedRate,
945     address caller
946   );
947 
948   event BurnTokens(
949     address indexed holder,
950     uint256 indexed projectId,
951     uint256 tokenCount,
952     string memo,
953     address caller
954   );
955 
956   event Migrate(uint256 indexed projectId, IJBMigratable to, address caller);
957 
958   event PrepMigration(uint256 indexed projectId, address from, address caller);
959 
960   function projects() external view returns (IJBProjects);
961 
962   function fundingCycleStore() external view returns (IJBFundingCycleStore);
963 
964   function tokenStore() external view returns (IJBTokenStore);
965 
966   function splitsStore() external view returns (IJBSplitsStore);
967 
968   function fundAccessConstraintsStore() external view returns (IJBFundAccessConstraintsStore);
969 
970   function directory() external view returns (IJBDirectory);
971 
972   function reservedTokenBalanceOf(uint256 _projectId) external view returns (uint256);
973 
974   function totalOutstandingTokensOf(uint256 _projectId) external view returns (uint256);
975 
976   function getFundingCycleOf(uint256 _projectId, uint256 _configuration)
977     external
978     view
979     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);
980 
981   function latestConfiguredFundingCycleOf(uint256 _projectId)
982     external
983     view
984     returns (
985       JBFundingCycle memory,
986       JBFundingCycleMetadata memory metadata,
987       JBBallotState
988     );
989 
990   function currentFundingCycleOf(uint256 _projectId)
991     external
992     view
993     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);
994 
995   function queuedFundingCycleOf(uint256 _projectId)
996     external
997     view
998     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);
999 
1000   function launchProjectFor(
1001     address _owner,
1002     JBProjectMetadata calldata _projectMetadata,
1003     JBFundingCycleData calldata _data,
1004     JBFundingCycleMetadata calldata _metadata,
1005     uint256 _mustStartAtOrAfter,
1006     JBGroupedSplits[] memory _groupedSplits,
1007     JBFundAccessConstraints[] memory _fundAccessConstraints,
1008     IJBPaymentTerminal[] memory _terminals,
1009     string calldata _memo
1010   ) external returns (uint256 projectId);
1011 
1012   function launchFundingCyclesFor(
1013     uint256 _projectId,
1014     JBFundingCycleData calldata _data,
1015     JBFundingCycleMetadata calldata _metadata,
1016     uint256 _mustStartAtOrAfter,
1017     JBGroupedSplits[] memory _groupedSplits,
1018     JBFundAccessConstraints[] memory _fundAccessConstraints,
1019     IJBPaymentTerminal[] memory _terminals,
1020     string calldata _memo
1021   ) external returns (uint256 configuration);
1022 
1023   function reconfigureFundingCyclesOf(
1024     uint256 _projectId,
1025     JBFundingCycleData calldata _data,
1026     JBFundingCycleMetadata calldata _metadata,
1027     uint256 _mustStartAtOrAfter,
1028     JBGroupedSplits[] memory _groupedSplits,
1029     JBFundAccessConstraints[] memory _fundAccessConstraints,
1030     string calldata _memo
1031   ) external returns (uint256);
1032 
1033   function mintTokensOf(
1034     uint256 _projectId,
1035     uint256 _tokenCount,
1036     address _beneficiary,
1037     string calldata _memo,
1038     bool _preferClaimedTokens,
1039     bool _useReservedRate
1040   ) external returns (uint256 beneficiaryTokenCount);
1041 
1042   function burnTokensOf(
1043     address _holder,
1044     uint256 _projectId,
1045     uint256 _tokenCount,
1046     string calldata _memo,
1047     bool _preferClaimedTokens
1048   ) external;
1049 
1050   function distributeReservedTokensOf(uint256 _projectId, string memory _memo)
1051     external
1052     returns (uint256);
1053 
1054   function migrate(uint256 _projectId, IJBMigratable _to) external;
1055 }



```

```
Contract IJBController3_0_1 (JBXBuybackDelegate.sol#872-875) is not in CapWords



    
872 interface IJBController3_0_1 {
873   function reservedTokenBalanceOf(uint256 _projectId) external view returns (uint256);
874   function totalOutstandingTokensOf(uint256 _projectId) external view returns (uint256);
875 }



```

```
Parameter JBFundingCycleMetadataResolver.payPaused(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1792) is not in mixedCase



    
1792   function payPaused(JBFundingCycle memory _fundingCycle) internal pure returns (bool) {



```

```
Parameter JBFundingCycleMetadataResolver.dataSource(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1860) is not in mixedCase



    
1860   function dataSource(JBFundingCycle memory _fundingCycle) internal pure returns (address) {



```

```
Parameter JBFundingCycleMetadataResolver.reservedRate(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1774) is not in mixedCase



    
1774   function reservedRate(JBFundingCycle memory _fundingCycle) internal pure returns (uint256) {



```

```
Parameter JBFundingCycleMetadataResolver.controllerMigrationAllowed(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1820) is not in mixedCase



    
1820   function controllerMigrationAllowed(JBFundingCycle memory _fundingCycle)



```

```
Event JBXBuybackDelegate.JBXBuybackDelegate_Mint(uint256) (JBXBuybackDelegate.sol#3527) is not in CapWords



    
3527     event JBXBuybackDelegate_Mint(uint256 projectId);



```

```
Contract IJBAllowanceTerminal3_1 (JBXBuybackDelegate.sol#1343-1354) is not in CapWords



    
1343 interface IJBAllowanceTerminal3_1 {
1344   function useAllowanceOf(
1345     uint256 _projectId,
1346     uint256 _amount,
1347     uint256 _currency,
1348     address _token,
1349     uint256 _minReturnedTokens,
1350     address payable _beneficiary,
1351     string calldata _memo,
1352     bytes calldata _metadata
1353   ) external returns (uint256 netDistributedAmount);
1354 }



```

```
Parameter JBFundingCycleMetadataResolver.metadata(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1864) is not in mixedCase



    
1864   function metadata(JBFundingCycle memory _fundingCycle) internal pure returns (uint256) {



```

```
Parameter JBFundingCycleMetadataResolver.redemptionRate(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1778) is not in mixedCase



    
1778   function redemptionRate(JBFundingCycle memory _fundingCycle) internal pure returns (uint256) {



```

```
Parameter JBFundingCycleMetadataResolver.useDataSourceForRedeem(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1852) is not in mixedCase



    
1852   function useDataSourceForRedeem(JBFundingCycle memory _fundingCycle)



```

```
Parameter JBFundingCycleMetadataResolver.preferClaimedTokenOverride(JBFundingCycle)._fundingCycle (JBXBuybackDelegate.sol#1832) is not in mixedCase



    
1832   function preferClaimedTokenOverride(JBFundingCycle memory _fundingCycle)



```

```
Parameter JBGlobalFundingCycleMetadataResolver.setTerminalsAllowed(uint8)._data (JBXBuybackDelegate.sol#1710) is not in mixedCase



    
1710   function setTerminalsAllowed(uint8 _data) internal pure returns (bool) {



```

```
Parameter JBGlobalFundingCycleMetadataResolver.expandMetadata(uint8)._packedMetadata (JBXBuybackDelegate.sol#1751) is not in mixedCase



    
1751   function expandMetadata(uint8 _packedMetadata)



```

```
Parameter JBGlobalFundingCycleMetadataResolver.setControllerAllowed(uint8)._data (JBXBuybackDelegate.sol#1714) is not in mixedCase



    
1714   function setControllerAllowed(uint8 _data) internal pure returns (bool) {



```

```
Contract IJBPayoutRedemptionPaymentTerminal3_1 (JBXBuybackDelegate.sol#1523-1694) is not in CapWords



    
1523 interface IJBPayoutRedemptionPaymentTerminal3_1 is
1524   IJBPaymentTerminal,
1525   IJBPayoutTerminal3_1,
1526   IJBAllowanceTerminal3_1,
1527   IJBRedemptionTerminal,
1528   IJBFeeHoldingTerminal
1529 {
1530   event AddToBalance(
1531     uint256 indexed projectId,
1532     uint256 amount,
1533     uint256 refundedFees,
1534     string memo,
1535     bytes metadata,
1536     address caller
1537   );
1538 
1539   event Migrate(
1540     uint256 indexed projectId,
1541     IJBPaymentTerminal indexed to,
1542     uint256 amount,
1543     address caller
1544   );
1545 
1546   event DistributePayouts(
1547     uint256 indexed fundingCycleConfiguration,
1548     uint256 indexed fundingCycleNumber,
1549     uint256 indexed projectId,
1550     address beneficiary,
1551     uint256 amount,
1552     uint256 distributedAmount,
1553     uint256 fee,
1554     uint256 beneficiaryDistributionAmount,
1555     bytes metadata,
1556     address caller
1557   );
1558 
1559   event UseAllowance(
1560     uint256 indexed fundingCycleConfiguration,
1561     uint256 indexed fundingCycleNumber,
1562     uint256 indexed projectId,
1563     address beneficiary,
1564     uint256 amount,
1565     uint256 distributedAmount,
1566     uint256 netDistributedamount,
1567     string memo,
1568     bytes metadata,
1569     address caller
1570   );
1571 
1572   event HoldFee(
1573     uint256 indexed projectId,
1574     uint256 indexed amount,
1575     uint256 indexed fee,
1576     uint256 feeDiscount,
1577     address beneficiary,
1578     address caller
1579   );
1580 
1581   event ProcessFee(
1582     uint256 indexed projectId,
1583     uint256 indexed amount,
1584     bool indexed wasHeld,
1585     address beneficiary,
1586     address caller
1587   );
1588 
1589   event RefundHeldFees(
1590     uint256 indexed projectId,
1591     uint256 indexed amount,
1592     uint256 indexed refundedFees,
1593     uint256 leftoverAmount,
1594     address caller
1595   );
1596 
1597   event Pay(
1598     uint256 indexed fundingCycleConfiguration,
1599     uint256 indexed fundingCycleNumber,
1600     uint256 indexed projectId,
1601     address payer,
1602     address beneficiary,
1603     uint256 amount,
1604     uint256 beneficiaryTokenCount,
1605     string memo,
1606     bytes metadata,
1607     address caller
1608   );
1609 
1610   event DelegateDidPay(
1611     IJBPayDelegate indexed delegate,
1612     JBDidPayData data,
1613     uint256 delegatedAmount,
1614     address caller
1615   );
1616 
1617   event RedeemTokens(
1618     uint256 indexed fundingCycleConfiguration,
1619     uint256 indexed fundingCycleNumber,
1620     uint256 indexed projectId,
1621     address holder,
1622     address beneficiary,
1623     uint256 tokenCount,
1624     uint256 reclaimedAmount,
1625     string memo,
1626     bytes metadata,
1627     address caller
1628   );
1629 
1630   event DelegateDidRedeem(
1631     IJBRedemptionDelegate indexed delegate,
1632     JBDidRedeemData data,
1633     uint256 delegatedAmount,
1634     address caller
1635   );
1636 
1637   event DistributeToPayoutSplit(
1638     uint256 indexed projectId,
1639     uint256 indexed domain,
1640     uint256 indexed group,
1641     JBSplit split,
1642     uint256 amount,
1643     uint256 netAmount,
1644     address caller
1645   );
1646 
1647   event SetFee(uint256 fee, address caller);
1648 
1649   event SetFeeGauge(IJBFeeGauge indexed feeGauge, address caller);
1650 
1651   event SetFeelessAddress(address indexed addrs, bool indexed flag, address caller);
1652 
1653   event PayoutReverted(uint256 indexed projectId, JBSplit split, uint256 amount, bytes reason, address caller);
1654 
1655   event FeeReverted(
1656     uint256 indexed projectId,
1657     uint256 indexed feeProjectId,
1658     uint256 amount,
1659     bytes reason,
1660     address caller
1661   );
1662 
1663   function projects() external view returns (IJBProjects);
1664 
1665   function splitsStore() external view returns (IJBSplitsStore);
1666 
1667   function directory() external view returns (IJBDirectory);
1668 
1669   function prices() external view returns (IJBPrices);
1670 
1671   function store() external view returns (IJBSingleTokenPaymentTerminalStore);
1672 
1673   function baseWeightCurrency() external view returns (uint256);
1674 
1675   function payoutSplitsGroup() external view returns (uint256);
1676 
1677   function heldFeesOf(uint256 _projectId) external view returns (JBFee[] memory);
1678 
1679   function fee() external view returns (uint256);
1680 
1681   function feeGauge() external view returns (IJBFeeGauge);
1682 
1683   function isFeelessAddress(address _contract) external view returns (bool);
1684 
1685   function migrate(uint256 _projectId, IJBPaymentTerminal _to) external returns (uint256 balance);
1686 
1687   function processFees(uint256 _projectId) external;
1688 
1689   function setFee(uint256 _fee) external;
1690 
1691   function setFeeGauge(IJBFeeGauge _feeGauge) external;
1692 
1693   function setFeelessAddress(address _contract, bool _flag) external;
1694 }



```

```
Parameter JBGlobalFundingCycleMetadataResolver.packFundingCycleGlobalMetadata(JBGlobalFundingCycleMetadata)._metadata (JBXBuybackDelegate.sol#1730) is not in mixedCase



    
1730   function packFundingCycleGlobalMetadata(JBGlobalFundingCycleMetadata memory _metadata)



```

## similar-names
### Severity: Informational

### JBXBuybackDelegate.sol


```
Variable IUniswapV3SwapCallback.uniswapV3SwapCallback(int256,int256,bytes).amount0Delta (JBXBuybackDelegate.sol#3272) is too similar to IUniswapV3SwapCallback.uniswapV3SwapCallback(int256,int256,bytes).amount1Delta (JBXBuybackDelegate.sol#3273)



    
3272         int256 amount0Delta,



```

```
Variable IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount0Requested (JBXBuybackDelegate.sol#3028) is too similar to IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount1Requested (JBXBuybackDelegate.sol#3029)



    
3028         uint128 amount0Requested,



```

```
Variable IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount0Requested (JBXBuybackDelegate.sol#3102) is too similar to IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount1Requested (JBXBuybackDelegate.sol#3103)



    
3102         uint128 amount0Requested,



```

```
Variable IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount0Requested (JBXBuybackDelegate.sol#3028) is too similar to IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount1Requested (JBXBuybackDelegate.sol#3103)



    
3028         uint128 amount0Requested,



```

```
Variable IUniswapV3PoolState.positions(bytes32).tokensOwed0 (JBXBuybackDelegate.sol#2924) is too similar to IUniswapV3PoolState.positions(bytes32).tokensOwed1 (JBXBuybackDelegate.sol#2925)



    
2924             uint128 tokensOwed0,



```

```
Variable IUniswapV3PoolState.positions(bytes32).feeGrowthInside0LastX128 (JBXBuybackDelegate.sol#2922) is too similar to IUniswapV3PoolState.positions(bytes32).feeGrowthInside1LastX128 (JBXBuybackDelegate.sol#2923)



    
2922             uint256 feeGrowthInside0LastX128,



```

```
Variable JBXBuybackDelegate.uniswapV3SwapCallback(int256,int256,bytes).amount0Delta (JBXBuybackDelegate.sol#3690) is too similar to JBXBuybackDelegate.uniswapV3SwapCallback(int256,int256,bytes).amount1Delta (JBXBuybackDelegate.sol#3690)



    
3690     function uniswapV3SwapCallback(int256 amount0Delta, int256 amount1Delta, bytes calldata data) external override {



```

```
Variable IUniswapV3PoolState.ticks(int24).feeGrowthOutside0X128 (JBXBuybackDelegate.sol#2899) is too similar to IUniswapV3PoolState.ticks(int24).feeGrowthOutside1X128 (JBXBuybackDelegate.sol#2900)



    
2899             uint256 feeGrowthOutside0X128,



```

```
Variable IUniswapV3PoolOwnerActions.setFeeProtocol(uint8,uint8).feeProtocol0 (JBXBuybackDelegate.sol#3092) is too similar to IUniswapV3PoolOwnerActions.setFeeProtocol(uint8,uint8).feeProtocol1 (JBXBuybackDelegate.sol#3092)



    
3092     function setFeeProtocol(uint8 feeProtocol0, uint8 feeProtocol1) external;



```

```
Variable JBXBuybackDelegate.uniswapV3SwapCallback(int256,int256,bytes).amount0Delta (JBXBuybackDelegate.sol#3690) is too similar to IUniswapV3SwapCallback.uniswapV3SwapCallback(int256,int256,bytes).amount1Delta (JBXBuybackDelegate.sol#3273)



    
3690     function uniswapV3SwapCallback(int256 amount0Delta, int256 amount1Delta, bytes calldata data) external override {



```

```
Variable IUniswapV3PoolOwnerActions.collectProtocol(address,uint128,uint128).amount0Requested (JBXBuybackDelegate.sol#3102) is too similar to IUniswapV3PoolActions.collect(address,int24,int24,uint128,uint128).amount1Requested (JBXBuybackDelegate.sol#3029)



    
3102         uint128 amount0Requested,



```

```
Variable IUniswapV3SwapCallback.uniswapV3SwapCallback(int256,int256,bytes).amount0Delta (JBXBuybackDelegate.sol#3272) is too similar to JBXBuybackDelegate.uniswapV3SwapCallback(int256,int256,bytes).amount1Delta (JBXBuybackDelegate.sol#3690)



    
3272         int256 amount0Delta,



```

## too-many-digits
### Severity: Informational

### JBXBuybackDelegate.sol


```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000003) >> 64 (JBXBuybackDelegate.sol#2467)



    
2467                 result = (result * 0x10000000000000003) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x400000000000 > 0 (JBXBuybackDelegate.sol#2334)



    
2334             if (x & 0x400000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000000058B9) >> 64 (JBXBuybackDelegate.sol#2428)



    
2428                 result = (result * 0x100000000000058B9) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000002C5C86) >> 64 (JBXBuybackDelegate.sol#2407)



    
2407                 result = (result * 0x100000000002C5C86) >> 64;



```

```
PRBMath.sqrt(uint256) (JBXBuybackDelegate.sol#2748-2796) uses literals with too many digits:
	- xAux >= 0x10000000000000000 (JBXBuybackDelegate.sol#2760)



    
2760         if (xAux >= 0x10000000000000000) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000000002C6) >> 64 (JBXBuybackDelegate.sol#2443)



    
2443                 result = (result * 0x100000000000002C6) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000002C5C8) >> 64 (JBXBuybackDelegate.sol#2419)



    
2419                 result = (result * 0x1000000000002C5C8) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x100000000 > 0 (JBXBuybackDelegate.sol#2376)



    
2376             if (x & 0x100000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000162E430E5A2) >> 64 (JBXBuybackDelegate.sol#2350)



    
2350                 result = (result * 0x100000162E430E5A2) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x10000000000000 > 0 (JBXBuybackDelegate.sol#2316)



    
2316             if (x & 0x10000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x20000000 > 0 (JBXBuybackDelegate.sol#2385)



    
2385             if (x & 0x20000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000058B90C0B49) >> 64 (JBXBuybackDelegate.sol#2356)



    
2356                 result = (result * 0x100000058B90C0B49) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000000000B1) >> 64 (JBXBuybackDelegate.sol#2449)



    
2449                 result = (result * 0x100000000000000B1) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000058B90C) >> 64 (JBXBuybackDelegate.sol#2404)



    
2404                 result = (result * 0x1000000000058B90C) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000000B1721) >> 64 (JBXBuybackDelegate.sol#2413)



    
2413                 result = (result * 0x100000000000B1721) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x400000000000000 > 0 (JBXBuybackDelegate.sol#2298)



    
2298             if (x & 0x400000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000002C5C8601CC) >> 64 (JBXBuybackDelegate.sol#2359)



    
2359                 result = (result * 0x10000002C5C8601CC) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000B17217FBB) >> 64 (JBXBuybackDelegate.sol#2365)



    
2365                 result = (result * 0x10000000B17217FBB) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000B17217F) >> 64 (JBXBuybackDelegate.sol#2389)



    
2389                 result = (result * 0x1000000000B17217F) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000001) >> 64 (JBXBuybackDelegate.sol#2470)



    
2470                 result = (result * 0x10000000000000001) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000001) >> 64 (JBXBuybackDelegate.sol#2473)



    
2473                 result = (result * 0x10000000000000001) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x2000000000 > 0 (JBXBuybackDelegate.sol#2361)



    
2361             if (x & 0x2000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000162E43) >> 64 (JBXBuybackDelegate.sol#2410)



    
2410                 result = (result * 0x10000000000162E43) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x400000000 > 0 (JBXBuybackDelegate.sol#2370)



    
2370             if (x & 0x400000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x4000000000000 > 0 (JBXBuybackDelegate.sol#2322)



    
2322             if (x & 0x4000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000058B90CF1E6E) >> 64 (JBXBuybackDelegate.sol#2344)



    
2344                 result = (result * 0x10000058B90CF1E6E) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x100000000000 > 0 (JBXBuybackDelegate.sol#2340)



    
2340             if (x & 0x100000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000B17218) >> 64 (JBXBuybackDelegate.sol#2401)



    
2401                 result = (result * 0x10000000000B17218) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000002C5C85FE) >> 64 (JBXBuybackDelegate.sol#2383)



    
2383                 result = (result * 0x1000000002C5C85FE) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x4000000 > 0 (JBXBuybackDelegate.sol#2394)



    
2394             if (x & 0x4000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x8000000000000 > 0 (JBXBuybackDelegate.sol#2319)



    
2319             if (x & 0x8000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000059) >> 64 (JBXBuybackDelegate.sol#2452)



    
2452                 result = (result * 0x10000000000000059) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000000002C) >> 64 (JBXBuybackDelegate.sol#2455)



    
2455                 result = (result * 0x1000000000000002C) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x80000000000000 > 0 (JBXBuybackDelegate.sol#2307)



    
2307             if (x & 0x80000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000000162E) >> 64 (JBXBuybackDelegate.sol#2434)



    
2434                 result = (result * 0x1000000000000162E) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x800000000000000 > 0 (JBXBuybackDelegate.sol#2295)



    
2295             if (x & 0x800000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000B17) >> 64 (JBXBuybackDelegate.sol#2437)



    
2437                 result = (result * 0x10000000000000B17) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000002C5C860) >> 64 (JBXBuybackDelegate.sol#2395)



    
2395                 result = (result * 0x10000000002C5C860) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000B172183551) >> 64 (JBXBuybackDelegate.sol#2353)



    
2353                 result = (result * 0x1000000B172183551) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000058B90BFC) >> 64 (JBXBuybackDelegate.sol#2380)



    
2380                 result = (result * 0x10000000058B90BFC) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x800000000000 > 0 (JBXBuybackDelegate.sol#2331)



    
2331             if (x & 0x800000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x200000000000 > 0 (JBXBuybackDelegate.sol#2337)



    
2337             if (x & 0x200000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000058B90BFCE) >> 64 (JBXBuybackDelegate.sol#2368)



    
2368                 result = (result * 0x1000000058B90BFCE) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x10000000 > 0 (JBXBuybackDelegate.sol#2388)



    
2388             if (x & 0x10000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x800000 > 0 (JBXBuybackDelegate.sol#2403)



    
2403             if (x & 0x800000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x100000000000000 > 0 (JBXBuybackDelegate.sol#2304)



    
2304             if (x & 0x100000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x20000000000000 > 0 (JBXBuybackDelegate.sol#2313)



    
2313             if (x & 0x20000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x800000000 > 0 (JBXBuybackDelegate.sol#2367)



    
2367             if (x & 0x800000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x2000000 > 0 (JBXBuybackDelegate.sol#2397)



    
2397             if (x & 0x2000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x40000000000 > 0 (JBXBuybackDelegate.sol#2346)



    
2346             if (x & 0x40000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000058B91) >> 64 (JBXBuybackDelegate.sol#2416)



    
2416                 result = (result * 0x10000000000058B91) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000002C5C85FE3) >> 64 (JBXBuybackDelegate.sol#2371)



    
2371                 result = (result * 0x100000002C5C85FE3) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x8000000000000000 > 0 (JBXBuybackDelegate.sol#2283)



    
2283             if (x & 0x8000000000000000 > 0) {



```

```
PRBMath.sqrt(uint256) (JBXBuybackDelegate.sol#2748-2796) uses literals with too many digits:
	- xAux >= 0x100000000000000000000000000000000 (JBXBuybackDelegate.sol#2756)



    
2756         if (xAux >= 0x100000000000000000000000000000000) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x1000000000 > 0 (JBXBuybackDelegate.sol#2364)



    
2364             if (x & 0x1000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000162E42FFF0) >> 64 (JBXBuybackDelegate.sol#2362)



    
2362                 result = (result * 0x1000000162E42FFF0) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x200000 > 0 (JBXBuybackDelegate.sol#2409)



    
2409             if (x & 0x200000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x100000 > 0 (JBXBuybackDelegate.sol#2412)



    
2412             if (x & 0x100000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x4000000000000000 > 0 (JBXBuybackDelegate.sol#2286)



    
2286             if (x & 0x4000000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x8000000000 > 0 (JBXBuybackDelegate.sol#2355)



    
2355             if (x & 0x8000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000016) >> 64 (JBXBuybackDelegate.sol#2458)



    
2458                 result = (result * 0x10000000000000016) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000163) >> 64 (JBXBuybackDelegate.sol#2446)



    
2446                 result = (result * 0x10000000000000163) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x1000000000000 > 0 (JBXBuybackDelegate.sol#2328)



    
2328             if (x & 0x1000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000162E430) >> 64 (JBXBuybackDelegate.sol#2398)



    
2398                 result = (result * 0x1000000000162E430) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x200000000 > 0 (JBXBuybackDelegate.sol#2373)



    
2373             if (x & 0x200000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x1000000000000000 > 0 (JBXBuybackDelegate.sol#2292)



    
2292             if (x & 0x1000000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000000000B) >> 64 (JBXBuybackDelegate.sol#2461)



    
2461                 result = (result * 0x1000000000000000B) >> 64;



```

```
PRBMath.sqrt(uint256) (JBXBuybackDelegate.sol#2748-2796) uses literals with too many digits:
	- xAux >= 0x100000000 (JBXBuybackDelegate.sol#2764)



    
2764         if (xAux >= 0x100000000) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000162E42FF) >> 64 (JBXBuybackDelegate.sol#2386)



    
2386                 result = (result * 0x100000000162E42FF) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000000162E4) >> 64 (JBXBuybackDelegate.sol#2422)



    
2422                 result = (result * 0x100000000000162E4) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x80000000 > 0 (JBXBuybackDelegate.sol#2379)



    
2379             if (x & 0x80000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000B17217F8) >> 64 (JBXBuybackDelegate.sol#2377)



    
2377                 result = (result * 0x100000000B17217F8) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000000006) >> 64 (JBXBuybackDelegate.sol#2464)



    
2464                 result = (result * 0x10000000000000006) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x4000000000 > 0 (JBXBuybackDelegate.sol#2358)



    
2358             if (x & 0x4000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000B1721BCFC9A) >> 64 (JBXBuybackDelegate.sol#2341)



    
2341                 result = (result * 0x100000B1721BCFC9A) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000000002C5D) >> 64 (JBXBuybackDelegate.sol#2431)



    
2431                 result = (result * 0x10000000000002C5D) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x20000000000 > 0 (JBXBuybackDelegate.sol#2349)



    
2349             if (x & 0x20000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x2000000000000000 > 0 (JBXBuybackDelegate.sol#2289)



    
2289             if (x & 0x2000000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x200000000000000 > 0 (JBXBuybackDelegate.sol#2301)



    
2301             if (x & 0x200000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x80000000000 > 0 (JBXBuybackDelegate.sol#2343)



    
2343             if (x & 0x80000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x10000000000 > 0 (JBXBuybackDelegate.sol#2352)



    
2352             if (x & 0x10000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x8000000 > 0 (JBXBuybackDelegate.sol#2391)



    
2391             if (x & 0x8000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000000058C) >> 64 (JBXBuybackDelegate.sol#2440)



    
2440                 result = (result * 0x1000000000000058C) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x40000000 > 0 (JBXBuybackDelegate.sol#2382)



    
2382             if (x & 0x40000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x2000000000000 > 0 (JBXBuybackDelegate.sol#2325)



    
2325             if (x & 0x2000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x400000 > 0 (JBXBuybackDelegate.sol#2406)



    
2406             if (x & 0x400000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x1000000 > 0 (JBXBuybackDelegate.sol#2400)



    
2400             if (x & 0x1000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000000000000B172) >> 64 (JBXBuybackDelegate.sol#2425)



    
2425                 result = (result * 0x1000000000000B172) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- x & 0x40000000000000 > 0 (JBXBuybackDelegate.sol#2310)



    
2310             if (x & 0x40000000000000 > 0) {



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x10000000162E42FF1) >> 64 (JBXBuybackDelegate.sol#2374)



    
2374                 result = (result * 0x10000000162E42FF1) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x100000000058B90C0) >> 64 (JBXBuybackDelegate.sol#2392)



    
2392                 result = (result * 0x100000000058B90C0) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = (result * 0x1000002C5C863B73F) >> 64 (JBXBuybackDelegate.sol#2347)



    
2347                 result = (result * 0x1000002C5C863B73F) >> 64;



```

```
PRBMath.exp2(uint256) (JBXBuybackDelegate.sol#2276-2487) uses literals with too many digits:
	- result = 0x800000000000000000000000000000000000000000000000 (JBXBuybackDelegate.sol#2279)



    
2279             result = 0x800000000000000000000000000000000000000000000000;



```

```
TickMath.getSqrtRatioAtTick(int24) (JBXBuybackDelegate.sol#3300-3335) uses literals with too many digits:
	- ratio = 0x100000000000000000000000000000000 (JBXBuybackDelegate.sol#3305-3307)



    
3305             uint256 ratio = absTick & 0x1 != 0
3306                 ? 0xfffcb933bd6fad37aa2d162d1a594001
3307                 : 0x100000000000000000000000000000000;



```
