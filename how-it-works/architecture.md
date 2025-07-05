# 2.3 System Architecture

TrustBridge is built on Blend v2 over the Stellar blockchain. It enables isolated, programmable, and risk-managed lending pools.

## Core Components

### Isolated Lending Pools
- Each pool is independent
- Risk is contained per pool

### Backstop Reserve
- Formed by 20% of lender deposits and 100% of borrower collateral
- Covers shortfalls on defaults

### Collateralized Loans
- Borrowers must deposit XLM before receiving USDC
- Collateral is locked and used for liquidation if needed

### Risk Engine (Blend-native)
- Monitors pool health, repayment rate, utilization
- Freezes pool if thresholds are crossed

### TRBT Token (Reputation)
- Non-transferable score based on behavior
- Used to gate access to higher-quality pools