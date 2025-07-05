# 6.2 Helper + Platform Functions

## `get_pool_info`
**Role:** All  
Returns metadata for the pool: utilization, size, rates, backstop, etc.

## `get_user_position`
**Role:** All  
Returns user’s wallet role, balance, TRBT score, and exposure.

## `update_trbt_score`
**Role:** Protocol  
Updates TRBT score after repayment or default.

## `simulate_loan`
**Role:** All  
Returns interest/collateral estimates for a given borrow request. Useful for UI.