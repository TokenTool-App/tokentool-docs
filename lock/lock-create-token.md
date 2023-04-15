# create ERC20 token lock

## What is a token lock?

Token Locking allows DeFi projects to set custom token locking parameters.

By using TokenToolLocks to lock team members' tokens and treasury, projects can instill trust in their communities and show they are engaged for the long term. Time-locked tokens cannot be released until the lock expires, so investors can be confident that the team won't dump all their tokens on the market (aka "exit scam").



## Why is token lock important?

**Projects can lock a percentage of the pre-mined token supply or team-owned tokens into our time-locked decentralized smart contract vault. **

Projects cannot access tokens until the lock-up period expires. In this way, the community and investors can rest assured that the tokens will not be dumped by the team during the contract period, the so-called exit scam.

This is a huge innovation compared to most token offerings, where projects may avoid fulfilling their promises and sell all their tokens in bad faith, leaving holders, stakers and investors The price of the tokens of the latter is close to $0.



## How do I create my token lock?

Navigate to [https://tokentool.app/lock/create](https://tokentool.app/lock/create) and follow this simple procedure:

1. Link your wallet.
2. Go to [https://tokentool.app/lock/create](https://tokentool.app/lock/create)
3. After entering your token contract address, your token information and token balance will be displayed.
4. Enter the amount of token token balance you want to lock and select Lock until a certain point in time to unlock the token time

The following example: lock all token balances until unlocked at 2025-01-01 00:00:00.

![lock-token](../.gitbook/assets/lock/Snipaste_2022-05-08_23-15-40.png)

5. Click Authorize, MetaMask will now ask you to confirm the transaction. If you agree, click the "Confirm" button to complete the process.
6. After completing the authorization, click the lock button, MetaMask will now ask you to confirm the transaction.



be careful:

If your token contract has mechanisms such as dividends for holding coins, or rewards for holding coins, transfer limits, etc., there must be an operation to remove and exclude restrictions.

Please exclude the lock contract address of TokenToolLock, you can see the lock contract address of TokenToolLock in the yellow prompt.