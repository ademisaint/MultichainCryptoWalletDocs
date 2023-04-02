# Generate Wallet From Mnemonic

This generates a wallet from a Mnemonic phrase. The method takes an object as a parameter. This object's parameters are:

{% tabs %}

{% tab title="ETH" %}

```js
// Generate an Ethereum wallet from mnemonic.
const wallet = multichainWallet.generateWalletFromMnemonic({
  mnemonic:
    'candy maple cake sugar pudding cream honey rich smooth crumble sweet treat',
  derivationPath: "m/44'/60'/0'/0/0", // Leave empty to use default derivation path
  network: 'ethereum',
}); // NOTE - Address generated will work for EVM compatible blockchains E.g. Binance smart chain, Polygon etc
```

{% endtab %}

{% tab title="BTC" %}

```js
// Generate a Bitcoin wallet from mnemonic.
const wallet = multichainWallet.generateWalletFromMnemonic({
  mnemonic:
    'excess quit spot inspire stereo scrap cave wife narrow era pizza typical',
  derivationPath: "m/44'/0'/0'/0/0", // Leave empty to use default derivation path
  network: 'bitcoin', // 'bitcoin' or 'bitcoin-testnet'
});
```

{% endtab %}

{% tab title="SOL" %}

```js
// Generate a Solana wallet from mnemonic.
const wallet = multichainWallet.generateWalletFromMnemonic({
  mnemonic:
    'base dry mango subject neither labor portion weekend range couple right document',
  derivationPath: "m/44'/501'/0'/0'", // Leave empty to use default derivation path
  network: 'solana',
});
```

{% endtab %}

{% tab title="WAVES" %}

```js
// Generate a Waves wallet from mnemonic.
const wallet = multichainWallet.generateWalletFromMnemonic({
  mnemonic:
    'mushroom deliver work spray hire nuclear wrong deputy march six midnight outside motor differ adult',
  cluster: 'testnet',
  network: 'waves',
});
```

{% endtab %}

{% endtabs %}

## Parameters

| Parameter Name | Description | Required | Type | Parameter Type |
|----------------|-------------|----------|------|----------------|
| Mnemonic | mnemonics of the wallet | yes | string | header
| Network | network type | yes | string | query


## Response

```json
{
  address: '0x627306090abaB3A6e1400e9345bC60c78a8BEf57',
  privateKey: '0xc87509a1c067bbde78beb793e6fa76530b6382a4c0241e5e4a9ec0a0f44dc0d3',
  mnemonic: 'candy maple cake sugar pudding cream honey rich smooth crumble sweet treat'
}
```