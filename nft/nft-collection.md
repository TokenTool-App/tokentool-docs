# NFT batch collection

> **TokenTool is a blockchain toolbox that supports ETH, BSC, and many other public chains. **
> **It is recommended to use the computer version of Google Chrome + `Metamask` plug-in wallet for operation.**
> **Mobile phone users can also operate in `Wallet APP`-Discover-Enter the official website link.**

### Function Description

```

The NFT batch collection function allows users to merge NFTs stored in multiple addresses into a single address or contract.
Scenario: Send NFTs in a small address to a large address in batches

```

## First step

![nft-collection](../.gitbook/assets/nft/image-20231117171115512.png)

1. Open the NFT batch collection function link page [https://tokentool.app/nft/NftMoreToOne/bsc](https://tokentool.app/nft/NftMoreToOne/bsc)
2. Use the [import Account] button to import the private key of the small address that needs to be collected.
3. After entering the NFT contract address to be aggregated, click [Auto Get TokenId] to automatically obtain the NFTID of the address.
    1. If you cannot obtain the NFTID, please manually edit the ID value present in each address.
4. Enter the receiving address and send to the specified address.

![nft-collection](../.gitbook/assets/nft/image-20231117172628892.png)

1. Start the collection operation, and the collection is successful through transaction Hash.





### Frequently Asked Questions

- **Why can't I get the ID value from my address**
   - Answer: It is possible that your NFT contract does not have a function to query ID by address (for example, these functions do not exist: `tokensOfOwner(address)`, `walletOfOwner(address)`, `getOwnerTokens(address)`), which will not be possible. If the ID is found, it is also possible that there is no NFT in the current address.

- **Do I need to retain mining fees for batch collection of NFT small addresses**
   - Answer: Yes, batch collection is the same as transferring funds through your wallet. The tool only replaces your transfer operation. In the end, the address initiates the transfer, so gas and mining fees are required. In order to avoid failure, try to reserve as much mining fees as possible.