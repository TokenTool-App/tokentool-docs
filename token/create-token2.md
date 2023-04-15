# Create a [Double Marketing Reflow] token

> **TokenTool is a blockchain toolbox that supports ETH, BSC, and other super public chains. It can create a variety of model tokens with different mechanisms, and easily solve the problem of issuing tokens. You can create your own in a few minutes Token. **


> **Click to join [TokenTool Official Communication Group](https://t.me/tokentool_app) exchange feedback**

> **It is recommended to use the computer version of Google Chrome + `Metamask` plug-in wallet for operation.**
> **Mobile phone users can also operate in `TP wallet`-discovery-enter the official website link.**


> **Video tutorial link: [https://youtu.be/zPVY_oZH5qo](https://youtu.be/zPVY_oZH5qo)**


### Mechanism Description

```
The distribution of tax rates mainly includes:
marketing, team, reflow, destroy

Marketing: Deduct tokens, 'when triggered' exchange for BNB or USDT (depending on what pool you add) -> into the marketing wallet
Team: Deduct tokens, exchange BNB or USDT 'when triggered' (depending on what pool you add) -> into the team wallet (can be understood as the second marketing address)
Return : Tokens are deducted, and the pool is automatically added when it is triggered -> this part of the administrator address can be withdrawn from the pool
Destruction: Tokens are deducted and sent directly to the black hole for destruction
```



## Create a token with [Double Marketing Reflow]

Check out the steps below to learn how to use MetaMask to create a token with buy and sell rates through TokenTool.

1. First, we create tokens through the visual interface, and open the function of creating tokens through [https://www.tokentool.app/createToken/v2](https://www.tokentool.app/createToken/v2). Fill in the token currency information.

![create token ](../.gitbook/assets/v2/Snipaste_2022-05-03_14-39-31.png)

2. Parameter introduction

**Currency name:** The name information of the token (such as BitCoin)

**Currency symbol:** The symbol information of the token (such as BTC)

**Initial supply:** The total supply of tokens (when the precision is 18 digits, the total supply can be followed by 15 0s, when the precision is 17 digits, the total supply can be followed by 16 0s, and so on.. )

**Accuracy:** The number of digits of precision of the token (the precision is the number of decimal places representing the currency `for example: 0.000001` means that there are 6 digits of precision)

**Blacklist:** The blacklist restricts buying and selling switch (after it is turned on, it can be operated on the administrator page to add certain addresses that cannot be used for `transaction`, `transfer`)

**Custom trading pair:** By default, BNB trading pair is used to create tokens. By customizing the trading pair switch, you can enter USDT, BUSD and other contract addresses to combine trading pair information


**Trading platform:** Different chains will have different trading platforms (such as `uniswap` for the ETH chain, `pancakeSwap` for the BSC chain, etc.), **After the token is created, liquidity needs to be added to the corresponding trading platform . **

**Creator/Owner:** The creator/owner of this token, the owner administrator, only the administrator can enter the administrator background to modify the handling fee parameters and other operations

**Team address:** The fee for the address allocated to the team according to the fee ratio

**Marketing address:** The fee allocated to the marketing address according to the handling fee ratio (similar to 2 marketing addresses, if not, you can fill in the same)

**Purchasing fee:** The handling fee charged when the user makes a purchase through swap ( **The following handling fee is the default value, if you need to modify it, you can enter the administrator page to modify the ratio** )

**Sell handling fee:** The handling fee charged when the user sells through swap ( **The following handling fee is the default value, if you need to modify it, you can enter the administrator page to modify the ratio** )

**Return Proportion Allocation:** (Secondary allocation based on the received handling fee)

​ **Liquidity:** The proportion of handling fees is added to the liquidity.

​ **Marketing:** The proportion of handling fees is exchanged into BNB and returned to the marketing address

​ **Team:** The proportion of handling fees is converted into BNB and returned to the team address

## Token Manager

Check out the steps below to learn how to use MetaMask to access the Token Admin page through TokenTool.

![create token](../.gitbook/assets/v2/admin2.png)

1. Admin wallet link MetaMask wallet link
2. Enter the contract address of the token in the Token administrator page to enter the administrator page

![create token](../.gitbook/assets/v2/admin1.png)

1. **Ownership transfer:** The owner right can be transferred to a third party or other address in the future
2. **Destroy authority:** Transfer owner address to `0x0000000000000000000000000000000000000000` address
3. **Buying and selling fees:** You can edit and modify your transaction fees (handling fees are charged during swap transactions, and no handling fees will be charged for transfers)
4. **Backflow switch:** The transaction fee collected by the user in the swap will be stored in the current contract, and the `minimum amount of backflow` has been reached to trigger the backflow mechanism
5. **Backflow ratio:** According to the backflow ratio, backflow to each position
    1. Liquidity representatives enter the pool
    2. Marketing representative transfers to marketing address
    3. The team representative transfers to the team address
6. **Maximum single transfer amount:** purchase limit/transfer limit (ordinary users cannot exceed the single maximum transfer amount when buying or selling/transfer)

![create token](../.gitbook/assets/v2/admin3.png)

1. **Wallet maximum holding limit:** The number of an address cannot exceed (wallet maximum holding limit)

2. **Handling fee white list:** Fixed addresses can be added to the white list to make them free of handling fees when conducting transactions. Only one address can be added at a time, and there is no upper limit for adding multiple addresses

3. **Whitelist of position limit:** If position limit is set, the maximum number of wallets will be limited for all addresses. If you want to lift the limit, you will be able to join the white list

4. **White list of transfer restrictions:** If transfer restrictions are set, users will be restricted when trading, and if they are added to the white list, they will not be restricted

5. **Blacklist restrictions:** When the user address is added to the blacklist, the user will not be able to `transfer` `transaction` operations

6. **Marketing/Team Address:** The address can be edited twice

7. **Maximum amount of destruction:** If the currency has a destruction mechanism during the transaction, you can set the amount of destruction that will not be destroyed

8. **Destroy amount:** Transfer the balance in your wallet to the black hole address `0x0000000000000000000000000000000000000dEaD`

9. **Kill block:** Automatically kill block, input 3 means kill 3 blocks, which means that the address purchased in the first 3 blocks (bsc about 9 seconds) will automatically transfer tokens to the marketing address.

10. **Address fission:** Each transaction will automatically airdrop `little bit` tokens to a random address to achieve the effect of increasing the currency holding address


### Frequently Asked Questions
- **The tokens I created can be swapped in multiple swaps, such as `Bobing swap` `BabySwap` .. Add to the pool? **
   - Answer: When creating a token, there will be a platform choice. If you choose a swap, for example, if you choose `Bobing swap`, you need to add a pool in `Bobing swap`.

- **Is the code automatically open-sourced?**
- Answer: Yes, all chains with complete block browser facilities are automatically open source, including `ETH` `BSC` `ARB`...etc

- **Is the marketing/team address into tokens or USDT?**
   - Answer: The entry into the marketing wallet depends on your trading pair. To create a token, the chain currency is used by default (BSC chain uses BNB to add the pool by default). The marketing entry is BNB. If the custom trading pair uses `USDT` , then the marketing input is USDT.
  
- **I forgot to turn on the blacklist switch when creating tokens, can I still use the blacklist function? **
- Answer: No, if you do not turn on the blacklist function, there will be no blacklist logic code in the contract code, and the detection contract robot will not detect the blacklist switch.

- **What does the trigger mechanism mentioned above mean? **
   - Answer: When a non-whitelist address is buying or selling, the tax collected will be stored in the contract address. If there is a **sell operation**, it will trigger marketing, backflow, dividends and other mechanisms

- Where did the part of the LP that reflowed and automatically added to the pool go? **
   - Answer: The `LP` generated after returning to the pool is automatically issued to the `administrator wallet`.

- **Can I use my home currency as my trading pair? **
   - Answer: Yes, when creating tokens, turn on the custom trading pair switch, enter your mother currency contract, and you can use your mother currency to add the pool when adding liquidity.



> Referrer

> Create token address: [https://www.tokentool.app/createToken/v2](https://www.tokentool.app/createToken/v2)

> YouTube teaching video: [https://youtu.be/zPVY_oZH5qo](https://youtu.be/zPVY_oZH5qo)