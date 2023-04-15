# Create a [Pool Dividend] token

> **TokenTool is a blockchain toolbox that supports ETH, BSC, and other super public chains. It can create a variety of model tokens with different mechanisms, and easily solve the problem of issuing tokens. You can create your own in a few minutes Token. **


> **Click to join [TokenTool Official Communication Group](https://t.me/tokentool_app) exchange feedback**

> **It is recommended to use the computer version of Google Chrome + `Metamask` plug-in wallet for operation.**
> **Mobile phone users can also operate in `TP wallet`-discovery-enter the official website link.**




### Mechanism Description

```
The distribution of tax rates mainly includes:
Marketing, reflow, destruction, adding pool dividends

Marketing : Tokens are deducted, exchanged for pot coins at 'trigger' -> into the marketing wallet
Return : Tokens are deducted, and the pool is automatically added when it is triggered -> this part of the administrator address can be withdrawn from the pool
Destruction: Tokens are deducted and sent directly to the black hole for destruction
Adding pool dividends: Deduct tokens, 'when triggered' exchange dividend coins for pool adding users
```



Check out the steps below to learn how to use the Matamask wallet on the PC side to create tokens for holding dividends through TokenTool.

1. The MateMask wallet is linked to the blockchain network.
2. Open the create token link address [https://tokentool.app/createToken/v4](https://tokentool.app/createToken/v4)
3. Enter the necessary information, but before that, let's review all the important fields that need to be filled:


![Snipaste_2022-05-06_22-43-21](../.gitbook/assets/v4/create-token-v4.png)



**Currency name:** The name information of the token (such as BitCoin)

**Currency symbol:** The symbol information of the token (such as BTC)

**Initial Supply:** The total supply of tokens

**Accuracy:** The number of digits of precision of the token (the precision is the number of decimal places representing the currency `for example: 0.000001` means that there are 6 digits of precision)

**Blacklist:** The blacklist restricts buying and selling switch (after it is turned on, it can be operated on the administrator page to add certain addresses that cannot be used for `transaction`, `transfer`)

**Trading platform:** Different chains will have different trading platforms (such as `uniswap` for the ETH chain, `pancakeSwap` for the BSC chain, etc.), **After the token is created, liquidity needs to be added to the corresponding trading platform . **

**Custom trading pair:** By default, BNB trading pair is used to create tokens. By customizing the trading pair switch, you can enter USDT, BUSD and other contract addresses to combine trading pair information

**Add pool dividend contract:** The address reward contract for adding pool can use mainstream currencies such as `USDT`, `DOGE`, `SHIB`, or you can use local currency dividends.


**Marketing Wallet:** The tokens of `Marketing Tax` will be converted into pot currency `BNB` or `USDT` (depending on your pool trading pair) and sent to this address.

**Liquidity (%):** Each transaction will deduct the corresponding proportion of tokens and send them to the `contract address`, and the pool will be automatically added when the **trigger mechanism** is activated to make the pool thicker.

**Marketing (%):** Each transaction will deduct a corresponding proportion of tokens and send them to the `contract address`, which will be automatically converted into pot coins when **triggers the mechanism** (depending on what pot you use, What currency does marketing) send to your marketing wallet address

**Dividend (%):** Each transaction will deduct the corresponding proportion of tokens and send them to the `contract address`, which will be automatically converted into `USDT` when **triggers the mechanism** (depending on the dividend token you choose) Issued to the address of the user who added the pool

**Destroy (%):** In each transaction, the base token will be destroyed according to the proportional amount, and transferred to `0x000000000000000000000000000000000000dead` black hole address




## Token administrator introduction

When the current owner (owner) has not given up the authority, he can enter the background through the token administrator page to visually modify its parameters and other information. We provide a friendly interactive page to make it easier for managers to operate contracts/modify parameters.



![token-admin](../.gitbook/assets/v4/token-admin-1.jpeg)

1. **Full name of currency:** Full name of token
2. **LP address: ** Display the contract address of the pool LP, you can click the `Lock Pool` button to jump to the lock pool page
3. **Contract address: ** Display the current token contract address
4. **Ownership transfer:** The owner authority can be transferred to a third party or other address in the future
5. **Destroy authority:** Transfer owner address to `0x0000000000000000000000000000000000000000` address
6. **Trade Fee:** You can edit and modify your transaction fee (the fee is charged during the swap transaction, and the transfer fee will not be charged)
7. **Add pool handling fee:** The handling fee charged by the user when adding the pool (a part of the handling fee is collected as `dividend`)
8. **Withdrawal pool handling fee:** The handling fee charged by the user when withdrawing from the pool (a part of the handling fee is collected as `dividend`)
9. **Kill block:** Automatically kill block, input 3 means kill 3 blocks, which means that the address purchased in the first 3 blocks (bsc about 9 seconds) will automatically transfer tokens to the marketing address.
10. **Address fission:** Each transaction will automatically airdrop `little bit` tokens to a random address to achieve the effect of increasing the currency holding address





![token-admin](../.gitbook/assets/v4/token-admin-2.jpeg)

7. **Whitelist of handling fees:** Addresses added to the whitelist will not generate taxes and fees during transactions. Address Add multiple addresses in batches, one address per line. Controls can be added and removed accordingly.

8. **Buying and selling blacklist restrictions:** Addresses added to the blacklist will not be able to [transfer]/[transaction]/[buy and sell], and can be controlled according to addition and removal.

9. **Single maximum transfer amount:** purchase limit/transfer limit (ordinary users cannot exceed the single maximum transfer amount when buying or selling/transfer)

10. **Wallet maximum holding limit:** The number of an address cannot exceed (wallet maximum holding limit)

11. **Whitelist of position limit:** If position limit is set, the maximum number of wallets will be limited for all addresses. If you want to lift the limit, you will be able to join the white list

12. **White list of transfer/buying and selling restrictions:** If transfer restrictions are set, users will be restricted when trading, and if they join the white list, they will not be restricted

13. **Minimum dividend/dividend interval:**

     1. **Minimum dividend:** Refers to when the balance in the dividend pool is greater than the dividend, for example (dividend `USDT`, fill in the minimum amount of 10, and the dividend will not start until the USDT in the contract address reaches 10U).
     2. **Dividend interval:** After queuing up for dividends last time, how long will it take to start the next round of dividends.
     3. **Reminder: The minimum amount and dividend interval can be modified to increase the dividend speed. **

14. **Pooling dividend contract:** You can modify the dividend contract. To modify the dividend contract address, you need to pay attention to the conditions of the dividend contract. You can check the answers to the following FAQs.

15. **Marketing address:** The address can be modified twice, and the transaction pair used in the pot is also the currency for marketing.

16. **Destroy:** Destroy will destroy the amount of coins and transfer them to the black hole address, and transfer them to `0x000000000000000000000000000000000000dead` address.

    



### Frequently Asked Questions

- What currency can be distributed for dividends? **
   - Answer: Dividends can be distributed between the local currency and other currencies, and there are no conditions for the local currency.
   - Other currencies: It is mainly related to your trading pair in the pot. For example, if you use `USDT` as the trading pair pool, you can directly distribute the trading pair currency **`USDT`** and **have a trading pair with USDT Coins** such as `BTC`, `DOGE`, `SHIB` and other mainstream currencies.

- **Can I get dividends in BNB? **
   - Answer: Yes, you can use the `BNB` trading pair, and the dividend contract can be `WBNB`** (direct dividend trading pair WBNB)**.
   - Or you can use `USDT` trading pair, the dividend contract can also be `WBNB` **(WBNB has a trading pair with USDT)**

- **Adding pool is set to 0%, why do users still charge tax when adding pool? **
   - Answer: When adding a pool on the swap page, **Must be the transaction pair on the top, such as (USDT)**, and add the current currency to the pool below.
   - If it is a BNB trading pair, **users must first convert BNB to WBNB** at 1:1, and then add the pool, with WBNB on the top and the current currency on the bottom.
- **What is the concept of the dividend pool mentioned in the above description? **
   - Answer: When buying and selling from non-whitelist addresses, a handling fee will be charged, and the handling fee will **trigger the exchange mechanism** when selling, such as dividends** `USDT`**, the tax of the dividend part will be converted into the contract according to the dividend contract In the address, the `USDT` in the contract address is greater than **`minimum dividend number`** and when the interval between the last dividend and this dividend is met, the dividend mechanism will be triggered and the added pool address will start to distribute dividends.
- **Is the dividend distributed to all those who add to the pool at one time? **
   - Answer: No, queuing up for dividends, every time the dividend is triggered (the above conditions are met), about 7 to 10 addresses will be queued for dividends, and when the dividend reaches the last address, it will start to cycle from the first address again.
- **The tokens I created can be swapped in multiple swaps, such as `Bobing swap` `BabySwap` .. Add to the pool? **
   - Answer: When creating a token, there will be a platform choice. What swap you choose (for example, you choose `Bobing swap`), you must add a pool to `Bobing swap`.


- **Can the tokens I created with the pool bonus dividend mechanism be added to the pool with `USDT`, `BUSD` or `my own sub-token`?**
   - Answer: According to the transaction pair you use when you create it, if you don’t customize it, the default is to use the chain’s native currency BSC chain is `BNB`, Ethereum is `ETH` currency, what currency is the custom transaction pair to add to the pool also need to use your own The currency at the time of definition is added to the pool.

- **Is the code automatically open-sourced?**
   - Answer: Yes, all chains with complete block browser facilities are automatically open source, including `ETH` `BSC` `ARB`...etc

- **Is the marketing into tokens or USDT?**
   - Answer: The marketing wallet depends on your trading pair. The default trading pair you created is BNB, and the custom trading pair is the currency when you customize it, for example (custom `USDT`, etc.).

- **I forgot to turn on the blacklist switch when creating tokens, can I still use the blacklist function? **
   - Answer: No, if you do not turn on the blacklist function, there will be no blacklist logic code in the contract code, and the detection contract robot will not detect the blacklist switch.

- **What does the trigger mechanism mentioned above mean? **
   - Answer: When a non-whitelist address is buying or selling, the tax collected will be stored in the contract address. If there is a **sell operation**, it will trigger marketing, backflow, dividends and other mechanisms

- **I am on the BSC chain, can I create dividend XX coins, or sub-coins created by myself? **
   - Answer: As long as your XX currency has a BNB transaction pair deposit, you can get dividends. Most mainstream currencies have BNB transaction pairs, such as `USDT`, `BUSD`, `BTC`, `ETH` and so on.

- Where did the part of the LP that reflowed and automatically added to the pool go? **
   - Answer: The `LP` generated after returning to the pool is automatically distributed to the `Marketing Wallet`.
- **Why didn't they receive dividends after I used the batch transfer tool to distribute LP to retail investors?**

   - Answer: The form of direct transfer of LP will not include the address of receiving LP in the dividend list. Directly `receiving LP transfer` instead of obtaining the address of LP through `adding pool` operation, you need to `sell a sum` or `return Only by adding to the pool once can you enjoy LP dividends