# buildspace Store on Solana Pay Project

[Reference Link](https://buildspace.so/p/build-solana-pay-store)

### **👝 Add 'Connect Wallet' button**

```
import { WalletMultiButton } from '@solana/wallet-adapter-react-ui';

<WalletMultiButton className="cta-button connect-wallet-button" />
```

### **🌐 Fetching items from the back room (IPFS)**

Using [Pinata](https://www.pinata.cloud/?utm_source=buildspace?utm_source=buildspace.so&utm_medium=buildspace_project)

products.json

```
[
  {
    "id": 1,
    "name": "OG Emoji pack",
    "price": "0.09",
    "description": "Get this fire emoji pack for only $0.09! Includes 3 hot emojis: Forreal, Flooshed, and Sheesh!",
    "image_url": "https://i.imgur.com/rVD8bjt.png",
    "filename": "Emojis.zip",
    "hash": "QmWWH69mTL66r3H8P4wUn24t1L5pvdTJGUTKBqT11KCHS5"
  }
]
```

The main fields we care about are the id, name, and price fields.

### **🥺 Get paid in SOL tokens**

1. Generate a transaction object on the server

2. Fetch the transaction object from the server

3. Ask the user to sign the transactions

4. Check if the transaction has been confirmed

### **🥺 Get paid in USDC**

First, head over to this [faucet](https://spl-token-faucet.com/?token-name=USDC?utm_source=buildspace.so&utm_medium=buildspace_project) to request some USDC tokens

### **💳 Turn transactions to payments**


### **💾 Read from our database**

### **🛒 Add items via your app**

### **🎓 Finishing touches**

The mainnet USDC SPL token address is EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v

