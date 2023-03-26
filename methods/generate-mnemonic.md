# Generate Mnemonic

This process is used to produce mnemonics. The default word count is 12, but if you wish to generate more or less, you may give a numeric parameter.

```js
const mnemonic = multichainWallet.generateMnemonic();

// Note: Mnemonics with less than 12 words have low entropy and may be guessed by an attacker.
```

## Response

```json
net idle lava mango another capable inhale portion blossom fluid discover cruise
```
