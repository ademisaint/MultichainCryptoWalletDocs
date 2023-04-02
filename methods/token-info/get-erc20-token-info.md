# Get ERC20 Token Info

With this, information on ERC20 tokens from compatible blockchains can be retrieved using their respective token addresses.

```js
// getting token info.

const info = await multichainWallet.getTokenInfo({
  address: '0x7fe03a082fd18a80a7dbd55e9b216bcf540557e4',
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

## parameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Address | network address | yes | string | header
| Network | network type | yes | string | query
| rpcUrl | rpcUrl | No | string | query

## Response

```json
{
  name: 'Mocked USDT',
  symbol: 'USDT',
  decimals: 6,
  address: '0x7fe03a082fd18a80a7dbd55e9b216bcf540557e4',
  totalSupply: 1000000000000
}
```
