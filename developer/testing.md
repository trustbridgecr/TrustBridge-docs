# 7.5 Local Testing (Soroban CLI)

Test contract interactions using:

```bash
soroban contract invoke \
  --network futurenet \
  --id $NEXT_PUBLIC_CONTRACT_ID \
  --source your_wallet \
  --fn deposit \
  --arg <amount>
```

✅ Ensure trustlines are set  
✅ Use Stellar Faucet for testnet tokens  
✅ Use Stellar Expert for transaction verification