# Ethereum Network

{% tabs %}

{% tab title="READ" %}

```js
// Calling a read smart contract function.
const data = await multichainWallet.smartContractCall({
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  network: 'ethereum',
  contractAddress: '0x5592EC0cfb4dbc12D3aB100b257153436a1f0FEa',
  method: 'transfer',
  methodType: 'write',
  params: ['0x2455eC6700092991Ce0782365A89d5Cd89c8Fa22', '1000000000000000000'],
  contractAbi: [
    {
      constant: false,
      inputs: [
        { name: '_to', type: 'address' },
        { name: '_value', type: 'uint256' },
      ],
      name: 'transfer',
      outputs: [{ name: '', type: 'bool' }],
      payable: false,
      stateMutability: 'nonpayable',
      type: 'function',
    },
  ],
  privateKey:
    '0f9e5c0bee6c7d06b95204ca22dea8d7f89bb04e8527a2c59e134d185d9af8ad',
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% tab title="WRITE"%}

```js
// calling a write smart contract function.
const data = await multichainWallet.smartContractCall({
  rpcUrl: 'https://rpc.ankr.com/eth_goerli',
  network: 'ethereum',
  contractAddress: '0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D',
  method: 'factory',
  methodType: 'read',
  params: [],
  contractAbi: [
    {
      inputs: [],
      name: 'factory',
      outputs: [{ internalType: 'address', name: '', type: 'address' }],
      stateMutability: 'view',
      type: 'function',
    },
  ],
}); // NOTE - For other EVM compatible blockchains all you have to do is change the rpcUrl.
```

{% endtab %}

{% endtabs %}

## Response

````json
{
  data: object;
}
````