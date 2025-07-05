# 6.4 Borrower Actions

## `borrow`
Initiates a loan from the pool. Requires:
- Loan amount
- Collateral (XLM)
- Pool not frozen

## `repay`
Repays the loan with interest. Unlocks collateral and improves TRBT.

## `simulate_loan`
Estimates interest, repayment, and required collateral before submitting.