## Sūrya's Description Report

### Files Description Table


|  File Name  |
|-------------|
| amm/KcsDexRouter.sol |
| amm/KcsFactory.sol |
| amm/KcsRouter.sol |
| interfaces/IERC20.sol |
| interfaces/IGovernanceToken.sol |
| interfaces/IMasterBreeder.sol |
| Authorizable.sol |
| KDEX.sol |
| MasterBreeder.sol |
| Timelock.sol |


### Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **IKcsDexFactory** | Interface |  |||
| └ | feeTo | External ❗️ |   |NO❗️ |
| └ | feeToSetter | External ❗️ |   |NO❗️ |
| └ | getPair | External ❗️ |   |NO❗️ |
| └ | allPairs | External ❗️ |   |NO❗️ |
| └ | allPairsLength | External ❗️ |   |NO❗️ |
| └ | createPair | External ❗️ | 🛑  |NO❗️ |
| └ | setFeeTo | External ❗️ | 🛑  |NO❗️ |
| └ | setFeeToSetter | External ❗️ | 🛑  |NO❗️ |
||||||
| **TransferHelper** | Library |  |||
| └ | safeApprove | Internal 🔒 | 🛑  | |
| └ | safeTransfer | Internal 🔒 | 🛑  | |
| └ | safeTransferFrom | Internal 🔒 | 🛑  | |
| └ | safeTransferETH | Internal 🔒 | 🛑  | |
||||||
| **IKcsDexRouter01** | Interface |  |||
| └ | factory | External ❗️ |   |NO❗️ |
| └ | WETH | External ❗️ |   |NO❗️ |
| └ | addLiquidity | External ❗️ | 🛑  |NO❗️ |
| └ | addLiquidityETH | External ❗️ |  💵 |NO❗️ |
| └ | removeLiquidity | External ❗️ | 🛑  |NO❗️ |
| └ | removeLiquidityETH | External ❗️ | 🛑  |NO❗️ |
| └ | removeLiquidityWithPermit | External ❗️ | 🛑  |NO❗️ |
| └ | removeLiquidityETHWithPermit | External ❗️ | 🛑  |NO❗️ |
| └ | swapExactTokensForTokens | External ❗️ | 🛑  |NO❗️ |
| └ | swapTokensForExactTokens | External ❗️ | 🛑  |NO❗️ |
| └ | swapExactETHForTokens | External ❗️ |  💵 |NO❗️ |
| └ | swapTokensForExactETH | External ❗️ | 🛑  |NO❗️ |
| └ | swapExactTokensForETH | External ❗️ | 🛑  |NO❗️ |
| └ | swapETHForExactTokens | External ❗️ |  💵 |NO❗️ |
| └ | quote | External ❗️ |   |NO❗️ |
| └ | getAmountOut | External ❗️ |   |NO❗️ |
| └ | getAmountIn | External ❗️ |   |NO❗️ |
| └ | getAmountsOut | External ❗️ |   |NO❗️ |
| └ | getAmountsIn | External ❗️ |   |NO❗️ |
||||||
| **IKcsDexRouter02** | Interface | IKcsDexRouter01 |||
| └ | removeLiquidityETHSupportingFeeOnTransferTokens | External ❗️ | 🛑  |NO❗️ |
| └ | removeLiquidityETHWithPermitSupportingFeeOnTransferTokens | External ❗️ | 🛑  |NO❗️ |
| └ | swapExactTokensForTokensSupportingFeeOnTransferTokens | External ❗️ | 🛑  |NO❗️ |
| └ | swapExactETHForTokensSupportingFeeOnTransferTokens | External ❗️ |  💵 |NO❗️ |
| └ | swapExactTokensForETHSupportingFeeOnTransferTokens | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKcsDexPair** | Interface |  |||
| └ | name | External ❗️ |   |NO❗️ |
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | decimals | External ❗️ |   |NO❗️ |
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
| └ | DOMAIN_SEPARATOR | External ❗️ |   |NO❗️ |
| └ | PERMIT_TYPEHASH | External ❗️ |   |NO❗️ |
| └ | nonces | External ❗️ |   |NO❗️ |
| └ | permit | External ❗️ | 🛑  |NO❗️ |
| └ | MINIMUM_LIQUIDITY | External ❗️ |   |NO❗️ |
| └ | factory | External ❗️ |   |NO❗️ |
| └ | token0 | External ❗️ |   |NO❗️ |
| └ | token1 | External ❗️ |   |NO❗️ |
| └ | getReserves | External ❗️ |   |NO❗️ |
| └ | price0CumulativeLast | External ❗️ |   |NO❗️ |
| └ | price1CumulativeLast | External ❗️ |   |NO❗️ |
| └ | kLast | External ❗️ |   |NO❗️ |
| └ | mint | External ❗️ | 🛑  |NO❗️ |
| └ | burn | External ❗️ | 🛑  |NO❗️ |
| └ | swap | External ❗️ | 🛑  |NO❗️ |
| └ | skim | External ❗️ | 🛑  |NO❗️ |
| └ | sync | External ❗️ | 🛑  |NO❗️ |
| └ | initialize | External ❗️ | 🛑  |NO❗️ |
||||||
| **SafeMath** | Library |  |||
| └ | add | Internal 🔒 |   | |
| └ | sub | Internal 🔒 |   | |
| └ | mul | Internal 🔒 |   | |
||||||
| **KcsDexLibrary** | Library |  |||
| └ | sortTokens | Internal 🔒 |   | |
| └ | pairFor | Internal 🔒 |   | |
| └ | getReserves | Internal 🔒 |   | |
| └ | quote | Internal 🔒 |   | |
| └ | getAmountOut | Internal 🔒 |   | |
| └ | getAmountIn | Internal 🔒 |   | |
| └ | getAmountsOut | Internal 🔒 |   | |
| └ | getAmountsIn | Internal 🔒 |   | |
||||||
| **IERC20** | Interface |  |||
| └ | name | External ❗️ |   |NO❗️ |
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | decimals | External ❗️ |   |NO❗️ |
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
||||||
| **IWETH** | Interface |  |||
| └ | deposit | External ❗️ |  💵 |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | withdraw | External ❗️ | 🛑  |NO❗️ |
||||||
| **KcsDexRouter** | Implementation | IKcsDexRouter02 |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | <Receive Ether> | External ❗️ |  💵 |NO❗️ |
| └ | _addLiquidity | Internal 🔒 | 🛑  | |
| └ | addLiquidity | External ❗️ | 🛑  | ensure |
| └ | addLiquidityETH | External ❗️ |  💵 | ensure |
| └ | removeLiquidity | Public ❗️ | 🛑  | ensure |
| └ | removeLiquidityETH | Public ❗️ | 🛑  | ensure |
| └ | removeLiquidityWithPermit | External ❗️ | 🛑  |NO❗️ |
| └ | removeLiquidityETHWithPermit | External ❗️ | 🛑  |NO❗️ |
| └ | removeLiquidityETHSupportingFeeOnTransferTokens | Public ❗️ | 🛑  | ensure |
| └ | removeLiquidityETHWithPermitSupportingFeeOnTransferTokens | External ❗️ | 🛑  |NO❗️ |
| └ | _swap | Internal 🔒 | 🛑  | |
| └ | swapExactTokensForTokens | External ❗️ | 🛑  | ensure |
| └ | swapTokensForExactTokens | External ❗️ | 🛑  | ensure |
| └ | swapExactETHForTokens | External ❗️ |  💵 | ensure |
| └ | swapTokensForExactETH | External ❗️ | 🛑  | ensure |
| └ | swapExactTokensForETH | External ❗️ | 🛑  | ensure |
| └ | swapETHForExactTokens | External ❗️ |  💵 | ensure |
| └ | _swapSupportingFeeOnTransferTokens | Internal 🔒 | 🛑  | |
| └ | swapExactTokensForTokensSupportingFeeOnTransferTokens | External ❗️ | 🛑  | ensure |
| └ | swapExactETHForTokensSupportingFeeOnTransferTokens | External ❗️ |  💵 | ensure |
| └ | swapExactTokensForETHSupportingFeeOnTransferTokens | External ❗️ | 🛑  | ensure |
| └ | quote | Public ❗️ |   |NO❗️ |
| └ | getAmountOut | Public ❗️ |   |NO❗️ |
| └ | getAmountIn | Public ❗️ |   |NO❗️ |
| └ | getAmountsOut | Public ❗️ |   |NO❗️ |
| └ | getAmountsIn | Public ❗️ |   |NO❗️ |
||||||
| **IKcsDexFactory** | Interface |  |||
| └ | feeTo | External ❗️ |   |NO❗️ |
| └ | feeToSetter | External ❗️ |   |NO❗️ |
| └ | getPair | External ❗️ |   |NO❗️ |
| └ | allPairs | External ❗️ |   |NO❗️ |
| └ | allPairsLength | External ❗️ |   |NO❗️ |
| └ | createPair | External ❗️ | 🛑  |NO❗️ |
| └ | setFeeTo | External ❗️ | 🛑  |NO❗️ |
| └ | setFeeToSetter | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKcsDexPair** | Interface |  |||
| └ | name | External ❗️ |   |NO❗️ |
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | decimals | External ❗️ |   |NO❗️ |
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
| └ | DOMAIN_SEPARATOR | External ❗️ |   |NO❗️ |
| └ | PERMIT_TYPEHASH | External ❗️ |   |NO❗️ |
| └ | nonces | External ❗️ |   |NO❗️ |
| └ | permit | External ❗️ | 🛑  |NO❗️ |
| └ | MINIMUM_LIQUIDITY | External ❗️ |   |NO❗️ |
| └ | factory | External ❗️ |   |NO❗️ |
| └ | token0 | External ❗️ |   |NO❗️ |
| └ | token1 | External ❗️ |   |NO❗️ |
| └ | getReserves | External ❗️ |   |NO❗️ |
| └ | price0CumulativeLast | External ❗️ |   |NO❗️ |
| └ | price1CumulativeLast | External ❗️ |   |NO❗️ |
| └ | kLast | External ❗️ |   |NO❗️ |
| └ | mint | External ❗️ | 🛑  |NO❗️ |
| └ | burn | External ❗️ | 🛑  |NO❗️ |
| └ | swap | External ❗️ | 🛑  |NO❗️ |
| └ | skim | External ❗️ | 🛑  |NO❗️ |
| └ | sync | External ❗️ | 🛑  |NO❗️ |
| └ | initialize | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKcsDexERC20** | Interface |  |||
| └ | name | External ❗️ |   |NO❗️ |
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | decimals | External ❗️ |   |NO❗️ |
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
| └ | DOMAIN_SEPARATOR | External ❗️ |   |NO❗️ |
| └ | PERMIT_TYPEHASH | External ❗️ |   |NO❗️ |
| └ | nonces | External ❗️ |   |NO❗️ |
| └ | permit | External ❗️ | 🛑  |NO❗️ |
||||||
| **SafeMath** | Library |  |||
| └ | add | Internal 🔒 |   | |
| └ | sub | Internal 🔒 |   | |
| └ | mul | Internal 🔒 |   | |
||||||
| **KcsDexERC20** | Implementation | IKcsDexERC20 |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | _mint | Internal 🔒 | 🛑  | |
| └ | _burn | Internal 🔒 | 🛑  | |
| └ | _approve | Private 🔐 | 🛑  | |
| └ | _transfer | Private 🔐 | 🛑  | |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
| └ | permit | External ❗️ | 🛑  |NO❗️ |
||||||
| **Math** | Library |  |||
| └ | min | Internal 🔒 |   | |
| └ | sqrt | Internal 🔒 |   | |
||||||
| **UQ112x112** | Library |  |||
| └ | encode | Internal 🔒 |   | |
| └ | uqdiv | Internal 🔒 |   | |
||||||
| **IERC20** | Interface |  |||
| └ | name | External ❗️ |   |NO❗️ |
| └ | symbol | External ❗️ |   |NO❗️ |
| └ | decimals | External ❗️ |   |NO❗️ |
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKcsDexCallee** | Interface |  |||
| └ | kcsdexCall | External ❗️ | 🛑  |NO❗️ |
||||||
| **KcsDexPair** | Implementation | IKcsDexPair, KcsDexERC20 |||
| └ | getReserves | Public ❗️ |   |NO❗️ |
| └ | _safeTransfer | Private 🔐 | 🛑  | |
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | initialize | External ❗️ | 🛑  |NO❗️ |
| └ | _update | Private 🔐 | 🛑  | |
| └ | _mintFee | Private 🔐 | 🛑  | |
| └ | mint | External ❗️ | 🛑  | lock |
| └ | burn | External ❗️ | 🛑  | lock |
| └ | swap | External ❗️ | 🛑  | lock |
| └ | skim | External ❗️ | 🛑  | lock |
| └ | sync | External ❗️ | 🛑  | lock |
||||||
| **KcsDexFactory** | Implementation | IKcsDexFactory |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | allPairsLength | External ❗️ |   |NO❗️ |
| └ | createPair | External ❗️ | 🛑  |NO❗️ |
| └ | setFeeTo | External ❗️ | 🛑  |NO❗️ |
| └ | setFeeToSetter | External ❗️ | 🛑  |NO❗️ |
||||||
| **IERC20** | Interface |  |||
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | permit | External ❗️ | 🛑  |NO❗️ |
||||||
| **IKDEX** | Interface |  |||
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | permit | External ❗️ | 🛑  |NO❗️ |
| └ | cap | External ❗️ |   |NO❗️ |
| └ | capUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lockFromUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lockToUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | unlockedSupply | External ❗️ |   |NO❗️ |
| └ | lockedSupply | External ❗️ |   |NO❗️ |
| └ | circulatingSupply | External ❗️ |   |NO❗️ |
| └ | totalLock | External ❗️ |   |NO❗️ |
| └ | mint | External ❗️ | 🛑  |NO❗️ |
| └ | manualMint | External ❗️ | 🛑  |NO❗️ |
| └ | totalBalanceOf | External ❗️ |   |NO❗️ |
| └ | lockOf | External ❗️ |   |NO❗️ |
| └ | lastUnlockBlock | External ❗️ |   |NO❗️ |
| └ | lock | External ❗️ | 🛑  |NO❗️ |
| └ | canUnlockAmount | External ❗️ |   |NO❗️ |
| └ | unlock | External ❗️ | 🛑  |NO❗️ |
| └ | transferAll | External ❗️ | 🛑  |NO❗️ |
| └ | delegates | External ❗️ |   |NO❗️ |
| └ | delegate | External ❗️ | 🛑  |NO❗️ |
| └ | delegateBySig | External ❗️ | 🛑  |NO❗️ |
| └ | getCurrentVotes | External ❗️ |   |NO❗️ |
| └ | getPriorVotes | External ❗️ |   |NO❗️ |
||||||
| **IMasterBreeder** | Interface |  |||
| └ | poolId1 | External ❗️ | 🛑  |NO❗️ |
| └ | userInfo | External ❗️ |   |NO❗️ |
| └ | poolExistence | External ❗️ |   |NO❗️ |
| └ | poolLength | External ❗️ |   |NO❗️ |
| └ | add | External ❗️ | 🛑  |NO❗️ |
| └ | set | External ❗️ | 🛑  |NO❗️ |
| └ | massUpdatePools | External ❗️ | 🛑  |NO❗️ |
| └ | updatePool | External ❗️ | 🛑  |NO❗️ |
| └ | getMultiplier | External ❗️ |   |NO❗️ |
| └ | getPoolReward | External ❗️ |   |NO❗️ |
| └ | pendingReward | External ❗️ |   |NO❗️ |
| └ | claimRewards | External ❗️ | 🛑  |NO❗️ |
| └ | claimReward | External ❗️ | 🛑  |NO❗️ |
| └ | getGlobalAmount | External ❗️ |   |NO❗️ |
| └ | getGlobalRefAmount | External ❗️ |   |NO❗️ |
| └ | getTotalRefs | External ❗️ |   |NO❗️ |
| └ | getRefValueOf | External ❗️ |   |NO❗️ |
| └ | deposit | External ❗️ | 🛑  |NO❗️ |
| └ | withdraw | External ❗️ | 🛑  |NO❗️ |
| └ | emergencyWithdraw | External ❗️ | 🛑  |NO❗️ |
| └ | dev | External ❗️ | 🛑  |NO❗️ |
| └ | bonusFinishUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | halvingUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lpUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | comUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | founderUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | rewardUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | rewardMulUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lockUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lockdevUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | locklpUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lockcomUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | lockfounderUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | starblockUpdate | External ❗️ | 🛑  |NO❗️ |
| └ | getNewRewardPerBlock | External ❗️ |   |NO❗️ |
| └ | userDelta | External ❗️ |   |NO❗️ |
| └ | reviseWithdraw | External ❗️ | 🛑  |NO❗️ |
| └ | reviseDeposit | External ❗️ | 🛑  |NO❗️ |
| └ | setStageStarts | External ❗️ | 🛑  |NO❗️ |
| └ | setStageEnds | External ❗️ | 🛑  |NO❗️ |
| └ | setUserFeeStage | External ❗️ | 🛑  |NO❗️ |
| └ | setDevFeeStage | External ❗️ | 🛑  |NO❗️ |
| └ | setDevDepFee | External ❗️ | 🛑  |NO❗️ |
| └ | setUserDepFee | External ❗️ | 🛑  |NO❗️ |
| └ | reclaimTokenOwnership | External ❗️ | 🛑  |NO❗️ |
||||||
| **Authorizable** | Implementation | Ownable |||
| └ | addAuthorized | Public ❗️ | 🛑  | onlyOwner |
| └ | removeAuthorized | Public ❗️ | 🛑  | onlyOwner |
||||||
| **KDEX** | Implementation | ERC20, Ownable, Authorizable |||
| └ | <Constructor> | Public ❗️ | 🛑  | ERC20 |
| └ | cap | Public ❗️ |   |NO❗️ |
| └ | capUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lockFromUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lockToUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | unlockedSupply | Public ❗️ |   |NO❗️ |
| └ | lockedSupply | Public ❗️ |   |NO❗️ |
| └ | circulatingSupply | Public ❗️ |   |NO❗️ |
| └ | totalLock | Public ❗️ |   |NO❗️ |
| └ | _beforeTokenTransfer | Internal 🔒 | 🛑  | |
| └ | _transfer | Internal 🔒 | 🛑  | |
| └ | mint | Public ❗️ | 🛑  | onlyOwner |
| └ | manualMint | Public ❗️ | 🛑  | onlyAuthorized |
| └ | totalBalanceOf | Public ❗️ |   |NO❗️ |
| └ | lockOf | Public ❗️ |   |NO❗️ |
| └ | lastUnlockBlock | Public ❗️ |   |NO❗️ |
| └ | lock | Public ❗️ | 🛑  | onlyOwner |
| └ | canUnlockAmount | Public ❗️ |   |NO❗️ |
| └ | unlock | Public ❗️ | 🛑  |NO❗️ |
| └ | transferAll | Public ❗️ | 🛑  |NO❗️ |
| └ | delegates | External ❗️ |   |NO❗️ |
| └ | delegate | External ❗️ | 🛑  |NO❗️ |
| └ | delegateBySig | External ❗️ | 🛑  |NO❗️ |
| └ | getCurrentVotes | External ❗️ |   |NO❗️ |
| └ | getPriorVotes | External ❗️ |   |NO❗️ |
| └ | _delegate | Internal 🔒 | 🛑  | |
| └ | _moveDelegates | Internal 🔒 | 🛑  | |
| └ | _writeCheckpoint | Internal 🔒 | 🛑  | |
| └ | safe32 | Internal 🔒 |   | |
| └ | getChainId | Internal 🔒 |   | |
||||||
| **MasterBreeder** | Implementation | Ownable, Authorizable, ReentrancyGuard |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | poolLength | External ❗️ |   |NO❗️ |
| └ | add | Public ❗️ | 🛑  | onlyOwner nonDuplicated |
| └ | set | Public ❗️ | 🛑  | onlyOwner |
| └ | massUpdatePools | Public ❗️ | 🛑  |NO❗️ |
| └ | updatePool | Public ❗️ | 🛑  |NO❗️ |
| └ | getMultiplier | Public ❗️ |   |NO❗️ |
| └ | getPoolReward | Public ❗️ |   |NO❗️ |
| └ | pendingReward | External ❗️ |   |NO❗️ |
| └ | claimRewards | Public ❗️ | 🛑  |NO❗️ |
| └ | claimReward | Public ❗️ | 🛑  |NO❗️ |
| └ | _harvest | Internal 🔒 | 🛑  | |
| └ | getGlobalAmount | Public ❗️ |   |NO❗️ |
| └ | getGlobalRefAmount | Public ❗️ |   |NO❗️ |
| └ | getTotalRefs | Public ❗️ |   |NO❗️ |
| └ | getRefValueOf | Public ❗️ |   |NO❗️ |
| └ | deposit | Public ❗️ | 🛑  | nonReentrant |
| └ | withdraw | Public ❗️ | 🛑  | nonReentrant |
| └ | emergencyWithdraw | Public ❗️ | 🛑  | nonReentrant |
| └ | safeGovTokenTransfer | Internal 🔒 | 🛑  | |
| └ | dev | Public ❗️ | 🛑  | onlyAuthorized |
| └ | bonusFinishUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | halvingUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lpUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | comUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | founderUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | rewardUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | rewardMulUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lockUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lockdevUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | locklpUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lockcomUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | lockfounderUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | starblockUpdate | Public ❗️ | 🛑  | onlyAuthorized |
| └ | getNewRewardPerBlock | Public ❗️ |   |NO❗️ |
| └ | userDelta | Public ❗️ |   |NO❗️ |
| └ | reviseWithdraw | Public ❗️ | 🛑  | onlyAuthorized |
| └ | reviseDeposit | Public ❗️ | 🛑  | onlyAuthorized |
| └ | setStageStarts | Public ❗️ | 🛑  | onlyAuthorized |
| └ | setStageEnds | Public ❗️ | 🛑  | onlyAuthorized |
| └ | setUserFeeStage | Public ❗️ | 🛑  | onlyAuthorized |
| └ | setDevFeeStage | Public ❗️ | 🛑  | onlyAuthorized |
| └ | setDevDepFee | Public ❗️ | 🛑  | onlyAuthorized |
| └ | setUserDepFee | Public ❗️ | 🛑  | onlyAuthorized |
| └ | reclaimTokenOwnership | Public ❗️ | 🛑  | onlyAuthorized |
||||||
| **Timelock** | Implementation |  |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | <Receive Ether> | External ❗️ |  💵 |NO❗️ |
| └ | setDelay | Public ❗️ | 🛑  |NO❗️ |
| └ | acceptAdmin | Public ❗️ | 🛑  |NO❗️ |
| └ | setPendingAdmin | Public ❗️ | 🛑  |NO❗️ |
| └ | queueTransaction | Public ❗️ | 🛑  |NO❗️ |
| └ | cancelTransaction | Public ❗️ | 🛑  |NO❗️ |
| └ | executeTransaction | Public ❗️ |  💵 |NO❗️ |
| └ | getBlockTimestamp | Internal 🔒 |   | |


### Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |
