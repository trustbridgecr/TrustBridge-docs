# 7.4 Smart Contract Integration

TrustBridge uses the Blend v2 smart contract suite via Soroban SDK.

### Key Contracts:
- `BlendPool` — pool logic, lending ratio, interest computation
- `RiskModule` — detects unhealthy pools, triggers freeze
- `BackstopModule` — manages the insurance fund
- `BorrowerActions` — borrower flows (request, repay)
- `LenderActions` — funding, balance tracking

Use the Soroban CLI to simulate contract calls and test locally.

💡 You can get free XLM from the Stellar Testnet Faucet.