# Bitcoin Network

Allows for the transfer of BTC from one address to another.

{% tabs %}

{% tab title="BTC" %}

```js
// Transferring BTC from one address to another.
const response = await multichainWallet.transfer({
  privateKey: 'L3tSvMViDit1GSp7mbV2xFCGv6M45kDNuSyNY9xyUxmUPBFrBkc4',
  recipientAddress: '2NAhbS79dEUeqcnbC27UppwnjoVSwET5bat',
  amount: 0.001,
  network: 'bitcoin-testnet', // 'bitcoin' or 'bitcoin-testnet'
  fee: 10000, // Optional param default value is 10000
  subtractFee: false, // Optional param default value is false
});
```

{% endtab %}

{% endtabs %}

## Response

```json
{
  object;
}
```
