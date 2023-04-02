# Decrypt Encrypted JSON

This method enables the decryption of encrypted JSONs, also known as keystore.

```js
// decrypting encrypted JSON.

const decrypted = await multichainWallet.getWalletFromEncryptedJson({
  network: 'ethereum',
  json:
    '{"address":"1c082d1052fb44134a408651c01148adbfcce7fe","id":"abfb9f10-165a-4b7a-935d-51729f10c310","version":3,"Crypto":{"cipher":"aes-128-ctr","cipherparams":{"iv":"f3fac53ee2d76c293977d1af3a7d73bb"},"ciphertext":"c5034579cdf32d7a612c9a83801aad899abfebb7436712f363ecf89546bbcbce","kdf":"scrypt","kdfparams":{"salt":"78ff80ece5d681b1aecd829526388472d1889da233229fa5c1416e8f2035b7a8","n":131072,"dklen":32,"p":1,"r":8},"mac":"0f70eca6138ffe60b174308b6ab7a8a81a0d2b662e2cf5d8727443cf12af766c"}}',
  password: 'walletpassword',
});
```

## Response

```json
{
  privateKey: '0x0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
  address: '0x1C082D1052fb44134a408651c01148aDBFcCe7Fe'
}
```