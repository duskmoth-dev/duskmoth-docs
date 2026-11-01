# Private transactions on Solana

Mainnet funds are real. Begin with a small amount that meets the current withdrawal minimum after fees.

1. Prepare a deposit: `Shield 0.03 SOL`. The amount is an example, not a required amount or a fee quote.
2. Review the intent, sanctions check, token, and amount. Approve the wallet requests only if correct.
3. Wait for pool scanning, proof preparation, wallet transaction approval, confirmation, and indexing. First-time scans can take several minutes.
4. Save the deposit transaction link. Open Wallet → Show private balance.
5. Use `Withdraw 0.03 SOL to YOUR_WALLET_ADDRESS` to return funds to your own full Solana address, or substitute a recipient address.
6. Check the relayer fee, withdrawal minimum, recipient, and exact net amount. Save the withdrawal transaction link and verify both transactions independently.

Fees are deducted from the withdrawal amount. Never assume the recipient receives the gross amount.
Use Withdraw for existing private funds. `Send 0.03 SOL to RECIPIENT_ADDRESS privately` creates a new deposit first.
The “later” command deposits now; it does not schedule an automatic future transfer.
If a deposit confirmed but withdrawal failed, do not deposit again. Check transaction status and existing private balance first.

Privacy is not a guarantee of anonymity or untraceability. Funded end-to-end validation remains a separate release requirement.
