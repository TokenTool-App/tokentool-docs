# create mining
How to use TokenTool to create mining activities
[https://youtu.be/QfqfRCVvPc8](https://youtu.be/QfqfRCVvPc8)

## Step 1: Mining Rules

1. Link your wallet.
2. Go to [https://tokentool.app/mining/list](https://tokentool.app/mining/list) to create a mining page.
3. Click Create Mining

![create-mining](../.gitbook/assets/mining/Snipaste_2022-06-20_16-37-44.png)

#### **1.1 Select mining type**
TokenTool provides the following two different mining types, both of which do not support deflationary tokens (the deflationary type automatically increases or decreases the supply according to the price of the currency), once the mining pool is created, the parameters cannot be modified.

- **Single currency pledge mining**: Encourage users to lock tokens and reduce circulating tokens; after creation, users only need to pledge one token to obtain mining income;
- **Dual currency market-making mining**: Encourage users to make market for project tokens and improve the liquidity of tokens on the chain; after creation, users need to pledge two tokens in the liquidity pool to make market , to obtain LP, and then pledge LP in the mining pool to obtain mining rewards.
#### **1.2 Set Mining Pool Parameters**
1. Token address: the contract address that the user pledges. If it is **dual currency market making mining** it is the LP pool address.
2. Start time: Select the time to start mining, which must be greater than the current time
3. Duration: the total number of mining days, (integer units).
4. Lock-up time: the lock-up time of the user's pledged balance, which can only be withdrawn after the expiration time.
5. Invitation mechanism: Whether to enable the invitation mechanism.
6. Invitation ratio: After the user invites the sub-agent, the reward commission ratio. The unit per thousand, such as (100, is 100 thousandths, assuming that user A rewards 1000 tokens, 100 ratios will be transferred to the inviter).

## Step 2: Reward Rules
![create-mining](../.gitbook/assets/mining/Snipaste_2022-06-20_16-39-49.png)
1. Enter the address of the reward contract, and the user rewards those who pledge to the user.
1. Enter the number of daily rewards and the total number of rewards: the rewards for participating mining users are divided according to the proportion of participating funds.
1. Logo, official website and other extended information.


## Step 3: Confirm completion

![create-mining](../.gitbook/assets/mining/Snipaste_2022-06-20_16-40-07.png)

After confirming that the information is correct, **[Authorize]** and **[Create]** two steps, after clicking "Submit", MetaMask will now ask you to confirm the transaction. It will also show you the fee you need to pay for the transaction. If you agree, then click the "Confirm" button to complete the process with the following result:

![create-mining](../.gitbook/assets/mining/Snipaste_2022-06-20_16-41-15.png)