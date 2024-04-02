# DID-Authenticator

A lightweight utility package for decentralized identity (DID) authentication.

## Installation

Install the package using npm:

```bash
npm install did-authenticator
```

## Usage

```javascript
const { verifyDID } = require('did-authenticator');

const userDID = 'did:example:123456789';
const userSignature = '...'; // User's signature

const isValid = verifyDID(userDID, userSignature);
if (isValid) {
  console.log('User authenticated successfully!');
} else {
  console.error('Invalid authentication.');
}
```

## API

### `verifyDID(did, signature)`

Verifies the authenticity of a user based on their DID and provided signature.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
