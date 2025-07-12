# mxpy faucet request

Request native token funds from the faucet on Devnet, Testnet, or other networks.

## Usage

```bash
mxpy faucet request [options]
```

## Parameters

- `--pem PEM`  
  Path to the PEM file, if keyfile not provided.
- `--keyfile KEYFILE`  
  Path to a JSON keyfile, if PEM not provided.
- `--passfile PASSFILE`  
  Path to a file containing the keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--ledger`  
  Boolean flag for signing transaction using Ledger.
- `--sender-wallet-index SENDER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).
- `--sender-username SENDER_USERNAME`  
  The username of the sender.
- `--hrp HRP`  
  The HRP used to convert the address to its bech32 representation.
- `--chain {D,T}`  
  The chain identifier.
- `--api API`  
  Custom API URL for the native auth client.
- `--wallet-url WALLET_URL`  
  Custom wallet URL to call the faucet from.

## Rules:
- Make sure the bech32 address starts with the correct hrp, otherwise return an error for not using the correct wallet address or network.
- Required parameters: {`--pem` or `--keyfile` [,`--passfile`]}, {`--chain` or `--api`, `--wallet-url`}

## Example

```bash
mxpy faucet request --pem wallet.pem --chain D
```

```bash
mxpy faucet request --keyfile wallet.json --passfile wallet.txt --api https://testnet-api.multiversx.com --wallet-url https://testnet-wallet.multiversx.com
```
