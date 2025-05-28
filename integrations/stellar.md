# Stellar Integration

TrustBridge uses the Stellar blockchain to manage escrow funds, handle asset transfers, and provide a secure, decentralized financial layer for loan agreements.

## 🌐 Why Stellar?

Stellar offers the perfect foundation for microloans and decentralized finance due to its:

- Low transaction fees
- Fast settlement times
- Native support for multi-signature accounts
- Custom assets and trustlines
- Growing ecosystem with wallet and DApp support

---

## 🔧 Key Stellar Concepts Used

### 🔐 Wallets

TrustBridge supports wallet connections using:

- **Freighter**
- **xBull**
- **Albedo**
- **LOBSTR**

Users must ensure their wallets are set to **Testnet** or **Mainnet** based on the environment.

### 🔗 Trustlines

Before receiving any asset (e.g., USDC), a user must set a **trustline** with the specific asset issuer. This is done via the API endpoint `/helper/set-trustline`.

### 💵 Custom Assets

Escrows in TrustBridge hold and release tokenized assets like USDC or XLM. These assets are created and distributed within the Stellar network.

### 📜 Smart Contracts (Soroban)

TrustBridge leverages Soroban smart contracts (via Trustless Work) to define escrow logic, milestone tracking, and dispute resolution.

---

## 📥 Receiving Funds

Funds are released to the borrower wallet when a milestone is approved. These transfers occur directly on Stellar using signed transactions via `sendTransaction`.

---

## 🛡️ Security

- Escrows are governed by multi-signature rules.
- All critical operations require user signatures.
- Assets are non-custodial and verifiable on-chain.

---

Next: [Credits & Contributions](credits.md)
