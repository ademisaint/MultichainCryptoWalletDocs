# Ethereum Network

Enables ETH transfer and transaction overriding.

## Transfer

{% tabs %}

{% tab title="ETH" %}

```js
// Transferring ETH from one address to another.
const transfer = await multichainWallet.transfer({
  recipientAddress: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  amount: 1,
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  privateKey:
    '0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
  gasPrice: '10', // Gas price is in Gwei. Leave empty to use default gas price
  data: 'Money for transportation', // Send a message
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% tab title="ERC20" %}

```js
// Transferring ERC20 tokens from one address to another.
const transfer = await multichainWallet.transfer({
  recipientAddress: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  amount: 10,
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  privateKey:
    '0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
  gasPrice: '10', // Gas price is in Gwei. leave empty to use default gas price
  tokenAddress: '0xdac17f958d2ee523a2206206994597c13d831ec7',
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% endtabs %}

## override

{% tabs %}

{% tab title="ETH" %}

```js
// Overriding pending ETH transaction.
const transfer = await multichainWallet.transfer({
  recipientAddress: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  amount: 0,
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  privateKey:
    '0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
  gasPrice: '10',
  nonce: 1, // The pending transaction nonce
  data: 'Money for feeding', // Send a message
});

```

{% endtab %}

{% tab title="ERC20" %}

```js
// Overriding ERC20 token pending transaction.
const transfer = await multichainWallet.transfer({
  recipientAddress: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  amount: 0,
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  privateKey:
    '0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
  gasPrice: '10',
  tokenAddress: '0xdac17f958d2ee523a2206206994597c13d831ec7',
  nonce: 1, // The pending transaction nonce
});
```

{% endtabs %}

## Response

```json
{
  object;
}
```
