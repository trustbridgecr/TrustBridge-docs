# 10.2 Soroban CLI Commands

Test interactions with Blend contracts using Soroban CLI:

### Deposit Example
```bash
soroban contract invoke \
  --network futurenet \
  --id $NEXT_PUBLIC_CONTRACT_ID \
  --source your_wallet \
  --fn deposit \
  --arg <amount>
```

### Tips:
- Ensure you have set trustlines
- Use Stellar Testnet Faucet for tokens
- Use Stellar Expert for transaction validation