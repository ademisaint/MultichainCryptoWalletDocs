# Get Transaction

This returns the transaction receipt for a given transaction hash. An object is provided as a parameter to this method

{% tabs %}

{% tab title="ETH" %}

```js
// Get the transaction receipt on Ethereum network.
const receipt = await multichainWallet.getTransaction({
  hash: '0x5a90cea37e3a5dbee6e10190ff5a3769ad27a0c6f625458682104e26e0491055',
  network: 'ethereum',
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% tab title="BTC" %}

```js
// Get the transaction receipt on Bitcoin network.
const receipt = await getTransaction({
  network: 'bitcoin-testnet', // 'bitcoin' or 'bitcoin-testnet'
  hash: '4f6c3661e0e6d190dbdfb6c0791396fccee653c5bf4a5249b049341c2b539ee1',
});
```

{% endtab %}

{% tab title="SOL" %}

```js
// Get the transaction receipt on Solana network.
const receipt = await multichainWallet.getTransaction({
  rpcUrl: 'https://api.devnet.solana.com',
  hash:
    'CkG1ynQ2vN8bmNsBUKG8ix3moUUfELWwd8K2f7mmqDd7LifFFfgyFhBux6t22AncbY4NR3PsEU3DbH7mDBMXWk7',
  network: 'solana',
});
```

{% endtab %}

{% tab title="WAVES" %}

```js
// Get the transaction receipt on Waves network.
const receipt = await multichainWallet.getTransaction({
  rpcUrl: 'https://nodes-testnet.wavesnodes.com',
  hash: 'Barwuj1gCiQ9wCfLQ1nbdz2CSyQXLnRxnDEubtdTwJpd',
  network: 'waves',
});
```

{% endtab %}

{% endtabs %}

## Parameters 

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Hash | network address | yes | string | header
| Network | network type | yes | string | query

## Response

```json
{
  object;
}
```