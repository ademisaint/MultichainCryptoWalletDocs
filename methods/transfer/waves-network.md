# Waves Network

This option allows for the seamless transfer of WAVES and associated tokens between wallets within the Waves blockchain ecosystem.

{% tabs %}

{% tab title="WAVES" %}

```js
// Transferring WAVES from one address to another.

const response = await multichainWallet.transfer({
  recipientAddress: '3N4x4ML4D6fiU18Tpw86puRoN78FCTs9VQu',
  amount: 0.0001,
  network: 'waves',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  privateKey:
    'mushroom deliver work spray hire nuclear wrong deputy march six midnight outside motor differ adult',
});
```

{% endtab %}

{% tab title="TOKEN" %}

```js
// Transferring a token from one address to another.
const transfer = await multichainWallet.transfer({
  recipientAddress: '3N4x4ML4D6fiU18Tpw86puRoN78FCTs9VQu',
  tokenAddress: '39pnv8FVf3BX3xwtC6uhFxffy2sE3seXCPsf25eNn6qG',
  amount: 1,
  network: 'waves',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  privateKey:
    'mushroom deliver work spray hire nuclear wrong deputy march six midnight outside motor differ adult',
});
```

{% endtab %}

{% endtabs %}

## Prameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Private key | secret key | yes | string | header
| Network | network type | yes | string | header
| Token Address | contract address  | yes | string | header
| Recipient address | reciever's address | yes | string | header
| Amount | quatity of coin | yes | string | header
| rpcUrl| remote procedure call url | no | string | query

## Response

```json
{
  type: 4,
  id: '9CbA3dsyEvbdf52gqeBvVkjEP5zBmCQPANjguNznHryf',
  fee: 100000,
  feeAssetId: null,
  timestamp: 1661781621495,
  version: 3,
  chainId: 84,
  sender: '3NBE5tjbQn9BHczjD6NSSuFDKVHKsBRzTv9',
  senderPublicKey: '8JEFTsZfqp2Y7HpmaxqgGtiMLfsNAAq3bMkwZwGpUWPV',
  proofs: [
    '5m4DpkkYkVY4xkiMNyrNpiVUHNNAtyJrSH5UCkjWSnLTAabkCefLx6wWTFT1Xcb7K8C31H7ndZAX8mWrJLMrsqxr'
  ],
  recipient: '3N4x4ML4D6fiU18Tpw86puRoN78FCTs9VQu',
  assetId: '39pnv8FVf3BX3xwtC6uhFxffy2sE3seXCPsf25eNn6qG',
  feeAsset: null,
  amount: 100000000,
  attachment: ''
}
```
