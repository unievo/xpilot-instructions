# mxpy faucet request

Request xEGLD.

## Usage

```bash
mxpy faucet request [options]
```

## Parameters

- `--sender SENDER`  
  Alias of the wallet set in the address config.

- `--pem PEM`  
  PEM file, if keyfile not provided.

- `--keyfile KEYFILE`  
  JSON keyfile, if PEM not provided.

- `--ledger`  
  Sign transaction using ledger.

- `--sender-wallet-index SENDER_WALLET_INDEX`  
  Address index for PEM/keyfile/mnemonic/Ledger (default: 0).

- `--sender-username SENDER_USERNAME`  
  Username of the sender.

- `--hrp HRP`  
  HRP used to convert address to bech32.

- `--chain {D,T}`  
  Chain identifier.

- `--api API`  
  Custom API URL for the native auth client.

- `--wallet-url WALLET_URL`  
  Custom wallet URL to call the faucet from.

## Rules:
- Make sure the bech32 address starts with the correct hrp, otherwise return a warning for hrp mismatch.
- Required parameters: {`--sender`, `--pem` or `--keyfile`}, {`--chain` or `--api`, `--wallet-url`}

## Example

```bash
mxpy faucet request --sender alice --chain D

mxpy faucet request --pem wallet.pem --chain D

mxpy faucet request --keyfile wallet.json --api https://devnet-api.multiversx.com --wallet-url https://devnet-wallet.multiversx.com
