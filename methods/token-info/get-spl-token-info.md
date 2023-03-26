# Get SPL Token Info

Allows for fetching SPL tokens info on the solana by the token address. Note: Token has to be available on the solana token list registry

```js
// getting token info.

const info = await multichainWallet.getTokenInfo({
  address: '7Xn4mM868daxsGVJmaGrYxg8CZiuqBnDwUse66s5ALmr',
  network: 'solana',
  rpcUrl: 'https://api.devnet.solana.com',
  cluster: 'devnet',
});
```

## Response

```json
{
  object;
}
```
