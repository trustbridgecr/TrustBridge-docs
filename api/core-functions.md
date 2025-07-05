# 6.1 Core Functions

All interactions happen on-chain via Soroban on Stellar’s Futurenet.

## `init_pool`
**Role:** Platform  
Initializes a new pool with parameters like interest model, accepted assets, collateral ratio, and risk settings.

## `deposit`
**Role:** Lender  
Supplies liquidity to a pool. 80% goes to active pool, 20% to backstop.

## `borrow`
**Role:** Borrower  
Requests a loan from the pool. Requires XLM collateral and unfrozen pool.

## `repay`
**Role:** Borrower  
Repays loan + interest. Unlocks collateral and updates TRBT score.

## `withdraw`
**Role:** Lender  
Withdraws available liquidity if pool has sufficient funds.

## `freeze_pool`
**Role:** Protocol  
Automatically triggered if risk levels (e.g., backstop ratio) fall below safe thresholds.