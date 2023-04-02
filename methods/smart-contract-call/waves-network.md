# Waves Network

{% tabs %}

{% tab title="READ" %}

```js
// calling a read smart contract function.
const data = await multichainWallet.smartContractCall({
  network: 'waves',
  methodType: 'read',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  contractAddress: '3N9uzrTiArce1h9VCqK3QUUZmFqBgg5rZSW',
  method: '3N1gVpA5MVY4WsMpzQ6RfcscpDDdqBbLx6n_balance',
  params: [],
});
```

{% endtab %}

{% tab title="WRITE"%}

```js
// calling a write smart contract function.
const data = await multichainWallet.smartContractCall({
  network: 'waves',
  methodType: 'write',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  contractAddress: '3N9uzrTiArce1h9VCqK3QUUZmFqBgg5rZSW',
  privateKey:
    'mushroom deliver work spray hire nuclear wrong deputy march six midnight outside motor differ adult',
  method: 'deposit',
  payment: [{ assetId: null, amount: 1000 }],
  params: [],
});
```

{% endtab %}

{% endtabs %}

## Prameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| private key | secret key | yes | string | header
| Network | network type | yes | string | query
| rpcUrl | rpcUrl | No | string | query
| address | contractAddress | yes | string | header

## Response

````json
{
  data: object;
}
````