# Batch deauthorization

The blockchain is becoming more and more mature in the decentralized field, and more and more decentralized applications are developed on the blockchain. For example, the DeFi field has become popular in recent years. The main DeFi applications include ERC20 token lending, pledge and trade. If you want to use ERC20 on DeFi protocols such as [Uniswap](https://uniswap.org/), [Aave](https://aave.com/) and [Yearn](https://yearn.finance/) Tokens, you need to authorize the dApp to use these tokens. This is called _**ERC20 Authorization**_. These authorizations are essential to the functioning of DeFi platforms, but can be very dangerous if left unchecked.

![approve](../.gitbook/assets/approve.png)

## ERC20 authorization process

First of all, let's take a look at a picture, what is the authorization process like. User A authorizes USDT tokens to another contract \(unsafe\) or personal address when accessing the dApp. At this time, it is equivalent to authorizing U to the target with a certain amount to operate your U. This is a very dangerous situation. In the recent period, there have been many incidents similar to stealing U. Similar to using this method, many users lack blockchain knowledge and think that it is just an authorized operation.

## Pirate U case analysis

1. The attacker forges an empty activity page and distributes information through multiple channels such as the media
2. The user clicks the button to receive short positions through the page, and at this time the contract `approve` is called to authorize, the authorized object is the attacker's address, and the authorized amount is unlimited
3. The attacker transfers the USDT in the user's wallet through `transferFrom`.

    ![Phishing](../.gitbook/assets/Snipaste_2021-09-29_14-49-29.png)![Phishing](../.gitbook/assets/Snipaste_2021-09-29_14-51-41.png)

In the picture we can see the call authorization information\(use your USDT\)

0x095ea7b3000000000000000000000000 (call authorization function

57ce3d5cd8685bed28ae71f3a5cfd3b42464fe0b (authorized to attacker address

0ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff

After the current authorization is confirmed, `57ce3d5cd8685bed28ae71f3a5cfd3b42464fe0b` attacker can transfer all your USDT away, as long as you have U, he can transfer away. If the address does not cancel the authorization in time, it will bring more losses. The following will teach you how to check which contracts and addresses are authorized by the wallet address, and regularly cancel the expired contracts.

## Solution

Use Token Tool [https://TokenTool.App](https://tokentool.app) or [https://TokenTool.App/approve/eth](https://tokentool.app/approve/eth) to query Address authorization information.

![cointool](../.gitbook/assets/Snipaste_2021-09-29_15-10-52.png)

1. Link the wallet, scan the wallet address (If you have not authorized the contract, prompt: you have not authorized tokens to the contract, great!

![cointool](../.gitbook/assets/Snipaste_2021-09-29_15-13-14.png)

1. Scan out the authorized contract information (⚠️The scanned address is not the current user wallet address, and the authorization cannot be canceled

![cointool](../.gitbook/assets/Snipaste_2021-09-29_15-15-51.png)

```text
// The essence of canceling the authorization is to call the contract authorization, and authorize the amount of 0 to the target address
0x095ea7b3 // authorization method
0000000000000000000000001bb7995f64c393a73a480ec7400bb52c335a4809 // authorized address
00000000000000000000000000000000000000000000000000000000000000000 // authorized amount (0)
```

> Original link: [https://docs.tokentool.app/learn/batch-approve](https://github.com/TokenTool-App/tokentool-docs/blob/main/learn/batch-approve.md)
>
> Citing reference knowledge
>
> [https://medium.com/zengo/unicats-go-phishing-eaf39ff9da64](https://medium.com/zengo/unicats-go-phishing-eaf39ff9da64) UniCats Phishing Analysis
>
> [https://www.lianzixun.cn/news/9562620.html](https://www.lianzixun.cn/news/9562620.html) Transfer authorization phishing to control your wallet