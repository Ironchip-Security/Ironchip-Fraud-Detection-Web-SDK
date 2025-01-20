# Ironchip-Fraud-Detection-Web-SDK

# LBFraud Web SDK

## How to use?

```js
//import the lbfraud_sdk library 
import { LBFraudSDK,LBFraudSDKEnvironment } from 'lbfraud_sdk';

//Initialize the client the available environments are Development, Testing and Production(default) 
const client = new LBFraudSDK({
  apiKey: 'api-key',
  environment: LBFraudSDKEnvironment.Testing,
});

//TransactionID (required,unique): transaction identifier request for fraud results
//UserID (required): User identifier

client.sendTransaction("transaction-id","user-id").then(() => {});
```

## Development

### Build

To build the package and update the changes use the command

```bash
npm install
npm run build
```

### Test

There is a package inside the repo to test the changes.

1. If you want to test the changes without uploading to npm use

    ```bash
    npm link
    ```

2. On the test_client folder run

    ```bash
    npm install
    npm run build
    ```

### Obfuscation

Before uploading the sdk to anywhere remember to obfuscate to make more complex to read the code.

We were using the https://obfuscator.io/ website
