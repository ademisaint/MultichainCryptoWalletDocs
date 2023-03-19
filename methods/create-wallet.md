# Create Wallet

A new wallet is created using this technique. A payload object can be used as a parameter for the method. The payload's parameter is:

{% tab %}

{% tab title="ethereum" %}

```text
// Creating an Ethereum wallet.
const wallet = multichainWallet.createWallet({
  derivationPath: "m/44'/60'/0'/0/0", // Leave empty to use default derivation path
  network: 'ethereum',
}); // NOTE - Address generated will work for EVM compatible blockchains E.g. Binance smart chain, Polygon etc
```

{% endtab %}

{% tab title="Bitcoin" %}

```text
// Creating a Bitcoin wallet.
const wallet = multichainWallet.createWallet({
  derivationPath: "m/44'/0'/0'/0/0", // Leave empty to use default derivation path
  network: 'bitcoin', // 'bitcoin' or 'bitcoin-testnet'
});
```

{% endtab %}

{% tab title="solana" %}

```text
// Creating a Solana wallet.
const wallet = multichainWallet.createWallet({
  derivationPath: "m/44'/501'/0'/0'", // Leave empty to use default derivation path
  network: 'solana',
});
```

{% endtab %}

{% tab title="waves" %}

```text
// Creating a Waves wallet.
const wallet = await multichainWallet.createWallet({
  cluster: 'testnet' // Can also be mainnet,
  network: 'waves',
});
```

{% endtab %}

{% endtab %}

## Response

´´´Text
{
  address: '0xfBE11AC0258cc8288cA24E818691Eb062f7042E9',
  privateKey: '0xfdf745f45d1942feea79b4c0a3fc1ca67da366899f7e6cebaa06496806ca8127',
  mnemonic: 'net idle lava mango another capable inhale portion blossom fluid discover cruise'
}
```

