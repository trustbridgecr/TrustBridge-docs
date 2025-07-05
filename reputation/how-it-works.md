# 9.1 How TRBT is Calculated

The TrustBridge Token (TRBT) is a non-transferable, on-chain reputation system that evolves with user behavior.

## Positive Contributions:
- Successfully repaid loans
- Regular participation in lending pools
- Responsible borrowing and liquidity provisioning

## Negative Contributions:
- Loan defaults
- Missed repayment deadlines

TRBT is updated automatically by the `update_trbt_score` function after key events.

> The higher your TRBT score, the more trusted you become on-chain.