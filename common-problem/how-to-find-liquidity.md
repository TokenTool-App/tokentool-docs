# How to find the contract address of a liquidity pool (LP)

When we add liquidity to a pool, we often need to know the contract address of the LP to lock the pool. Here are some methods to quickly find the LP contract address of your ERC20 token.

## Method 1: Search by adding liquidity record

1. Use a blockchain explorer to search for the transaction record of adding liquidity.
2. For example, use the transaction hash of adding liquidity, such as ( [https://testnet.bscscan.com/tx/0xdfd9412767cba1f16051850abd4d6685deb9d655f308624f8a65a0891ed87077](https://testnet.bscscan.com/tx/0xdfd9412767cba1f16051850abd4d6685deb9d655f308624f8a65a0891ed87077) )
3. In this example, 5 BNB and 1,000,000,000,000 Doge tokens were added to the Pancake exchange.
4. Finally, 2,236,067.977... LP tokens were obtained.
5. Click on the Pancake LPs token contract address.
6. Enter the Pancake LPs token contract details page (as shown below)
7. The address in the red part of the upper right corner is the LP token contract address.

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-05-16_16-10-28.png)

## Method 2: Search by contract address

1. Use a blockchain explorer to search for the contract address, in the `Contract` and `Read Contract` positions.

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-05-26_11-18-00.png)

2. Search for the keyword `uniswapPair`

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-05-26_11-19-02.png)

Note: By searching for the `uniswapPair` field address in the contract, you can obtain the LP address.

## Method 3: Search via the token admin page

1. Open the corresponding page of the token issuer and enter the token admin page (this method is suitable for contracts that have not lost their permissions).
2. Enter the contract address to enter the admin page.

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-05-26_11-24-01.png)

3. View the LP address.

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-05-26_11-25-24.png)

Note: This method searches for the LP address of the BNB-XXX trading pair. If you add liquidity to a non-BNB trading pair, please use the first method to find your LP address.

## Method 4: Use the contract security check function

1. Open the contract security check function URL: [https://tokentool.app/audit/contract](https://tokentool.app/audit/contract)
2. Select the supported blockchain and enter the contract address for security check.

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-11-24_22-25-45.png)

3. Obtain the pool address by checking the pool size detection information.

![add-liquidity](../.gitbook/assets/common-problem/Snipaste_2022-11-24_22-23-15.png)
