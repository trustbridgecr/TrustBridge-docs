# 2.1 Lending Lifecycle

TrustBridge facilitates decentralized microloans through programmable lending pools and on-chain collateralization.

## 1. Loan Request
Borrowers connect their wallet and select an active lending pool. They specify:
- Loan amount
- Purpose
- Duration
They must lock a fixed percentage (e.g. 20%) of the loan amount in XLM as collateral.

## 2. Liquidity Allocation
Once initiated:
- 80% of lender deposits go to active liquidity.
- 20% of lender funds go to a backstop reserve (insurance against defaults).

## 3. Disbursement
After Blend verifies that:
- The borrower’s collateral is sufficient, and
- The pool is not frozen or risky,

...the stablecoin (e.g. USDC) is sent to the borrower's wallet.

## 4. Interest Accrual
Lenders earn interest based on:
- Share of liquidity
- Pool utilization
- Dynamic rate adjustment by Blend

## 5. Repayment
Borrowers must repay the loan (principal + interest) before the deadline. If successful:
- Collateral is released
- TRBT score is increased

## 6. Default Handling
If the borrower fails to repay:
- XLM collateral is liquidated
- Backstop fund covers any remaining shortfall

## 7. Risk Monitoring & Freezing
Blend Engine monitors:
- Pool health
- Defaults
- Utilization and backstop

If thresholds are breached, the pool is frozen automatically.