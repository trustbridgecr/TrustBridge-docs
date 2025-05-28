# Architecture

The TrustBridge architecture is built around a decentralized loan system powered by the Stellar blockchain and Trustless Work APIs. It combines smart escrow logic, wallet-to-wallet transactions, and milestone-based loan delivery.

## Components

### 1. Frontend (Next.js)

- User interface for lenders and borrowers.
- Interacts with wallet providers (Freighter, xBull).
- Displays loan offers, escrow details, and milestone progress.

### 2. Backend/API

- Handles communication with Trustless Work and Stellar.
- Stores metadata in Firebase (e.g., user profiles, loan history).
- Secures operations like creating offers, funding escrows, and dispute logic.

### 3. Trustless Work API

- Manages escrow deployment, milestone tracking, and dispute resolution.
- Decentralized logic with built-in role separation (approver, resolver, etc.).

### 4. Stellar Blockchain

- Asset and escrow contract settlement layer.
- Handles trustlines, XLM/USDC transfer, and multisig logic.

### 5. Firebase (Firestore)

- Stores non-sensitive app data (loan metadata, user actions).
- Syncs with frontend for real-time updates.

## Visual Diagram (Text)

```
[ User Wallet ]
     ↓
[ TrustBridge Frontend (Next.js) ]
     ↓
[ API + Firebase ] <--> [ Trustless Work API ]
     ↓
[ Stellar Escrow Contract ]
```

## Security & Trust Model

- Escrows are non-custodial and controlled by role-based multisig logic.
- All sensitive operations require wallet signatures.
- Disputes and releases are verifiable on-chain.

---

Next: [Loan Flow](loan-flow.md)
