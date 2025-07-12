# mxpy wallet sign-message

Sign a message using a wallet.

## Usage

```bash
mxpy wallet sign-message --message [message] [--pem PEM | --keyfile KEYFILE] [options]
```

## Parameters

- `--message MESSAGE`  
  The message you want to sign.

- `--pem PEM`  
  The PEM file, if keyfile not provided.

- `--keyfile KEYFILE`  
  A JSON keyfile, if PEM not provided.

- `--passfile PASSFILE`  
  A file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.

- `--ledger`  
  Bool flag for signing transaction using ledger.

- `--sender-wallet-index SENDER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).

- `--sender-username SENDER_USERNAME`  
  The username of the sender.

- `--hrp HRP`  
  The hrp used to convert the address to its bech32 representation.

- `-h, --help`  
  Show help message and exit.

## Example

Sign a message using a PEM file:

```bash
mxpy wallet sign-message --message "Hello MultiversX" --pem wallet.pem
