# Get Address From Private Key

This function returns the address associated with the private key passed as an argument. It accepts an object as input and the following parameters:

{% tabs %}

{% tab title="ETH" %}

```js
// Get the address from the private key on the Ethereum network.
const address = multichainWallet.getAddressFromPrivateKey({
  privateKey:
    '0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
  network: 'ethereum',
});
```

{% endtab %}

{% tab title="BTC" %}

```js
// Get the address from the private key on the Bitcoin network.
const data = multichainWallet.getAddressFromPrivateKey({
  privateKey: 'KxqTGtCMnX6oL9rxynDKCRJXt64Gm5ame4AEQcYncFhSSUxFBkeJ',
  network: 'bitcoin', // 'bitcoin' or 'bitcoin-testnet'
});
```

{% endtab %}

{% tab title="SOL" %}

```js
// Get the address from the private key on the Solana network.
const address = multichainWallet.getAddressFromPrivateKey({
  privateKey:
    'bXXgTj2cgXMFAGpLHkF5GhnoNeUpmcJDsxXDhXQhQhL2BDpJumdwMGeC5Cs66stsN3GfkMH8oyHu24dnojKbtfp',
  network: 'solana',
});
```

{% endtab %}

{% endtabs %}

## Response

```json
{
  address: '0x1C082D1052fb44134a408651c01148aDBFcCe7Fe';
}
```