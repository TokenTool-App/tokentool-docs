# NFT batch sending

> **TokenTool is a blockchain toolbox that supports ETH, BSC, and many other public chains. **
> **It is recommended to use the computer version of Google Chrome + `Metamask` plug-in wallet for operation.**
> **Mobile phone users can also operate in `Wallet APP`-Discover-Enter the official website link.**

### Function Description

```

The batch sending function of NFT allows users to send multiple NFTs to multiple addresses in a one-time operation.
Scenario: Send 100 XX-NFT in the current linked wallet to 100 addresses.
Note: You need to know the NFT contract address of the wallet and each NFTID.

```

## First step

![nft-multiSender](../.gitbook/assets/nft/image-20231117161814363.png)

1. Open the batch sending NFT function link page https://tokentool.app/nft/multiSender/bsc

2. Paste the NFT contract address to be sent into the input box

3. Enter the receiving address and received NFTID, and you can view the format template through [Show Example] in the lower right corner.
    1. Format usage: address, NFTID (⚠️Note that the comma is an English comma symbol)
    1. In the example: `0xd41b9AC5767cd90AbC7C997730591cBb7223D3D9,1` sends the NFT with NFTID 1 to the `...3D3D9` address
   
4. You can also upload the xlsx form of the file through [Upload File]. The format needs to be filled in according to the [template file] (https://tokentool.app/example.xlsx).

![nft-multiSender](../.gitbook/assets/nft/image-20231117162124689.png)

6. Address is the receiving address, and Amount is NFTID.

## Second step

![nft-multiSender](../.gitbook/assets/nft/image-20231117162504488.png)

1. Determine the sending address and the NFTID sent
2. Click Approve to perform the authorization operation.
3. MetaMask will now ask you to confirm the transaction. If you agree, click the "Confirm" button to complete the process.
4. After completing the Approve authorization operation, proceed to the next step to send NFT in batches.

![nft-multiSender](../.gitbook/assets/nft/image-20231117163116173.png)