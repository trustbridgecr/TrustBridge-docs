# 2.4 Loan Flow

## 1. Pool Access
Borrower selects a TrustBridge pool via the frontend.

## 2. Collateral Submission
Borrower deposits XLM to meet collateral ratio. Verified via oracle.

## 3. Loan Disbursement
If conditions are met, Blend sends USDC directly to borrower.

## 4. Interest Accrual
Lenders start earning interest immediately. Rates depend on demand and utilization.

## 5. Repayment
Borrower repays loan (principal + interest). Collateral is released and TRBT score updated.

## 6. Default
If borrower fails:
- Collateral is liquidated
- Backstop covers remaining shortfall
- Risk level is updated