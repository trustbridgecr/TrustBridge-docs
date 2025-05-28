# Borrower Guide

This guide explains how borrowers can request loans and manage their escrow contracts through TrustBridge.

## Step 1: Connect Your Wallet

- Open the TrustBridge app and connect a Stellar-compatible wallet (e.g., Freighter, xBull).
- Ensure your wallet has a trustline for the desired asset (e.g., USDC).

## Step 2: Submit a Loan Request

- Navigate to “Request a Loan”.
- Fill in:
  - Loan amount
  - Purpose
  - Number and description of milestones
  - Duration and deadline
  - Asset to receive

## Step 3: Await Offers

- Your loan request will be listed publicly.
- Lenders may review and send offers with custom terms.
- You can review and accept any offer that suits you.

## Step 4: Escrow Creation

- Once you accept an offer, an escrow contract is initialized by the lender.
- Wait for the lender to fund the escrow.

## Step 5: Work on Milestones

- Complete the task or goal defined for each milestone.
- Mark each milestone as ready (`changeMilestoneFlag`).
- Wait for approval to trigger fund release.

## Step 6: Receive Funds

- Upon milestone approval, funds are released automatically to your wallet.

## Step 7: Handle Disputes (if needed)

- If you believe the lender is unfairly rejecting a milestone, initiate a dispute (`startDispute`).
- A resolver will handle the case through `resolveDispute`.

## Best Practices

- Be specific and realistic with milestone planning.
- Keep communication clear and timely with the lender.
- Follow up on approvals to ensure smooth disbursements.

---

Next: [Offer a Loan](lender-guide.md)
