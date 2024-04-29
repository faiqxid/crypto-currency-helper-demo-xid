```markdown
# Crypto Currency Helper Demo X

This is a demo for the crypto-currency-helper package, showcasing its usage for currency conversion and transaction encryption/decryption.

## Installation

To use this demo, you need to have Node.js installed on your machine.

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Usage

```javascript
const { convertCurrency, encryptTransactionDetails, decryptTransactionDetails } = require('crypto-currency-helper');

// Convert currency
const convertedAmount = convertCurrency(100, 'BTC', 'ETH');
console.log('Converted Amount:', convertedAmount);

// Encrypt transaction details
const transaction = { from: 'Alice', to: 'Bob', amount: 10 };
const key = 'secret_key';
const encryptedTransaction = encryptTransactionDetails(transaction, key);
console.log('Encrypted Transaction:', encryptedTransaction);

// Decrypt transaction details
const decryptedTransaction = decryptTransactionDetails(encryptedTransaction, key);
console.log('Decrypted Transaction:', decryptedTransaction);
```

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```