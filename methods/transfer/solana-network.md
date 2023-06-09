# Solana Network

Allows the transfer of SOL and associated tokens between wallets, allowing for smooth transactions within the Solana blockchain ecosystem.

{% tabs %}

{% tab title="SOL" %}

````js
// Transferring SOL from one address to another.
const transfer = await multichainWallet.transfer({
  recipientAddress: '9DSRMyr3EfxPzxZo9wMBPku7mvcazHTHfyjhcfw5yucA',
  amount: 1,
  network: 'solana',
  rpcUrl: 'https://api.devnet.solana.com',
  privateKey:
    'bXXgTj2cgXMFAGpLHkF5GhnoNeUpmcJDsxXDhXQhQhL2BDpJumdwMGeC5Cs66stsN3GfkMH8oyHu24dnojKbtfp',
});
````

{% endtab %}

{% tab title="TOKEN" %}

```js
// Transferring a token from one address to another.
const transfer = await multichainWallet.transfer({
  recipientAddress: '9DSRMyr3EfxPzxZo9wMBPku7mvcazHTHfyjhcfw5yucA',
  tokenAddress: 'DV2exYApRFWEVb9oQkedLRYeSm8ccxNReLfEksEE5FZm',
  amount: 1,
  network: 'solana',
  rpcUrl: 'https://api.devnet.solana.com',
  privateKey:
    'h5KUPKU4z8c9nhMCQsvCLq4q6Xn9XK1B1cKjC9bJVLQLgJDvknKCBtZdHKDoKBHuATnSYaHRvjJSDdBWN8P67hh',
});
```

{% endtab %}

{% endtabs %}

## Prameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Private key | private key | yes | string | header
| Network | network type | yes | string | header
| Token Address | contract address  | No | string | header
| Recipient address | reciever's address | yes | string | header
| Amount | quatity of coin | yes | string | header
| rpcUrl| remote procedure call url | no | string | query

## Response

```json
{
  hash: '3nGq2yczqCpm8bF2dyvdPtXpnFLJ1oGWkDfD6neLbRay8SjNqYNhWQBKE1ZFunxvFhJ47FyT6igNpYPP293jXCZk';
}
```
