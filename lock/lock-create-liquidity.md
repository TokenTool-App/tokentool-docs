# Create a liquidity lock pool



Teaching video: Add liquidity, lock pool, unlock and other operations [https://youtu.be/Dqb9qL22YwU](https://youtu.be/Dqb9qL22YwU)



Navigate to [https://tokentool.app/lock/create](https://tokentool.app/lock/create) and follow this simple procedure:

1. Link your wallet.
2. Go to [https://tokentool.app/lock/create](https://tokentool.app/lock/create)
3. After entering your liquidity token contract address, your token pool information and balance will be displayed (as shown in the figure TTT-WBNB transaction pair, exchange, balance and other information).
     **tips: If you don’t know the LP address of your token, you can find the LP address through [How to Query LP Address](https://docs.tokentool.app/common-problem/how-to-find-liquidity). **

![lock-token](../.gitbook/assets/lock/Snipaste_2022-05-08_23-15-41.png)

4. Enter the amount of pool balance you want to lock, and select the time to lock until unlocked at a certain point in time

![lock-token](../.gitbook/assets/lock/Snipaste_2022-11-25_22-41-21.png)


5. Click Authorize to approve
5. MetaMask will now ask you to confirm the transaction. If you agree, click the "Confirm" button to complete the process.
6. After completing the authorization, click the lock button, MetaMask will now ask you to confirm the transaction.

![lock-token](../.gitbook/assets/lock/Snipaste_2022-11-25_22-44-12.png)

7. Click "Lock"

![lock-token](../.gitbook/assets/lock/Snipaste_2022-11-25_22-45-13.png)


8. MetaMask will now ask you to confirm the transaction. It will also show the fee you need to pay for the transaction. If you agree, then click the "Confirm" button to complete the "Lock" process.

![lock-token](../.gitbook/assets/lock/Snipaste_2022-11-25_22-49-25.png)


be careful:

If your token contract has LP dividends, or holds LP rewards and other mechanisms, it must be dismantled.

Please exclude the lock contract address of TokenToolLock, you can see the lock contract address of TokenToolLock in the yellow prompt.