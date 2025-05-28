# Lender Guide

This guide walks lenders through the process of reviewing loan requests, making offers, and managing escrows on TrustBridge.

## Step 1: Connect Your Wallet

- Open the TrustBridge app and connect your Stellar wallet.
- Ensure you have a sufficient balance in the asset you want to lend (e.g., USDC or XLM).

## Step 2: Browse Loan Requests

- Navigate to the loan marketplace.
- View detailed proposals from borrowers including:
  - Requested amount
  - Purpose
  - Milestones
  - Timeline

## Step 3: Make a Loan Offer

- Click on a request to create a custom loan offer.
- Define:
  - Interest rate (optional)
  - Any additional conditions or fees
  - Preferred asset

## Step 4: Wait for Acceptance

- The borrower may review and accept your offer.
- You’ll be notified if your offer is chosen.

## Step 5: Fund the Escrow

- Once accepted, call `fundEscrow` to deposit funds into the escrow contract.
- The escrow is now active and milestone tracking begins.

## Step 6: Monitor Milestones

- Borrowers will mark milestones as complete.
- As the lender or assigned approver, you may:
  - Review submissions
  - Approve or reject milestones using `changeMilestoneStatus`

## Step 7: Dispute Handling (if needed)

- If you suspect fraud or incomplete work, initiate a dispute.
- A resolver will step in via `resolveDispute`.

## Completion & Repayment

- TrustBridge currently handles repayments off-chain.
- You can coordinate directly with the borrower or via integrated tools (if available).

---

Next: [Dashboard](dashboard.md)
