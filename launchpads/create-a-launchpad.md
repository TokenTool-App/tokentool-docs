# create launchpad

## Step 1: Validate the token
1. Link your wallet.
2. Go to [https://tokentool.app/launchpad/create](https://tokentool.app/launchpad/create)
3. Enter your token address (if you already have one), if not, you can create your token through [one-click issuance](https://tokentool.app/createToken/V2)
4. After entering the token, the token information will be displayed. After clicking [Authorize], you can enter the next step

![create-luanchpad](../.gitbook/assets/launchpad/Snipaste_2022-05-05_22-05-50.png)

5. MetaMask will now ask you to authorize the operation of the contract. If you agree, click the "Confirm" button to complete the process.



## Step 2: Fill in the pre-sale information

When your authorization is complete, you will come to the second step, you need to enter your raised Launchpad information, the following are some important parameter information:

1. All scale and numerical information must use positive numbers
2. The pre-sale rate indicates how many tokens private equity investors can get by spending 1 BNB during the pre-sale stage.
3. Whitelist: If your presale is in private mode or has a whitelist of presale contributors, please select "Enable". You can enable/disable the whitelist at any time later
4. Soft cap: the soft cap must be greater than or equal to 50% of the hard cap
5. Refund type: If you reach the hard cap at the end of the pre-sale, you can choose to refund or destroy the extra tokens
6. Liquidity (%), the percentage of liquidity allocated to the Swap decentralized exchange, the minimum value is 51%, and the maximum value is 100%
7. Listing rate, the initial fee rate of the liquidity pool when the listing rate is listed (1 BNB = x token). This price is usually lower than the pre-sale price, and has been used to obtain a higher listing price on the Swap exchange
8. The pre-sale start time must be greater than the current time
9. The pre-sale end time must be greater than the pre-sale start time
10. Liquidity lock (minutes): After listing, the LP pool lock time is listed as 60 minutes.

You can check the total amount of tokens required to create a presale pool (displayed above the previous/next buttons)

Here is an example:

![create-launchpad](../.gitbook/assets/launchpad/Snipaste_2022-05-05_22-18-03.png)



Analyze example data, (current pre-sale data)

1. The pre-sale rate is (1BNB=200) quantity,

2. Soft top: 500, hard top: 1000. Then the pre-sale will need 200 * 1000 = 200000 tokens for sale,
3. The minimum buy-in is 0.01, and the maximum buy-in is 0.1, which means that an address can only buy 0.1BNB at most, so it will also get 20 tokens correspondingly
4. Refund type Burning, if the pre-sale is over and the private placement BNB has not reached the hard cap, but has reached the soft cap of 500BNB, then 100,000 tokens of the 200,000 tokens sold in the private placement will be transferred to the black hole address.
5. The router will be a decentralized exchange to be listed, such as the pancake-Swap of the BSC chain
6. Liquidity (%), the percentage of private placement funds allocated to liquidity, what percentage of the BNB you privately raised will need to be allocated, (for example, if 1,000 BNB are privately raised, 80% will be Use 800 BNB to add liquidity, and there is 20% left, 200BNB will eventually be returned to the address of the pre-seller)
7. Listing rate: The initial fee rate of the liquidity pool at the listing rate (1 BNB = 150 tokens as shown in the figure).
8. Ultimately adding liquidity will require (800 * 150 tokens = 120000 tokens and 800 BNB to add liquidity)
9. When the pre-sale starts, private investors can purchase
10. The end of the pre-sale time. At the end of the time, your private placement fee must reach the minimum soft cap standard, otherwise it will be a failed pre-sale.
11. Your liquidity is locked for 500 minutes after the opening
12. In the end you need 120,000 tokens to add liquidity and 200,000 tokens for pre-sale



## Step 3: Add additional information

There are some caveats for this step:

1. Logo URL and website address are required and cannot be empty. Without these, you will not be able to complete this step.

2. The logo URL must end with a supported image extension: png, jpg, jpeg, or gif.

    For example: https://ipfs.io/ipfs/Qma34oPEZzS5nEcKxzrdvpW6Th2gR2qxKayE18CFwNSJN6

    If you don't have an online picture URL, you can use the [TokenTool IPFS](https://tokentool.app/other/ipfs) file system to upload pictures to IPFS

3. After the input is complete, click Next.



Here's an example:




![create-launchpad](../.gitbook/assets/launchpad/Snipaste_2022-05-05_22-46-16.png)



## Step 4: Finish

This is the last step, you can check all your parameter setting information before submitting for the last time, make sure everything is normal and click "Submit", or you can return to the previous step to make changes.



Here's an example of who:

![create-launchpad](../.gitbook/assets/launchpad/Snipaste_2022-05-05_22-52-59.png)



After clicking "Submit", MetaMask will now ask you to confirm the transaction. It will also show you the fee you need to pay for the transaction. If you agree, then click the "Confirm" button to complete the process with the following result:



![create-launchpad](../.gitbook/assets/launchpad/Snipaste_2022-05-05_23-05-53.png)