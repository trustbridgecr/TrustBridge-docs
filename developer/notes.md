# 7.6 Developer Notes

- 🧪 TrustBridge uses **Husky** to enforce linting and formatting on every commit.
- 🚨 Pushes are blocked if errors exist.

Check before pushing:
```bash
npm run lint
npm run format
```

- 💡 Backstop logic is handled automatically at protocol level.
- 🧾 No escrows or milestone flows: liquidity is direct and permissionless.
- 👥 User roles (borrower/lender) are inferred from wallet activity.
- 🔎 All contract data is visible on-chain via Stellar Explorer.