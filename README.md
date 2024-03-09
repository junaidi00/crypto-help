# Crypto Help

A Node.js module for handling cryptocurrency operations.

## Installation

```bash
npm install crypto-help
```

## USAGE

```javascript
const { convertCurrency, encryptTransactionDetails, decryptTransactionDetails } = require('crypto-help');

// Convert currency
const convertedAmount = convertCurrency(100, 'BTC', 'ETH');
console.log(convertedAmount);

// Encrypt transaction details
const transaction = { from: 'Alice', to: 'Bob', amount: 10 };
const key = 'secret_key';
const encryptedTransaction = encryptTransactionDetails(transaction, key);
console.log('Encrypted Transaction:', encryptedTransaction);

// Decrypt transaction details
const decryptedTransaction = decryptTransactionDetails(encryptedTransaction, key);
console.log('Decrypted Transaction:', decryptedTransaction);
```