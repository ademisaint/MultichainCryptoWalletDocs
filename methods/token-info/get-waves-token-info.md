# Get Waves Token Info

This method is used for fetching Waves based asset info.

```js
// getting token info.

const info = await multichainWallet.getTokenInfo({
  network: 'waves',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  address: '39pnv8FVf3BX3xwtC6uhFxffy2sE3seXCPsf25eNn6qG',
});
```

## Response

## Prameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Network | network type | yes | string | query
| rpcUrl | rpcUrl | No | string | query
| Address | contract address | yes | string | header

```json
{
  name: 'T-BTC',
  symbol: 'T-BTC',
  address: '39pnv8FVf3BX3xwtC6uhFxffy2sE3seXCPsf25eNn6qG',
  decimals: 8,
  totalSupply: 2100000000000000
}
```
