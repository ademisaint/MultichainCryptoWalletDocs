# Get Address From Private Key

This method extracts the address associated with the provided private key by taking an object as its parameter. 

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

## Parameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Private Key | secret key | yes | string | header
| network | network type | yes | string | query

## Response

```json
{
  address: '0x1C082D1052fb44134a408651c01148aDBFcCe7Fe';
}
```