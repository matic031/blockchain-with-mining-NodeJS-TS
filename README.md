# Blockchain with mining made with NodeJS and TypeScript


This code implements a basic blockchain system with transactions, blocks, a chain, and a wallet.

The Transaction class represents a transaction with an amount, payer, and recipient. It has a method to serialize the transaction as a string.

The Block class represents a block in the blockchain. It has properties such as the previous block's hash, a transaction, and a timestamp. It also has a getter method to calculate the hash of the block using the SHA256 hashing algorithm.

The Chain class represents the blockchain itself. It is implemented as a singleton and contains an array of blocks. It has a method to mine a block by finding a solution that satisfies certain conditions. It also has a method to add a new block to the chain, after verifying the transaction and mining it. The Chain class also has a getter method to retrieve the last block in the chain.

The Wallet class represents a user's wallet in the blockchain system. It generates a key pair (public key and private key) using the RSA algorithm. It has a method to send money from the user's wallet to another wallet by creating a transaction, signing it with the private key, and adding it to the blockchain.

Overall, this code provides a basic implementation of a blockchain system with transactions, mining, and verification functionality.