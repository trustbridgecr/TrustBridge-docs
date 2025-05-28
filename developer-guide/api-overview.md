# API Overview – TrustBridge Integration with Trustless Work

This page describes how each API endpoint from Trustless Work is used within the TrustBridge platform and which roles are allowed to invoke them.

---

## 🧩 Core Functions

### `initializeEscrow`

**Role:** _Lender or Platform_  
Initializes a new escrow contract with full loan metadata including borrower, amount, duration, milestones, approvers, dispute resolver, and more.

---

### `fundEscrow`

**Role:** _Lender_  
Transfers loan funds into the escrow contract after initialization.

---

### `getEscrow`

**Role:** _Lender, Borrower, Platform_  
Retrieves escrow details by ID, including participants, milestones, status, and balances.

---

### `resolveDispute`

**Role:** _Dispute Resolver_  
Handles a dispute resolution process and determines fund distribution once a conflict arises.

---

### `changeMilestoneStatus`

**Role:** _Approver or Borrower (for self-managed flows)_  
Updates the status of a specific milestone (e.g., `approved`, `rejected`, `completed`).

---

### `changeMilestoneFlag`

**Role:** _Borrower_  
Flags a milestone as completed or in progress. May trigger further approval or fund release.

---

### `startDispute`

**Role:** _Borrower or Lender_  
Triggers a dispute when either party believes the escrow agreement is not being fulfilled.

---

### `releaseFunds`

**Role:** _Approver or Escrow Automation_  
Releases milestone funds to the borrower when conditions are met and verified.

---

### `updateEscrow`

**Role:** _Platform_  
Updates non-critical metadata fields like notes, deadline extensions, or administrative adjustments.

---

## 🔧 Helper Functions

### `setTrustline`

**Role:** _Borrower or Lender_  
Allows the escrow contract to hold or transfer assets on the Stellar network by setting trustlines.

---

### `sendTransaction`

**Role:** _Platform or Internal_  
Broadcasts signed Stellar transactions. Used for custom flows or complex operations.

---

### `getMultiple`

**Role:** _All roles_  
Fetches multiple escrows or milestones in batch mode, typically used in dashboards or analytics.

---

Use this guide to understand role-based access and correct usage of each API function within the TrustBridge platform.
