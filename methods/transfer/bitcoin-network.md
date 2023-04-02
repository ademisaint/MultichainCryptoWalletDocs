# Bitcoin Network

This method allows for the transfer of BTC from one address to another.

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

## Prameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Private key | private key | yes | string | header
| Network | network type | yes | string | header
| Recipient address | reciever's address | yes | string | header
| Amount | quatity of coin | yes | string | header
| fee | tariff/charge | no | integer | query

## Response

```json
{
  object;
}
```
