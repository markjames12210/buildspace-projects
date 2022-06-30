# buildspace Solana NFT Drop Project
### Welcome 👋
To get started with this course, clone this repo and follow these commands:

1. cd into the `app` folder
2. Run `npm install` at the root of your directory
3. Run `npm run start` to start the project


🔑 Setting up a Solana keypair.

In order to get uploading, we need to set up a local Solana keypair. Note: If you've done this in the past, still follow the instructions below.

In order for us to upload the NFTs to Solana, we need to have a "local wallet" to work with in the command line. Remember, you can't talk to Solana unless you have wallet and wallet is basically a "keypair" which is public key and a private key.

This can be done by running the command below. Note: When it asks, no need to give it a passphrase, can just press enter and keep it empty.

```bash
solana-keygen new --outfile ~/.config/solana/devnet.json
```
From here, we can set this keypair as our default keypair.

```bash
solana config set --keypair ~/.config/solana/devnet.json
```

And it should say 0 SOL. We can't deploy stuff to Solana without SOL, writing data to the blockchain costs money. In this case, we're on dev net so we can just give ourselves fake SOL. Go ahead and run:

```bash
solana airdrop 2
```

To upload NFT, execute follow command:

```bash
ts-node ~/metaplex/js/packages/cli/src/candy-machine-v2-cli.ts upload -e devnet -k ~/.config/solana/devnet.json -cp config.json ./assets
```

To verfify NFT:

```bash
ts-node ~/metaplex/js/packages/cli/src/candy-machine-v2-cli.ts verify_upload -e devnet -k ~/.config/solana/devnet.json
```

To update
```bash
ts-node ~/metaplex/js/packages/cli/src/candy-machine-v2-cli.ts update_candy_machine -e devnet -k ~/.config/solana/devnet.json -cp config.json
```

To confirm this project, click follow link:

https://nft-drop-starter-project-markjames.vercel.app/