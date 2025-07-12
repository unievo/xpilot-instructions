# mxpy contract unverify

Unverify a previously verified Smart Contract.

## Usage

```bash
mxpy contract unverify [contract address] --code-hash [hash] [options]
```

## Parameters

- `contract`  
  The bech32 address of the Smart Contract.

- `--code-hash CODE_HASH`  
  The code hash of the contract.

- `--verifier-url VERIFIER_URL`  
  The URL of the service that validates the contract.

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

Unverify a deployed contract:

```bash
mxpy contract unverify erd1contractaddress... --code-hash abcd1234 --verifier-url https://verifier.example.com
