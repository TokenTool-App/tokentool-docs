# Create a token with [additional issuance, false authority, backflow of local currency]

> **TokenTool is a blockchain toolbox that supports ETH, BSC, and other super public chains. It can create a variety of model tokens with different mechanisms, and easily solve the problem of issuing tokens. You can create your own in a few minutes Token. **


> **Click to join [TokenTool Official Communication Group](https://t.me/tokentool_app) exchange feedback**

> **It is recommended to use the computer version of Google Chrome + `Metamask` plug-in wallet for operation.**
> **Mobile phone users can also operate in `TP wallet`-discovery-enter the official website link.**


> **Video tutorial link: [https://youtu.be/K0PExlXV0LI](https://youtu.be/K0PExlXV0LI)**


### Mechanism Description

```

Tax rate distribution marketing: deduction of tokens, local currency directly into -> into the marketing wallet
Suspension of transactions: all addresses will not be able to transfer money, transaction operations
Coinable: The administrator can issue additional tokens.
Temporarily discard permissions: You can temporarily discard permissions and retrieve them after a fixed period of time

```
> **⚠️Note: The tokens created in this version will be detected by the contract detection robot for dangerous switches and other information. **



## Token basic information

First, we create tokens through the visual interface, and open the token creation function through [https://www.tokentool.app/createToken/eth](https://www.tokentool.app/createToken/eth). Fill in the token information .

![create token](../.gitbook/assets/Snipaste_2021-10-24_12-49-37.png)

Parameter introduction



**Currency name:** The name information of the token (such as BitCoin)

**Currency symbol:** The symbol information of the token (such as BTC)

**Initial supply:** The total supply of tokens (when the precision is 18 digits, the total supply can be followed by 15 0s, when the precision is 17 digits, the total supply can be followed by 16 0s, and so on.. )

**Accuracy:** The number of digits of precision of the token (the precision is the number of decimal places representing the currency `for example: 0.000001` means that there are 6 digits of precision)

**Creator/Owner:** The creator/owner of this token, the owner administrator, only the administrator can enter the administrator background to modify the handling fee parameters and other operations

**Description of handling fee (set tax for: `buy and sell`, `transfer` will charge tax):**

​ **Marketing tax:** After deducting the tax, local currency enters the marketing address

​ **Destruction tax:** Deduction of tax, the basic token will be destroyed according to the proportion of each transaction, and transferred to `0x000000000000000000000000000000000000dead` black hole address





## Token administrator introduction

Successfully created the token and generated the token address: `0xb1d1502fa0e5791c655b8e62e189335a25ebc8d4`, the token owner can manage the token through the `token administrator` function

![create token](../.gitbook/assets/Snipaste_2021-10-24_13-04-20.png)



**Enable suspension of transactions:** If enabled, the current token cannot be transferred (including swap operations)

**Blacklist Add/Remove:** By adding an address, the specified address will be filtered and cannot participate in any operation of the token, such as (scientist address added to the blacklist

**Burning amount:** Shrink the circulation of tokens, and put the total amount into the burning address.

**Number of minted coins:** To expand the supply, you need to fill in the address for minting coins, and send the minted coins to a certain address.

**Description of handling fee (set tax for: `buy and sell`, `transfer` will charge tax):**

​ **Marketing tax:** After deducting the tax, local currency enters the marketing address

​ **Destruction tax:** Deduction of tax, the basic token will be destroyed according to the proportion of each transaction, and transferred to `0x000000000000000000000000000000000000dead` black hole address

**Marketing address:** The marketing address can be modified twice.

**Temporarily give up permissions:** You can temporarily drop permissions, according to how many time units you set, after the time is up, you can get it back through the Token administrator page.

### Frequently Asked Questions

- **Could you explain the setup of the tax section? **
   - Answer: The tax setting is charged for **`Buy and Sell`** and **`Transfer`** operations, the marketing tax is entered into the marketing address, and the destruction tax is entered into the black hole address.
- **Can I set the tax separately for buying and selling differently? For example (buying marketing: 1%, selling marketing: 2%)? **
   - Answer: No, this version **`Business`** and **`Transfer`** are the same and cannot be disassembled. If you need to set differently, you can use other versions such as (V2, V3, version issued currency)
- **Why is there no swap platform to choose in this version? **
   - The reflow of this version tax is calculated in the local currency, so you can use any **`swap`** to add a pool, and you can use any **`trading pair`** to add a pool.







> Original link: [https://docs.tokentool.app/token/create-token](https://docs.tokentool.app/token/create-token)

>Video tutorial link: [https://youtu.be/K0PExlXV0LI](https://youtu.be/K0PExlXV0LI)