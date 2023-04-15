# Create a [Coin Dividend] token

> **TokenTool is a blockchain toolbox that supports ETH, BSC, and other super public chains. It can create a variety of model tokens with different mechanisms, and easily solve the problem of issuing tokens. You can create your own in a few minutes Token. **


> **Click to join [TokenTool Official Communication Group](https://t.me/tokentool_app) exchange feedback**

> **It is recommended to use the computer version of Google Chrome + `Metamask` plug-in wallet for operation.**
> **Mobile phone users can also operate in `TP wallet`-discovery-enter the official website link.**


> **Video tutorial link: [https://youtu.be/CePxDWuOyd8](https://youtu.be/CePxDWuOyd8)**


### Mechanism Description

```
The distribution of tax rates mainly includes:
Marketing, backflow, destruction, currency dividends

Marketing : Deduct tokens, 'when triggered' to exchange for bonus coins -> into the marketing wallet
Return : Tokens are deducted, and the pool is automatically added when it is triggered -> this part of the administrator address can be withdrawn from the pool
Destruction: Tokens are deducted and sent directly to the black hole for destruction
Currency dividends: Deduct tokens, 'when triggered' exchange for dividends and distribute them to currency holders
```



Check out the steps below to learn how to use the Matamask wallet on the PC side to create tokens for holding dividends through TokenTool.

1. The MateMask wallet is linked to the blockchain network.
2. Open the create token link address [https://tokentool.app/createToken/v3](https://tokentool.app/createToken/v3)
3. Enter the necessary information, but before that, let's review all the important fields that need to be filled:


![Snipaste_2022-05-06_22-43-21](../.gitbook/assets/v3/Snipaste_2022-05-06_22-43-21.png)



**Currency name:** The name information of the token (such as BitCoin)

**Currency symbol:** The symbol information of the token (such as BTC)

**Initial Supply:** The total supply of tokens

**Blacklist:** The blacklist restricts buying and selling switch (after it is turned on, it can be operated on the administrator page to add certain addresses that cannot be used for `transaction`, `transfer`)

**Trading platform:** Different chains will have different trading platforms (such as `uniswap` for the ETH chain, `pancakeSwap` for the BSC chain, etc.), **After the token is created, liquidity needs to be added to the corresponding trading platform . **

**Dividend contract:** Token reward contract address, the contract address of the token you want to use to reward users. For example, if you create a BitCoin token on Binance Smart Chain and want to reward your users with DOGE, you can enter 0xba2ae424d960c26247dd6c32edc70b295c744c43 (Binance-Peg Dogecoin contract address).

**Minimum amount of holding dividends:** In order to receive rewards, each wallet must hold at least this amount of tokens to be eligible to participate in the dividend DOGE rewards.

**Marketing Wallet:** The tokens in `Marketing Tax` will be converted into red coins and sent to this address.

**Liquidity (%):** Each transaction will deduct the corresponding proportion of tokens and send them to the `contract address`, and the pool will be automatically added when the **trigger mechanism** is activated to make the pool thicker.

**Marketing (%):** Each transaction will deduct the corresponding proportion of tokens and send them to the `contract address`, which will be automatically converted into red coins when **triggers the mechanism** (depending on the dividend token you choose, If you pay dividends, you will get what you want for marketing) and send it to your marketing wallet address

**Dividend (%):** Each transaction will deduct the corresponding proportion of tokens and send them to the `contract address`, and will be automatically converted into `USDT` (depending on your dividend tokens) when the **trigger mechanism** is issued For users who hold coins and reach the `Minimum Dividend Standard`

**Destroy (%):** In each transaction, the base token will be destroyed according to the proportional amount, and transferred to `0x000000000000000000000000000000000000dead` black hole address



For example, you create a BitCoin token with the following parameters:

Token name: BitCoin

Token: BTC

Total Supply: 100,000,000 BTC

Each transaction incurs a 6% fee.

in:

2% distributed to all holders in DOGE,

  2% locked in the liquidity pool to create a steadily rising price,

2% allocated to the marketing address: `0x...000000000000000000000`.

In the image below, you can see the information to enter in the various fields.

![create token](../.gitbook/assets/v3/Snipaste_2022-05-06_23-05-37.png)



4. After entering all the necessary information, click Create Now.

5. MetaMask will now ask you to confirm the transaction. It will also show you the fee you need to pay for the transaction. If you agree, click the "Confirm" button to complete the process.

## Token administrator introduction

When the current owner (owner) has not given up the authority, he can enter the background through the token administrator page to visually modify its parameters and other information. We provide a friendly interactive page to make it easier for managers to operate contracts/modify parameters.



![token-admin](../.gitbook/assets/v3/Snipaste_2022-05-07_12-16-43.png)

1. Currency name, supply, LP address (the LP address of the current token and BNB transaction, you can click `Lock Pool` to jump to the lock pool page),
2. Number of dividend holders, showing the number of currency holders currently participating in dividends
3. **Ownership transfer:** The owner right can be transferred to a third party or other address in the future
4. **Destroy authority:** Transfer owner address to `0x0000000000000000000000000000000000000000` address
5. **Trade fee:** You can edit and modify your transaction fee (the fee is charged during swap transactions, and the transfer fee will not be charged)
6. **Minimum amount of holding dividends:** Each wallet must hold at least this amount of tokens to be eligible to participate in the dividend DOGE rewards.





![token-admin](../.gitbook/assets/v3/Snipaste_2022-05-07_12-17-00.png)

7. **Whitelist of handling fees:** Addresses added to the whitelist will not generate taxes and fees during transactions. Address Add multiple addresses in batches, one address per line. Controls can be added and removed accordingly.
8. **Buying and selling blacklist restrictions:** Addresses added to the blacklist will not be able to [transfer]/[transaction]/[buy and sell], and can be controlled according to addition and removal.
9. **Exclude eligibility for dividends:** Fixed addresses can be excluded from eligibility for dividends.
10. **Marketing address:** The address can be modified twice, and the currency that is used for dividends is also the currency that is used for marketing.
11. **Destroy:** Destroy will destroy the amount of coins and transfer them to the black hole address, and transfer them to `0x000000000000000000000000000000000000dead` address.
12. **Kill block:** Automatically kill block, input 3 means kill 3 blocks, which means that the address purchased in the first 3 blocks (bsc about 9 seconds) will automatically transfer tokens to the marketing address.
13. **Address fission:** Each transaction will automatically airdrop `little bit` tokens to a random address to achieve the effect of increasing the currency holding address



### Frequently Asked Questions

- **The tokens I created can be swapped in multiple swaps, such as `Bobing swap` `BabySwap` .. Add to the pool? **
   - Answer: When creating a token, there will be a platform choice. If you choose a swap, for example, if you choose `Bobing swap`, you need to add a pool in `Bobing swap`.


- **Can I use `USDT`, `BUSDT` or `my own sub-token` to add to the pool for the tokens of the token holding dividend mechanism I created?**
   - Answer: No, the token holding dividend template must have a BNB pool.

- **Is the code automatically open-sourced?**
- Answer: Yes, all chains with complete block browser facilities are automatically open source, including `ETH` `BSC` `ARB`...etc

- **Is the marketing into tokens or USDT?**
   - Answer: The dividend token you choose is put into the marketing wallet. If you choose `USDT`, you will get `USDT`, and if you choose `DOGE`, you will get `DOGE`.
  
- **I forgot to turn on the blacklist switch when creating tokens, can I still use the blacklist function? **
- Answer: No, if you do not turn on the blacklist function, there will be no blacklist logic code in the contract code, and the detection contract robot will not detect the blacklist switch.

- **What does the trigger mechanism mentioned above mean? **
   - Answer: When a non-whitelist address is buying or selling, the tax collected will be stored in the contract address. If there is a **sell operation**, it will trigger marketing, backflow, dividends and other mechanisms

- **I am on the BSC chain, can I create dividend XX coins, or sub-coins created by myself? **
   - Answer: As long as your XX currency has a BNB transaction pair deposit, you can get dividends. Most mainstream currencies have BNB transaction pairs, such as `USDT`, `BUSD`, `BTC`, `ETH` and so on.

- Where did the part of the LP that reflowed and automatically added to the pool go? **
   - Answer: The `LP` generated after returning to the pool is automatically issued to the `administrator wallet`.



> Referrer

> Create token address: [https://www.tokentool.app/createToken/v3](https://www.tokentool.app/createToken/v3)

> YouTube teaching video: [https://youtu.be/CePxDWuOyd8](https://youtu.be/CePxDWuOyd8)