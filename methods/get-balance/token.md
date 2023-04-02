# Token

How to get balance of Tokens;

{% tabs %}

{% tab title="ERC20" %}

```js
// Get the balance of an ERC20 token.
const data = await multichainWallet.getBalance({
  address: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  tokenAddress: '0xdac17f958d2ee523a2206206994597c13d831ec7',
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% tab title="SOL" %}

```js
// Get the balance of a token on Solana.
const data = await multichainWallet.getBalance({
  address: '5PwN5k7hin2XxUUaXveur7jSe5qt2mkWinp1JEiv8xYu',
  tokenAddress: 'Es9vMFrzaCERmJfrF4H2FYD4KCoNkY11McCe8BenwNYB',
  network: 'solana',
  rpcUrl: 'https://rpc.ankr.com/solana',
});
```

{% endtab %}

{% tab title="WAVES" %}

```js
// Get the balance of a token on Waves.
const data = await multichainWallet.getBalance({
  network: 'waves',
  address: '3NBE5tjbQn9BHczjD6NSSuFDKVHKsBRzTv9',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  tokenAddress: '39pnv8FVf3BX3xwtC6uhFxffy2sE3seXCPsf25eNn6qG',
});
```

{% endtab %}

{% endtabs %}

## Parameter

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Address | network address | yes | string | path
| Network | network type | yes | string | header
| Token address | token address | yes | string | query

## Response

```text
{
  balance: 2;
}
```