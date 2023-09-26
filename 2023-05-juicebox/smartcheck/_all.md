
# SMARTCHECK ANALYSIS

## SOLIDITY_ADDRESS_HARDCODED
The contract contains unknown address. This address might be used for some malicious activity. Please check hardcoded address and it's usage.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#1967
Severity: Low
1967   address public constant ETH = address(0x000000000000000000000000000000000000EEEe);



JBXBuybackDelegate.sol#2283
Severity: Low
2283             if (x & 0x8000000000000000 > 0) {



JBXBuybackDelegate.sol#2284
Severity: Low
2284                 result = (result * 0x16A09E667F3BCC909) >> 64;



JBXBuybackDelegate.sol#2286
Severity: Low
2286             if (x & 0x4000000000000000 > 0) {



JBXBuybackDelegate.sol#2287
Severity: Low
2287                 result = (result * 0x1306FE0A31B7152DF) >> 64;



JBXBuybackDelegate.sol#2289
Severity: Low
2289             if (x & 0x2000000000000000 > 0) {



JBXBuybackDelegate.sol#2290
Severity: Low
2290                 result = (result * 0x1172B83C7D517ADCE) >> 64;



JBXBuybackDelegate.sol#2292
Severity: Low
2292             if (x & 0x1000000000000000 > 0) {



JBXBuybackDelegate.sol#2293
Severity: Low
2293                 result = (result * 0x10B5586CF9890F62A) >> 64;



JBXBuybackDelegate.sol#2295
Severity: Low
2295             if (x & 0x800000000000000 > 0) {



JBXBuybackDelegate.sol#2296
Severity: Low
2296                 result = (result * 0x1059B0D31585743AE) >> 64;



JBXBuybackDelegate.sol#2298
Severity: Low
2298             if (x & 0x400000000000000 > 0) {



JBXBuybackDelegate.sol#2299
Severity: Low
2299                 result = (result * 0x102C9A3E778060EE7) >> 64;



JBXBuybackDelegate.sol#2301
Severity: Low
2301             if (x & 0x200000000000000 > 0) {



JBXBuybackDelegate.sol#2302
Severity: Low
2302                 result = (result * 0x10163DA9FB33356D8) >> 64;



JBXBuybackDelegate.sol#2304
Severity: Low
2304             if (x & 0x100000000000000 > 0) {



JBXBuybackDelegate.sol#2305
Severity: Low
2305                 result = (result * 0x100B1AFA5ABCBED61) >> 64;



JBXBuybackDelegate.sol#2307
Severity: Low
2307             if (x & 0x80000000000000 > 0) {



JBXBuybackDelegate.sol#2308
Severity: Low
2308                 result = (result * 0x10058C86DA1C09EA2) >> 64;



JBXBuybackDelegate.sol#2310
Severity: Low
2310             if (x & 0x40000000000000 > 0) {



JBXBuybackDelegate.sol#2311
Severity: Low
2311                 result = (result * 0x1002C605E2E8CEC50) >> 64;



JBXBuybackDelegate.sol#2313
Severity: Low
2313             if (x & 0x20000000000000 > 0) {



JBXBuybackDelegate.sol#2314
Severity: Low
2314                 result = (result * 0x100162F3904051FA1) >> 64;



JBXBuybackDelegate.sol#2316
Severity: Low
2316             if (x & 0x10000000000000 > 0) {



JBXBuybackDelegate.sol#2317
Severity: Low
2317                 result = (result * 0x1000B175EFFDC76BA) >> 64;



JBXBuybackDelegate.sol#2319
Severity: Low
2319             if (x & 0x8000000000000 > 0) {



JBXBuybackDelegate.sol#2320
Severity: Low
2320                 result = (result * 0x100058BA01FB9F96D) >> 64;



JBXBuybackDelegate.sol#2322
Severity: Low
2322             if (x & 0x4000000000000 > 0) {



JBXBuybackDelegate.sol#2323
Severity: Low
2323                 result = (result * 0x10002C5CC37DA9492) >> 64;



JBXBuybackDelegate.sol#2325
Severity: Low
2325             if (x & 0x2000000000000 > 0) {



JBXBuybackDelegate.sol#2326
Severity: Low
2326                 result = (result * 0x1000162E525EE0547) >> 64;



JBXBuybackDelegate.sol#2328
Severity: Low
2328             if (x & 0x1000000000000 > 0) {



JBXBuybackDelegate.sol#2329
Severity: Low
2329                 result = (result * 0x10000B17255775C04) >> 64;



JBXBuybackDelegate.sol#2331
Severity: Low
2331             if (x & 0x800000000000 > 0) {



JBXBuybackDelegate.sol#2332
Severity: Low
2332                 result = (result * 0x1000058B91B5BC9AE) >> 64;



JBXBuybackDelegate.sol#2334
Severity: Low
2334             if (x & 0x400000000000 > 0) {



JBXBuybackDelegate.sol#2335
Severity: Low
2335                 result = (result * 0x100002C5C89D5EC6D) >> 64;



JBXBuybackDelegate.sol#2337
Severity: Low
2337             if (x & 0x200000000000 > 0) {



JBXBuybackDelegate.sol#2338
Severity: Low
2338                 result = (result * 0x10000162E43F4F831) >> 64;



JBXBuybackDelegate.sol#2340
Severity: Low
2340             if (x & 0x100000000000 > 0) {



JBXBuybackDelegate.sol#2341
Severity: Low
2341                 result = (result * 0x100000B1721BCFC9A) >> 64;



JBXBuybackDelegate.sol#2343
Severity: Low
2343             if (x & 0x80000000000 > 0) {



JBXBuybackDelegate.sol#2344
Severity: Low
2344                 result = (result * 0x10000058B90CF1E6E) >> 64;



JBXBuybackDelegate.sol#2346
Severity: Low
2346             if (x & 0x40000000000 > 0) {



JBXBuybackDelegate.sol#2347
Severity: Low
2347                 result = (result * 0x1000002C5C863B73F) >> 64;



JBXBuybackDelegate.sol#2349
Severity: Low
2349             if (x & 0x20000000000 > 0) {



JBXBuybackDelegate.sol#2350
Severity: Low
2350                 result = (result * 0x100000162E430E5A2) >> 64;



JBXBuybackDelegate.sol#2352
Severity: Low
2352             if (x & 0x10000000000 > 0) {



JBXBuybackDelegate.sol#2353
Severity: Low
2353                 result = (result * 0x1000000B172183551) >> 64;



JBXBuybackDelegate.sol#2355
Severity: Low
2355             if (x & 0x8000000000 > 0) {



JBXBuybackDelegate.sol#2356
Severity: Low
2356                 result = (result * 0x100000058B90C0B49) >> 64;



JBXBuybackDelegate.sol#2358
Severity: Low
2358             if (x & 0x4000000000 > 0) {



JBXBuybackDelegate.sol#2359
Severity: Low
2359                 result = (result * 0x10000002C5C8601CC) >> 64;



JBXBuybackDelegate.sol#2361
Severity: Low
2361             if (x & 0x2000000000 > 0) {



JBXBuybackDelegate.sol#2362
Severity: Low
2362                 result = (result * 0x1000000162E42FFF0) >> 64;



JBXBuybackDelegate.sol#2364
Severity: Low
2364             if (x & 0x1000000000 > 0) {



JBXBuybackDelegate.sol#2365
Severity: Low
2365                 result = (result * 0x10000000B17217FBB) >> 64;



JBXBuybackDelegate.sol#2367
Severity: Low
2367             if (x & 0x800000000 > 0) {



JBXBuybackDelegate.sol#2368
Severity: Low
2368                 result = (result * 0x1000000058B90BFCE) >> 64;



JBXBuybackDelegate.sol#2370
Severity: Low
2370             if (x & 0x400000000 > 0) {



JBXBuybackDelegate.sol#2371
Severity: Low
2371                 result = (result * 0x100000002C5C85FE3) >> 64;



JBXBuybackDelegate.sol#2373
Severity: Low
2373             if (x & 0x200000000 > 0) {



JBXBuybackDelegate.sol#2374
Severity: Low
2374                 result = (result * 0x10000000162E42FF1) >> 64;



JBXBuybackDelegate.sol#2376
Severity: Low
2376             if (x & 0x100000000 > 0) {



JBXBuybackDelegate.sol#2377
Severity: Low
2377                 result = (result * 0x100000000B17217F8) >> 64;



JBXBuybackDelegate.sol#2379
Severity: Low
2379             if (x & 0x80000000 > 0) {



JBXBuybackDelegate.sol#2380
Severity: Low
2380                 result = (result * 0x10000000058B90BFC) >> 64;



JBXBuybackDelegate.sol#2382
Severity: Low
2382             if (x & 0x40000000 > 0) {



JBXBuybackDelegate.sol#2383
Severity: Low
2383                 result = (result * 0x1000000002C5C85FE) >> 64;



JBXBuybackDelegate.sol#2385
Severity: Low
2385             if (x & 0x20000000 > 0) {



JBXBuybackDelegate.sol#2386
Severity: Low
2386                 result = (result * 0x100000000162E42FF) >> 64;



JBXBuybackDelegate.sol#2388
Severity: Low
2388             if (x & 0x10000000 > 0) {



JBXBuybackDelegate.sol#2389
Severity: Low
2389                 result = (result * 0x1000000000B17217F) >> 64;



JBXBuybackDelegate.sol#2391
Severity: Low
2391             if (x & 0x8000000 > 0) {



JBXBuybackDelegate.sol#2392
Severity: Low
2392                 result = (result * 0x100000000058B90C0) >> 64;



JBXBuybackDelegate.sol#2394
Severity: Low
2394             if (x & 0x4000000 > 0) {



JBXBuybackDelegate.sol#2395
Severity: Low
2395                 result = (result * 0x10000000002C5C860) >> 64;



JBXBuybackDelegate.sol#2397
Severity: Low
2397             if (x & 0x2000000 > 0) {



JBXBuybackDelegate.sol#2398
Severity: Low
2398                 result = (result * 0x1000000000162E430) >> 64;



JBXBuybackDelegate.sol#2400
Severity: Low
2400             if (x & 0x1000000 > 0) {



JBXBuybackDelegate.sol#2401
Severity: Low
2401                 result = (result * 0x10000000000B17218) >> 64;



JBXBuybackDelegate.sol#2403
Severity: Low
2403             if (x & 0x800000 > 0) {



JBXBuybackDelegate.sol#2404
Severity: Low
2404                 result = (result * 0x1000000000058B90C) >> 64;



JBXBuybackDelegate.sol#2406
Severity: Low
2406             if (x & 0x400000 > 0) {



JBXBuybackDelegate.sol#2407
Severity: Low
2407                 result = (result * 0x100000000002C5C86) >> 64;



JBXBuybackDelegate.sol#2409
Severity: Low
2409             if (x & 0x200000 > 0) {



JBXBuybackDelegate.sol#2410
Severity: Low
2410                 result = (result * 0x10000000000162E43) >> 64;



JBXBuybackDelegate.sol#2412
Severity: Low
2412             if (x & 0x100000 > 0) {



JBXBuybackDelegate.sol#2413
Severity: Low
2413                 result = (result * 0x100000000000B1721) >> 64;



JBXBuybackDelegate.sol#2415
Severity: Low
2415             if (x & 0x80000 > 0) {



JBXBuybackDelegate.sol#2416
Severity: Low
2416                 result = (result * 0x10000000000058B91) >> 64;



JBXBuybackDelegate.sol#2418
Severity: Low
2418             if (x & 0x40000 > 0) {



JBXBuybackDelegate.sol#2419
Severity: Low
2419                 result = (result * 0x1000000000002C5C8) >> 64;



JBXBuybackDelegate.sol#2421
Severity: Low
2421             if (x & 0x20000 > 0) {



JBXBuybackDelegate.sol#2422
Severity: Low
2422                 result = (result * 0x100000000000162E4) >> 64;



JBXBuybackDelegate.sol#2424
Severity: Low
2424             if (x & 0x10000 > 0) {



JBXBuybackDelegate.sol#2425
Severity: Low
2425                 result = (result * 0x1000000000000B172) >> 64;



JBXBuybackDelegate.sol#2427
Severity: Low
2427             if (x & 0x8000 > 0) {



JBXBuybackDelegate.sol#2428
Severity: Low
2428                 result = (result * 0x100000000000058B9) >> 64;



JBXBuybackDelegate.sol#2430
Severity: Low
2430             if (x & 0x4000 > 0) {



JBXBuybackDelegate.sol#2431
Severity: Low
2431                 result = (result * 0x10000000000002C5D) >> 64;



JBXBuybackDelegate.sol#2433
Severity: Low
2433             if (x & 0x2000 > 0) {



JBXBuybackDelegate.sol#2434
Severity: Low
2434                 result = (result * 0x1000000000000162E) >> 64;



JBXBuybackDelegate.sol#2436
Severity: Low
2436             if (x & 0x1000 > 0) {



JBXBuybackDelegate.sol#2437
Severity: Low
2437                 result = (result * 0x10000000000000B17) >> 64;



JBXBuybackDelegate.sol#2439
Severity: Low
2439             if (x & 0x800 > 0) {



JBXBuybackDelegate.sol#2440
Severity: Low
2440                 result = (result * 0x1000000000000058C) >> 64;



JBXBuybackDelegate.sol#2442
Severity: Low
2442             if (x & 0x400 > 0) {



JBXBuybackDelegate.sol#2443
Severity: Low
2443                 result = (result * 0x100000000000002C6) >> 64;



JBXBuybackDelegate.sol#2445
Severity: Low
2445             if (x & 0x200 > 0) {



JBXBuybackDelegate.sol#2446
Severity: Low
2446                 result = (result * 0x10000000000000163) >> 64;



JBXBuybackDelegate.sol#2448
Severity: Low
2448             if (x & 0x100 > 0) {



JBXBuybackDelegate.sol#2449
Severity: Low
2449                 result = (result * 0x100000000000000B1) >> 64;



JBXBuybackDelegate.sol#2451
Severity: Low
2451             if (x & 0x80 > 0) {



JBXBuybackDelegate.sol#2452
Severity: Low
2452                 result = (result * 0x10000000000000059) >> 64;



JBXBuybackDelegate.sol#2454
Severity: Low
2454             if (x & 0x40 > 0) {



JBXBuybackDelegate.sol#2455
Severity: Low
2455                 result = (result * 0x1000000000000002C) >> 64;



JBXBuybackDelegate.sol#2457
Severity: Low
2457             if (x & 0x20 > 0) {



JBXBuybackDelegate.sol#2458
Severity: Low
2458                 result = (result * 0x10000000000000016) >> 64;



JBXBuybackDelegate.sol#2460
Severity: Low
2460             if (x & 0x10 > 0) {



JBXBuybackDelegate.sol#2461
Severity: Low
2461                 result = (result * 0x1000000000000000B) >> 64;



JBXBuybackDelegate.sol#2463
Severity: Low
2463             if (x & 0x8 > 0) {



JBXBuybackDelegate.sol#2464
Severity: Low
2464                 result = (result * 0x10000000000000006) >> 64;



JBXBuybackDelegate.sol#2466
Severity: Low
2466             if (x & 0x4 > 0) {



JBXBuybackDelegate.sol#2467
Severity: Low
2467                 result = (result * 0x10000000000000003) >> 64;



JBXBuybackDelegate.sol#2469
Severity: Low
2469             if (x & 0x2 > 0) {



JBXBuybackDelegate.sol#2470
Severity: Low
2470                 result = (result * 0x10000000000000001) >> 64;



JBXBuybackDelegate.sol#2472
Severity: Low
2472             if (x & 0x1 > 0) {



JBXBuybackDelegate.sol#2473
Severity: Low
2473                 result = (result * 0x10000000000000001) >> 64;



JBXBuybackDelegate.sol#3305
Severity: Low
3305             uint256 ratio = absTick & 0x1 != 0



JBXBuybackDelegate.sol#3306
Severity: Low
3306                 ? 0xfffcb933bd6fad37aa2d162d1a594001



JBXBuybackDelegate.sol#3307
Severity: Low
3307                 : 0x100000000000000000000000000000000;



JBXBuybackDelegate.sol#3308
Severity: Low
3308             if (absTick & 0x2 != 0) ratio = (ratio * 0xfff97272373d413259a46990580e213a) >> 128;



JBXBuybackDelegate.sol#3308
Severity: Low
3308             if (absTick & 0x2 != 0) ratio = (ratio * 0xfff97272373d413259a46990580e213a) >> 128;



JBXBuybackDelegate.sol#3309
Severity: Low
3309             if (absTick & 0x4 != 0) ratio = (ratio * 0xfff2e50f5f656932ef12357cf3c7fdcc) >> 128;



JBXBuybackDelegate.sol#3309
Severity: Low
3309             if (absTick & 0x4 != 0) ratio = (ratio * 0xfff2e50f5f656932ef12357cf3c7fdcc) >> 128;



JBXBuybackDelegate.sol#3310
Severity: Low
3310             if (absTick & 0x8 != 0) ratio = (ratio * 0xffe5caca7e10e4e61c3624eaa0941cd0) >> 128;



JBXBuybackDelegate.sol#3310
Severity: Low
3310             if (absTick & 0x8 != 0) ratio = (ratio * 0xffe5caca7e10e4e61c3624eaa0941cd0) >> 128;



JBXBuybackDelegate.sol#3311
Severity: Low
3311             if (absTick & 0x10 != 0) ratio = (ratio * 0xffcb9843d60f6159c9db58835c926644) >> 128;



JBXBuybackDelegate.sol#3311
Severity: Low
3311             if (absTick & 0x10 != 0) ratio = (ratio * 0xffcb9843d60f6159c9db58835c926644) >> 128;



JBXBuybackDelegate.sol#3312
Severity: Low
3312             if (absTick & 0x20 != 0) ratio = (ratio * 0xff973b41fa98c081472e6896dfb254c0) >> 128;



JBXBuybackDelegate.sol#3312
Severity: Low
3312             if (absTick & 0x20 != 0) ratio = (ratio * 0xff973b41fa98c081472e6896dfb254c0) >> 128;



JBXBuybackDelegate.sol#3313
Severity: Low
3313             if (absTick & 0x40 != 0) ratio = (ratio * 0xff2ea16466c96a3843ec78b326b52861) >> 128;



JBXBuybackDelegate.sol#3313
Severity: Low
3313             if (absTick & 0x40 != 0) ratio = (ratio * 0xff2ea16466c96a3843ec78b326b52861) >> 128;



JBXBuybackDelegate.sol#3314
Severity: Low
3314             if (absTick & 0x80 != 0) ratio = (ratio * 0xfe5dee046a99a2a811c461f1969c3053) >> 128;



JBXBuybackDelegate.sol#3314
Severity: Low
3314             if (absTick & 0x80 != 0) ratio = (ratio * 0xfe5dee046a99a2a811c461f1969c3053) >> 128;



JBXBuybackDelegate.sol#3315
Severity: Low
3315             if (absTick & 0x100 != 0) ratio = (ratio * 0xfcbe86c7900a88aedcffc83b479aa3a4) >> 128;



JBXBuybackDelegate.sol#3315
Severity: Low
3315             if (absTick & 0x100 != 0) ratio = (ratio * 0xfcbe86c7900a88aedcffc83b479aa3a4) >> 128;



JBXBuybackDelegate.sol#3316
Severity: Low
3316             if (absTick & 0x200 != 0) ratio = (ratio * 0xf987a7253ac413176f2b074cf7815e54) >> 128;



JBXBuybackDelegate.sol#3316
Severity: Low
3316             if (absTick & 0x200 != 0) ratio = (ratio * 0xf987a7253ac413176f2b074cf7815e54) >> 128;



JBXBuybackDelegate.sol#3317
Severity: Low
3317             if (absTick & 0x400 != 0) ratio = (ratio * 0xf3392b0822b70005940c7a398e4b70f3) >> 128;



JBXBuybackDelegate.sol#3317
Severity: Low
3317             if (absTick & 0x400 != 0) ratio = (ratio * 0xf3392b0822b70005940c7a398e4b70f3) >> 128;



JBXBuybackDelegate.sol#3318
Severity: Low
3318             if (absTick & 0x800 != 0) ratio = (ratio * 0xe7159475a2c29b7443b29c7fa6e889d9) >> 128;



JBXBuybackDelegate.sol#3318
Severity: Low
3318             if (absTick & 0x800 != 0) ratio = (ratio * 0xe7159475a2c29b7443b29c7fa6e889d9) >> 128;



JBXBuybackDelegate.sol#3319
Severity: Low
3319             if (absTick & 0x1000 != 0) ratio = (ratio * 0xd097f3bdfd2022b8845ad8f792aa5825) >> 128;



JBXBuybackDelegate.sol#3319
Severity: Low
3319             if (absTick & 0x1000 != 0) ratio = (ratio * 0xd097f3bdfd2022b8845ad8f792aa5825) >> 128;



JBXBuybackDelegate.sol#3320
Severity: Low
3320             if (absTick & 0x2000 != 0) ratio = (ratio * 0xa9f746462d870fdf8a65dc1f90e061e5) >> 128;



JBXBuybackDelegate.sol#3320
Severity: Low
3320             if (absTick & 0x2000 != 0) ratio = (ratio * 0xa9f746462d870fdf8a65dc1f90e061e5) >> 128;



JBXBuybackDelegate.sol#3321
Severity: Low
3321             if (absTick & 0x4000 != 0) ratio = (ratio * 0x70d869a156d2a1b890bb3df62baf32f7) >> 128;



JBXBuybackDelegate.sol#3321
Severity: Low
3321             if (absTick & 0x4000 != 0) ratio = (ratio * 0x70d869a156d2a1b890bb3df62baf32f7) >> 128;



JBXBuybackDelegate.sol#3322
Severity: Low
3322             if (absTick & 0x8000 != 0) ratio = (ratio * 0x31be135f97d08fd981231505542fcfa6) >> 128;



JBXBuybackDelegate.sol#3322
Severity: Low
3322             if (absTick & 0x8000 != 0) ratio = (ratio * 0x31be135f97d08fd981231505542fcfa6) >> 128;



JBXBuybackDelegate.sol#3323
Severity: Low
3323             if (absTick & 0x10000 != 0) ratio = (ratio * 0x9aa508b5b7a84e1c677de54f3e99bc9) >> 128;



JBXBuybackDelegate.sol#3323
Severity: Low
3323             if (absTick & 0x10000 != 0) ratio = (ratio * 0x9aa508b5b7a84e1c677de54f3e99bc9) >> 128;



JBXBuybackDelegate.sol#3324
Severity: Low
3324             if (absTick & 0x20000 != 0) ratio = (ratio * 0x5d6af8dedb81196699c329225ee604) >> 128;



JBXBuybackDelegate.sol#3324
Severity: Low
3324             if (absTick & 0x20000 != 0) ratio = (ratio * 0x5d6af8dedb81196699c329225ee604) >> 128;



JBXBuybackDelegate.sol#3325
Severity: Low
3325             if (absTick & 0x40000 != 0) ratio = (ratio * 0x2216e584f5fa1ea926041bedfe98) >> 128;



JBXBuybackDelegate.sol#3325
Severity: Low
3325             if (absTick & 0x40000 != 0) ratio = (ratio * 0x2216e584f5fa1ea926041bedfe98) >> 128;



JBXBuybackDelegate.sol#3326
Severity: Low
3326             if (absTick & 0x80000 != 0) ratio = (ratio * 0x48a170391f7dc42444e8fa2) >> 128;



JBXBuybackDelegate.sol#3326
Severity: Low
3326             if (absTick & 0x80000 != 0) ratio = (ratio * 0x48a170391f7dc42444e8fa2) >> 128;



JBXBuybackDelegate.sol#2048
Severity: Low
2048         _transferOwnership(address(0));



```

## SOLIDITY_DIV_MUL
Solidity operates only with integers. Thus, if the division is done before the  multiplication, the rounding errors can increase dramatically.
[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#arithmetic)
Precision issues.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#3629
Severity: Medium
3629         if (_tokenCount < _quote * (1 - _slippage / SLIPPAGE_DENOMINATOR)) {



JBXBuybackDelegate.sol#3673
Severity: Medium
3673             uint256 _minimumReceivedFromSwap = _quote * (1 - _slippage / SLIPPAGE_DENOMINATOR);



```

## SOLIDITY_FUNCTIONS_RETURNS_TYPE_AND_NO_RETURN
Function doesn't initialize return value. As result default value will be returned.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#1730
Severity: Low
1730   function packFundingCycleGlobalMetadata(JBGlobalFundingCycleMetadata memory _metadata)



JBXBuybackDelegate.sol#2493
Severity: Low
2493     function mostSignificantBit(uint256 x) internal pure returns (uint256 msb) {



JBXBuybackDelegate.sol#3708
Severity: Low
3708     function redeemParams(JBRedeemParamsData calldata _data)



```

## SOLIDITY_PRAGMAS_VERSION
Solidity source files indicate the versions of the compiler they can be compiled with.

pragma solidity ^0.4.17; // bad: compiles w 0.4.17 and above
pragma solidity 0.4.24; // good : compiles w 0.4.24 only

It is recommended to follow the latter example, as future compiler versions may handle certain language constructions in a way the developer did not foresee.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#2
Severity: Low
2 pragma solidity ^0.8.16;



```

## SOLIDITY_PRIVATE_MODIFIER_DONT_HIDE_DATA
Contrary to a popular misconception, the ```private``` modifier does not make a variable invisible. Miners have access to all contractsâ€™ code and data. Developers must account for the lack of privacy in Ethereum.

[Vulnerability type by SmartDec classification](https://github.com/smartdec/classification#privacy)

Privacy.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#2007
Severity: Low
2007     address private _owner;



JBXBuybackDelegate.sol#3536
Severity: Low
3536     bool private immutable _projectTokenIsZero;



JBXBuybackDelegate.sol#3541
Severity: Low
3541     uint256 private constant SLIPPAGE_DENOMINATOR = 10000;



JBXBuybackDelegate.sol#3579
Severity: Low
3579     uint256 private mintedAmount = 1;



JBXBuybackDelegate.sol#3586
Severity: Low
3586     uint256 private reservedRate = 1;



```

## SOLIDITY_SHOULD_NOT_BE_PURE
In Solidity, function that do not read from the state or modify it can be declared as ```pure```.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#2543
Severity: Low
2543     function mulDiv(



JBXBuybackDelegate.sol#3342
Severity: Low
3342     function getTickAtSqrtRatio(uint160 sqrtPriceX96) internal pure returns (int24 tick) {



```

## SOLIDITY_SHOULD_RETURN_STRUCT
Consider using struct instead of multiple return values for ```internal``` or ```private``` functions. It can improve code readability.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#288
Severity: Low
288     returns (JBFundingCycle memory fundingCycle, JBBallotState ballotState);



JBXBuybackDelegate.sol#777
Severity: Low
777   ) external view returns (uint256 distributionLimit, uint256 distributionLimitCurrency);



JBXBuybackDelegate.sol#784
Severity: Low
784   ) external view returns (uint256 overflowAllowance, uint256 overflowAllowanceCurrency);



JBXBuybackDelegate.sol#794
Severity: Low
794     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);



JBXBuybackDelegate.sol#799
Severity: Low
799     returns (



JBXBuybackDelegate.sol#808
Severity: Low
808     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);



JBXBuybackDelegate.sol#813
Severity: Low
813     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);



JBXBuybackDelegate.sol#890
Severity: Low
890   ) external view returns (uint256 distributionLimit, uint256 distributionLimitCurrency);



JBXBuybackDelegate.sol#897
Severity: Low
897   ) external view returns (uint256 overflowAllowance, uint256 overflowAllowanceCurrency);



JBXBuybackDelegate.sol#979
Severity: Low
979     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);



JBXBuybackDelegate.sol#984
Severity: Low
984     returns (



JBXBuybackDelegate.sol#993
Severity: Low
993     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);



JBXBuybackDelegate.sol#998
Severity: Low
998     returns (JBFundingCycle memory fundingCycle, JBFundingCycleMetadata memory metadata);



JBXBuybackDelegate.sol#1292
Severity: Low
1292     returns (



JBXBuybackDelegate.sol#1323
Severity: Low
1323     returns (



JBXBuybackDelegate.sol#1510
Severity: Low
1510   ) external returns (JBFundingCycle memory fundingCycle, uint256 distributedAmount);



JBXBuybackDelegate.sol#1516
Severity: Low
1516   ) external returns (JBFundingCycle memory fundingCycle, uint256 withdrawnAmount);



JBXBuybackDelegate.sol#2852
Severity: Low
2852         returns (



JBXBuybackDelegate.sol#2872
Severity: Low
2872     function protocolFees() external view returns (uint128 token0, uint128 token1);



JBXBuybackDelegate.sol#2896
Severity: Low
2896         returns (



JBXBuybackDelegate.sol#2920
Severity: Low
2920         returns (



JBXBuybackDelegate.sol#2939
Severity: Low
2939         returns (



JBXBuybackDelegate.sol#2964
Severity: Low
2964         returns (int56[] memory tickCumulatives, uint160[] memory secondsPerLiquidityCumulativeX128s);



JBXBuybackDelegate.sol#2978
Severity: Low
2978         returns (



JBXBuybackDelegate.sol#3010
Severity: Low
3010     ) external returns (uint256 amount0, uint256 amount1);



JBXBuybackDelegate.sol#3030
Severity: Low
3030     ) external returns (uint128 amount0, uint128 amount1);



JBXBuybackDelegate.sol#3044
Severity: Low
3044     ) external returns (uint256 amount0, uint256 amount1);



JBXBuybackDelegate.sol#3062
Severity: Low
3062     ) external returns (int256 amount0, int256 amount1);



JBXBuybackDelegate.sol#3104
Severity: Low
3104     ) external returns (uint128 amount0, uint128 amount1);



JBXBuybackDelegate.sol#3620
Severity: Low
3620         returns (uint256 weight, string memory memo, JBPayDelegateAllocation[] memory delegateAllocations)



JBXBuybackDelegate.sol#3711
Severity: Low
3711         returns (uint256 reclaimAmount, string memory memo, JBRedemptionDelegateAllocation[] memory delegateAllocations)



```

## SOLIDITY_UPGRADE_TO_050
Prepare your code for Solidity 0.5.0 release.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#1989
Severity: Low
1989     function _msgData() internal view virtual returns (bytes calldata) {



```

## SOLIDITY_USING_INLINE_ASSEMBLY
Inline assembly is a way to access the Ethereum Virtual Machine at a low level. This discards several important safety features of Solidity.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#2553
Severity: Low
2553         assembly {



JBXBuybackDelegate.sol#3351
Severity: Low
3351             assembly {



JBXBuybackDelegate.sol#3356
Severity: Low
3356             assembly {



JBXBuybackDelegate.sol#3361
Severity: Low
3361             assembly {



JBXBuybackDelegate.sol#3366
Severity: Low
3366             assembly {



JBXBuybackDelegate.sol#3371
Severity: Low
3371             assembly {



JBXBuybackDelegate.sol#3376
Severity: Low
3376             assembly {



JBXBuybackDelegate.sol#3381
Severity: Low
3381             assembly {



JBXBuybackDelegate.sol#3386
Severity: Low
3386             assembly {



JBXBuybackDelegate.sol#3396
Severity: Low
3396             assembly {



JBXBuybackDelegate.sol#3402
Severity: Low
3402             assembly {



JBXBuybackDelegate.sol#3408
Severity: Low
3408             assembly {



JBXBuybackDelegate.sol#3414
Severity: Low
3414             assembly {



JBXBuybackDelegate.sol#3420
Severity: Low
3420             assembly {



JBXBuybackDelegate.sol#3426
Severity: Low
3426             assembly {



JBXBuybackDelegate.sol#3432
Severity: Low
3432             assembly {



JBXBuybackDelegate.sol#3438
Severity: Low
3438             assembly {



JBXBuybackDelegate.sol#3444
Severity: Low
3444             assembly {



JBXBuybackDelegate.sol#3450
Severity: Low
3450             assembly {



JBXBuybackDelegate.sol#3456
Severity: Low
3456             assembly {



JBXBuybackDelegate.sol#3462
Severity: Low
3462             assembly {



JBXBuybackDelegate.sol#3468
Severity: Low
3468             assembly {



JBXBuybackDelegate.sol#3474
Severity: Low
3474             assembly {



```

## SOLIDITY_VISIBILITY
The default function visibility level in contracts is ```public```, in interfaces - ```external```, state variable default visibility level is ```internal```.

In contracts, the fallback function can be ```external``` or ```public```. In interfaces, all the functions should be declared as ```external```. Explicitly define function visibility to prevent confusion.


### JBXBuybackDelegate.sol

```

JBXBuybackDelegate.sol#37
Severity: Low
37   function pay(



JBXBuybackDelegate.sol#48
Severity: Low
48   function addToBalanceOf(



JBXBuybackDelegate.sol#296
Severity: Low
296   function configureFor(



JBXBuybackDelegate.sol#659
Severity: Low
659   function issueFor(



JBXBuybackDelegate.sol#815
Severity: Low
815   function launchProjectFor(



JBXBuybackDelegate.sol#827
Severity: Low
827   function launchFundingCyclesFor(



JBXBuybackDelegate.sol#838
Severity: Low
838   function reconfigureFundingCyclesOf(



JBXBuybackDelegate.sol#848
Severity: Low
848   function mintTokensOf(



JBXBuybackDelegate.sol#857
Severity: Low
857   function burnTokensOf(



JBXBuybackDelegate.sol#1000
Severity: Low
1000   function launchProjectFor(



JBXBuybackDelegate.sol#1012
Severity: Low
1012   function launchFundingCyclesFor(



JBXBuybackDelegate.sol#1023
Severity: Low
1023   function reconfigureFundingCyclesOf(



JBXBuybackDelegate.sol#1033
Severity: Low
1033   function mintTokensOf(



JBXBuybackDelegate.sol#1042
Severity: Low
1042   function burnTokensOf(



JBXBuybackDelegate.sol#1344
Severity: Low
1344   function useAllowanceOf(



JBXBuybackDelegate.sol#1361
Severity: Low
1361   function addToBalanceOf(



JBXBuybackDelegate.sol#1405
Severity: Low
1405   function redeemTokensOf(



JBXBuybackDelegate.sol#1474
Severity: Low
1474   function recordPaymentFrom(



JBXBuybackDelegate.sol#1491
Severity: Low
1491   function recordRedemptionFor(



JBXBuybackDelegate.sol#2014
Severity: Low
2014     constructor() {



JBXBuybackDelegate.sol#3591
Severity: Low
3591     constructor(



JBXBuybackDelegate.sol#44
Severity: Low
44     string calldata _memo,



JBXBuybackDelegate.sol#45
Severity: Low
45     bytes calldata _metadata



JBXBuybackDelegate.sol#46
Severity: Low
46   ) external payable returns (uint256 beneficiaryTokenCount);



JBXBuybackDelegate.sol#52
Severity: Low
52     string calldata _memo,



JBXBuybackDelegate.sol#53
Severity: Low
53     bytes calldata _metadata



JBXBuybackDelegate.sol#298
Severity: Low
298     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#299
Severity: Low
299     uint256 _metadata,



JBXBuybackDelegate.sol#300
Severity: Low
300     uint256 _mustStartAtOrAfter



JBXBuybackDelegate.sol#301
Severity: Low
301   ) external returns (JBFundingCycle memory fundingCycle);



JBXBuybackDelegate.sol#661
Severity: Low
661     string calldata _name,



JBXBuybackDelegate.sol#662
Severity: Low
662     string calldata _symbol



JBXBuybackDelegate.sol#663
Severity: Low
663   ) external returns (IJBToken token);



JBXBuybackDelegate.sol#817
Severity: Low
817     JBProjectMetadata calldata _projectMetadata,



JBXBuybackDelegate.sol#818
Severity: Low
818     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#819
Severity: Low
819     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#819
Severity: Low
819     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#820
Severity: Low
820     uint256 _mustStartAtOrAfter,



JBXBuybackDelegate.sol#821
Severity: Low
821     JBGroupedSplits[] memory _groupedSplits,



JBXBuybackDelegate.sol#822
Severity: Low
822     JBFundAccessConstraints[] memory _fundAccessConstraints,



JBXBuybackDelegate.sol#823
Severity: Low
823     IJBPaymentTerminal[] memory _terminals,



JBXBuybackDelegate.sol#824
Severity: Low
824     string calldata _memo



JBXBuybackDelegate.sol#825
Severity: Low
825   ) external returns (uint256 projectId);



JBXBuybackDelegate.sol#829
Severity: Low
829     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#830
Severity: Low
830     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#831
Severity: Low
831     uint256 _mustStartAtOrAfter,



JBXBuybackDelegate.sol#832
Severity: Low
832     JBGroupedSplits[] memory _groupedSplits,



JBXBuybackDelegate.sol#833
Severity: Low
833     JBFundAccessConstraints[] memory _fundAccessConstraints,



JBXBuybackDelegate.sol#834
Severity: Low
834     IJBPaymentTerminal[] memory _terminals,



JBXBuybackDelegate.sol#835
Severity: Low
835     string calldata _memo



JBXBuybackDelegate.sol#836
Severity: Low
836   ) external returns (uint256 configuration);



JBXBuybackDelegate.sol#840
Severity: Low
840     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#841
Severity: Low
841     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#842
Severity: Low
842     uint256 _mustStartAtOrAfter,



JBXBuybackDelegate.sol#843
Severity: Low
843     JBGroupedSplits[] memory _groupedSplits,



JBXBuybackDelegate.sol#844
Severity: Low
844     JBFundAccessConstraints[] memory _fundAccessConstraints,



JBXBuybackDelegate.sol#845
Severity: Low
845     string calldata _memo



JBXBuybackDelegate.sol#846
Severity: Low
846   ) external returns (uint256);



JBXBuybackDelegate.sol#852
Severity: Low
852     string calldata _memo,



JBXBuybackDelegate.sol#853
Severity: Low
853     bool _preferClaimedTokens,



JBXBuybackDelegate.sol#854
Severity: Low
854     bool _useReservedRate



JBXBuybackDelegate.sol#855
Severity: Low
855   ) external returns (uint256 beneficiaryTokenCount);



JBXBuybackDelegate.sol#861
Severity: Low
861     string calldata _memo,



JBXBuybackDelegate.sol#862
Severity: Low
862     bool _preferClaimedTokens



JBXBuybackDelegate.sol#1002
Severity: Low
1002     JBProjectMetadata calldata _projectMetadata,



JBXBuybackDelegate.sol#1003
Severity: Low
1003     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#1004
Severity: Low
1004     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#1004
Severity: Low
1004     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#1005
Severity: Low
1005     uint256 _mustStartAtOrAfter,



JBXBuybackDelegate.sol#1006
Severity: Low
1006     JBGroupedSplits[] memory _groupedSplits,



JBXBuybackDelegate.sol#1007
Severity: Low
1007     JBFundAccessConstraints[] memory _fundAccessConstraints,



JBXBuybackDelegate.sol#1008
Severity: Low
1008     IJBPaymentTerminal[] memory _terminals,



JBXBuybackDelegate.sol#1009
Severity: Low
1009     string calldata _memo



JBXBuybackDelegate.sol#1010
Severity: Low
1010   ) external returns (uint256 projectId);



JBXBuybackDelegate.sol#1014
Severity: Low
1014     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#1015
Severity: Low
1015     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#1016
Severity: Low
1016     uint256 _mustStartAtOrAfter,



JBXBuybackDelegate.sol#1017
Severity: Low
1017     JBGroupedSplits[] memory _groupedSplits,



JBXBuybackDelegate.sol#1018
Severity: Low
1018     JBFundAccessConstraints[] memory _fundAccessConstraints,



JBXBuybackDelegate.sol#1019
Severity: Low
1019     IJBPaymentTerminal[] memory _terminals,



JBXBuybackDelegate.sol#1020
Severity: Low
1020     string calldata _memo



JBXBuybackDelegate.sol#1021
Severity: Low
1021   ) external returns (uint256 configuration);



JBXBuybackDelegate.sol#1025
Severity: Low
1025     JBFundingCycleData calldata _data,



JBXBuybackDelegate.sol#1026
Severity: Low
1026     JBFundingCycleMetadata calldata _metadata,



JBXBuybackDelegate.sol#1027
Severity: Low
1027     uint256 _mustStartAtOrAfter,



JBXBuybackDelegate.sol#1028
Severity: Low
1028     JBGroupedSplits[] memory _groupedSplits,



JBXBuybackDelegate.sol#1029
Severity: Low
1029     JBFundAccessConstraints[] memory _fundAccessConstraints,



JBXBuybackDelegate.sol#1030
Severity: Low
1030     string calldata _memo



JBXBuybackDelegate.sol#1031
Severity: Low
1031   ) external returns (uint256);



JBXBuybackDelegate.sol#1037
Severity: Low
1037     string calldata _memo,



JBXBuybackDelegate.sol#1038
Severity: Low
1038     bool _preferClaimedTokens,



JBXBuybackDelegate.sol#1039
Severity: Low
1039     bool _useReservedRate



JBXBuybackDelegate.sol#1040
Severity: Low
1040   ) external returns (uint256 beneficiaryTokenCount);



JBXBuybackDelegate.sol#1046
Severity: Low
1046     string calldata _memo,



JBXBuybackDelegate.sol#1047
Severity: Low
1047     bool _preferClaimedTokens



JBXBuybackDelegate.sol#1350
Severity: Low
1350     address payable _beneficiary,



JBXBuybackDelegate.sol#1351
Severity: Low
1351     string calldata _memo,



JBXBuybackDelegate.sol#1351
Severity: Low
1351     string calldata _memo,



JBXBuybackDelegate.sol#1352
Severity: Low
1352     bytes calldata _metadata



JBXBuybackDelegate.sol#1353
Severity: Low
1353   ) external returns (uint256 netDistributedAmount);



JBXBuybackDelegate.sol#1366
Severity: Low
1366     string calldata _memo,



JBXBuybackDelegate.sol#1367
Severity: Low
1367     bytes calldata _metadata



JBXBuybackDelegate.sol#1411
Severity: Low
1411     address payable _beneficiary,



JBXBuybackDelegate.sol#1412
Severity: Low
1412     string calldata _memo,



JBXBuybackDelegate.sol#1412
Severity: Low
1412     string calldata _memo,



JBXBuybackDelegate.sol#1413
Severity: Low
1413     bytes calldata _metadata



JBXBuybackDelegate.sol#1414
Severity: Low
1414   ) external returns (uint256 reclaimAmount);



JBXBuybackDelegate.sol#1480
Severity: Low
1480     string calldata _memo,



JBXBuybackDelegate.sol#1481
Severity: Low
1481     bytes calldata _metadata



JBXBuybackDelegate.sol#1484
Severity: Low
1484     returns (



JBXBuybackDelegate.sol#1486
Severity: Low
1486       uint256 tokenCount,



JBXBuybackDelegate.sol#1487
Severity: Low
1487       JBPayDelegateAllocation[] memory delegateAllocations,



JBXBuybackDelegate.sol#1488
Severity: Low
1488       string memory memo



JBXBuybackDelegate.sol#1495
Severity: Low
1495     string calldata _memo,



JBXBuybackDelegate.sol#1496
Severity: Low
1496     bytes calldata _metadata



JBXBuybackDelegate.sol#1499
Severity: Low
1499     returns (



JBXBuybackDelegate.sol#1501
Severity: Low
1501       uint256 reclaimAmount,



JBXBuybackDelegate.sol#1502
Severity: Low
1502       JBRedemptionDelegateAllocation[] memory delegateAllocations,



JBXBuybackDelegate.sol#1503
Severity: Low
1503       string memory memo



JBXBuybackDelegate.sol#2568
Severity: Low
2568         if (prod1 >= denominator) {



JBXBuybackDelegate.sol#2569
Severity: Low
2569             revert PRBMath__MulDivOverflow(prod1, denominator);



JBXBuybackDelegate.sol#2569
Severity: Low
2569             revert PRBMath__MulDivOverflow(prod1, denominator);



JBXBuybackDelegate.sol#3110
Severity: Low
3110     error LOK();



JBXBuybackDelegate.sol#3110
Severity: Low
3110     error LOK();



JBXBuybackDelegate.sol#3111
Severity: Low
3111     error TLU();



JBXBuybackDelegate.sol#3111
Severity: Low
3111     error TLU();



JBXBuybackDelegate.sol#3112
Severity: Low
3112     error TLM();



JBXBuybackDelegate.sol#3112
Severity: Low
3112     error TLM();



JBXBuybackDelegate.sol#3113
Severity: Low
3113     error TUM();



JBXBuybackDelegate.sol#3113
Severity: Low
3113     error TUM();



JBXBuybackDelegate.sol#3114
Severity: Low
3114     error AI();



JBXBuybackDelegate.sol#3114
Severity: Low
3114     error AI();



JBXBuybackDelegate.sol#3115
Severity: Low
3115     error M0();



JBXBuybackDelegate.sol#3115
Severity: Low
3115     error M0();



JBXBuybackDelegate.sol#3116
Severity: Low
3116     error M1();



JBXBuybackDelegate.sol#3116
Severity: Low
3116     error M1();



JBXBuybackDelegate.sol#3117
Severity: Low
3117     error AS();



JBXBuybackDelegate.sol#3117
Severity: Low
3117     error AS();



JBXBuybackDelegate.sol#3118
Severity: Low
3118     error IIA();



JBXBuybackDelegate.sol#3118
Severity: Low
3118     error IIA();



JBXBuybackDelegate.sol#3119
Severity: Low
3119     error L();



JBXBuybackDelegate.sol#3119
Severity: Low
3119     error L();



JBXBuybackDelegate.sol#3120
Severity: Low
3120     error F0();



JBXBuybackDelegate.sol#3120
Severity: Low
3120     error F0();



JBXBuybackDelegate.sol#3121
Severity: Low
3121     error F1();



JBXBuybackDelegate.sol#3121
Severity: Low
3121     error F1();



JBXBuybackDelegate.sol#3282
Severity: Low
3282     error T();



JBXBuybackDelegate.sol#3282
Severity: Low
3282     error T();



JBXBuybackDelegate.sol#3283
Severity: Low
3283     error R();



JBXBuybackDelegate.sol#3283
Severity: Low
3283     error R();



JBXBuybackDelegate.sol#3519
Severity: Low
3519     error JuiceBuyback_Unauthorized();



JBXBuybackDelegate.sol#3519
Severity: Low
3519     error JuiceBuyback_Unauthorized();



JBXBuybackDelegate.sol#3520
Severity: Low
3520     error JuiceBuyback_MaximumSlippage();



JBXBuybackDelegate.sol#3520
Severity: Low
3520     error JuiceBuyback_MaximumSlippage();



```
