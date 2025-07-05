# 6.3 Role-based Access Summary

| Function           | Borrower | Lender | Protocol | Platform |
|--------------------|----------|--------|----------|----------|
| init_pool          | ❌       | ❌     | ❌       | ✅       |
| deposit            | ❌       | ✅     | ❌       | ❌       |
| borrow             | ✅       | ❌     | ❌       | ❌       |
| repay              | ✅       | ❌     | ❌       | ❌       |
| withdraw           | ❌       | ✅     | ❌       | ❌       |
| freeze_pool        | ❌       | ❌     | ✅       | ❌       |
| get_pool_info      | ✅       | ✅     | ✅       | ✅       |
| get_user_position  | ✅       | ✅     | ✅       | ✅       |
| update_trbt_score  | ❌       | ❌     | ✅       | ❌       |
| simulate_loan      | ✅       | ✅     | ✅       | ✅       |