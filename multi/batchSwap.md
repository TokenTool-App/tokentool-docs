# Batch exchange (Swap)

Trading on TokenTool Swap is very easy compared to most exchanges. You will not be limited by slippage, all calculations are handled optimally for you.

Video Tutorial:

### Start Trading

Before you can make a transaction, you need a wallet compatible with Web3 blockchain interaction. You can use wallet plugins like metamask. You will also need some BEP20 tokens to make transactions.


### Batch exchange transactions on TokenTool Swap

1. [Go to the redemption page here. ](https://tokentool.app/batchSwap/bsc)[https://tokentool.app/batchSwap/bsc](https://tokentool.app/batchSwap/bsc)

2. If you haven't linked your wallet yet, click Link Wallet in your upper right corner. It can also be added through [Quick Network](https://tokentool.app/other/chainList). Fast link with blockchain network link.

3. Select the token you want to trade from the position of the button part, the default selection is BNB.

![batch-swap](../.gitbook/assets/batchSwap/Snipaste_2022-12-20_18-10-40.png)

**Note: (as shown in the picture above) we call the upper token token0 and the lower token token1, no matter which token you choose, you will exchange token0 for token1. Whether you buy or sell will set the order of tokens. In case the exchange fails! **

4. As shown in the picture, select the token you want to trade. Next, enter an amount for your **token0** token by clicking on the input box. Your **token1** token amount will be estimated automatically, always remember the exchange sequence via token0=>token1.

![batch-swap](../.gitbook/assets/batchSwap/Snipaste_2022-12-20_18-43-34.png)


### Setting parameter description

![batch-swap](../.gitbook/assets/batchSwap/Snipaste_2022-12-20_20-38-38.png)

##### Gwei gas fee

So first make sure you have enough BNB to cover the transaction gas fees on the chain. Usually the gs fee will fluctuate according to the packaged transaction queue on the chain. If there are many transactions, a higher gas fee may be required to push the transaction. Learn more about [Gwei gas fees](https://academy.binance.com/en/glossary/gas) here

##### Slippage settings

It is not uncommon for tokens on the **BNB smart chain to include transaction fees** in their contracts, usually these fees can be used for burning, or entering the marketing wallet address of the project party.
Slippage will be the tolerance for the amount received in a transaction, how much tokens we can accept to lose, for example, 1USDT is converted into 0.996378....BUSD in the figure, such as the slippage setting %**50%** . It means that this transaction can tolerate the loss of **50%** tokens. If it is set to 1%, when the transaction occurs, if the number of tokens lost is greater than 1%, it will prompt the miner to roll back this time Transaction exchange operation.

##### receiving address

![batch-swap](../.gitbook/assets/batchSwap/Snipaste_2022-12-20_20-38-38.png)

You can set a fixed receiving address during the transaction exchange, and the tokens of token1 can be automatically collected to the receiving address during the batch exchange, which can save secondary collection.

##### Trading Deadline

The tolerance time for transactions to be packaged on the chain, such as a sudden surge in Gwei gas fees, your transaction may have been in the padding state on the chain and cannot be successfully packaged.

##### Run type (mode)

![batch-swap](../.gitbook/assets/batchSwap/Snipaste_2022-12-20_20-41-15.png)

**Parallel execution:** All selected addresses will initiate exchange transactions at the same time, so it often happens that all transactions are completed at the same time in one block

![batch-swap](../.gitbook/assets/batchSwap/Snipaste_2022-12-20_20-41-14.png)

**Serial execution:** All selected addresses will conduct transactions in an orderly manner, and will be executed one by one in order from top to bottom.


---

**Reminder:** If you want your token to have a correct icon logo, you can apply for an avatar logo through the [link below](https://forms.gle/ZipsociVg2KPHRLd6).

[https://forms.gle/ZipsociVg2KPHRLd6](https://forms.gle/ZipsociVg2KPHRLd6)

---


> Reference address:
>
> [https://tokentool.app/batchSwap/bsc](https://tokentool.app/batchSwap/bsc) Batch Swap exchange
>
> [https://tokentool.app/oneToMore/bsc](https://tokentool.app/oneToMore/bsc) send tokens in batches
>
> [https://tokentool.app/batchCollection/bsc](https://tokentool.app/batchCollection/bsc) Batch collection of tokens
>
> [https://tokentool.app/createWallet/bsc](https://tokentool.app/createWallet/bsc) Create wallets in batches
>
> Video Tutorials