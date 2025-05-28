# ⚙️ Getting Started

Follow the steps below to get started with this project:

## 📦 Installation

Install dependencies:

```bash
npm i
```

Format the code using Prettier:

```bash
npx prettier --write .
```

Start the development server:

```bash
npm run dev
```

## 🔐 Environment Variables

Create a `.env` file in the root of the project with the following:

```env
# Firebase configuration
NEXT_PUBLIC_FIREBASE_API_KEY=YOUR_API_KEY
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=YOUR_AUTH_DOMAIN
NEXT_PUBLIC_FIREBASE_PROJECT_ID=YOUR_PROJECT_ID
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=YOUR_STORAGE_BUCKET
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=YOUR_MESSAGING_SENDER_ID
NEXT_PUBLIC_FIREBASE_APP_ID=YOUR_APP_ID

# Trustless Work API
NEXT_PUBLIC_API_KEY=YOUR_API_KEY
```

> 🎥 API Key Video: _dApp Trustless Work_
> 🎥 Firebase Video: _Firebase_

## 🔥 Firebase Setup

Once you have your Firebase database ready, add the following document in the `trustlines` collection:

```json
{
  "name": "USDC",
  "trustline": "GBBD47IF6LWK7P7MDEVSCWR7DPUWV3NY3DTQEVFL4NAT4AQH3ZLLFLA5",
  "trustlineDecimals": 10000000
}
```

## 🔑 Wallet Requirements

To use this platform, install one of the following wallets:

- Freighter
- Albedo
- xBull
- LOBSTR

> **Wallet Usage Note:** Ensure your wallet is set to **test net**. If you see "Not Available" in Freighter:

1. Go to **Security > Manage Connected Wallets**
2. Remove **localhost**
3. Reload and reconnect

If problems persist, contact support.

## 🧠 IMPORTANT NOTE (Husky Setup)

We use Husky to ensure code formatting and linting on git push. If `npm run format` or `npm run lint` fail, your push will be blocked.

Fix any errors before retrying your push.
