# Transfer

This function allows you to transfer a set number of tokens from a source address to a destination address. It takes an object as input and transfers the specified number of tokens.

1. [Ethereum Network](./ethereum-network.md)
2. [Bitcoin Network](./bitcoin-network.md)
3. [Solana Network](./solana-network.md)
4. [Waves Network](./waves-network.md)

The optional parameters that the object takes in are: gas price, nonce, and data.

- The gas price is the price of gas in Gwei. The higher the gas price, the faster the transaction will be. It's best to use a higher gas price than the default.
- The nonce is the number of transactions that have been sent from the source address and is used to ensure that the transaction is unique. The transaction is unique because the nonce is incremented each time a transaction is sent.
- The data is a string parameter used to pass across a message through the transaction. Can only be used on transfer of ETH.