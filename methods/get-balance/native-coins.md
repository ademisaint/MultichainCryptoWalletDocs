# Native Coins

How to get the balance of native coins;

{% tabs %}

{% tab title="ETH" %}

```js
// Get the ETH balance of an address.
const data = await multichainWallet.getBalance({
  address: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
}); // NOTE - For otherEVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% tab title="BNB" %}

```js
// Binance Smart chain
const data = await multichainWallet.getBalance({
  address: '0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22',
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
});
```

{% endtab %}

{% tab title="BTC" %}

```js
// Get the BTC balance of an address.
const data = await multichainWallet.getBalance({
  address: '2NAhbS79dEUeqcnbC27UppwnjoVSwET5bat',
  network: 'bitcoin-testnet', // 'bitcoin' or 'bitcoin-testnet'
});
```

{% endtab %}

{% tab title="SOL" %}

```js
// Get the SOL balance of an address.
const data = await multichainWallet.getBalance({
  address: 'DYgLjazTY6kMqagbDMsNttRHKQj9o6pNS8D6jMjWbmP7',
  network: 'solana',
  rpcUrl: 'https://api.devnet.solana.com',
});
```

{% endtab %}

{% tab title="WAVES" %}

```js
// Get the WAVES balance of an address.
const data = await multichainWallet.getBalance({
  network: 'waves',
  address: '3NBE5tjbQn9BHczjD6NSSuFDKVHKsBRzTv9',
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
});
```

{% endtab %}

{% endtabs %}

## Parameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Address | network address | yes | string | path
| Network | network type | yes | string | query

## Response

```json
{
  balance: 2;
}
```