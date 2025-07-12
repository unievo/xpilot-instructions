# mxpy contract verify

Verify the authenticity of the code of a deployed Smart Contract.

## Usage

```bash
mxpy contract verify [contract address] --packaged-src [JSON file] [options]
```

## Parameters

- `contract`  
  The bech32 address of the Smart Contract.

- `--packaged-src PACKAGED_SRC`  
  JSON file containing the source code of the contract.

- `--verifier-url VERIFIER_URL`  
  The URL of the service that validates the contract.

- `--docker-image DOCKER_IMAGE`  
  The docker image used for the build.

- `--contract-variant CONTRACT_VARIANT`  
  In case of a multicontract, specify the contract variant you want to verify.

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

- `--skip-confirmation, -y`  
  Can be used to skip the confirmation prompt.

- `-h, --help`  
  Show help message and exit.

## Example

Verify a deployed contract:

```bash
mxpy contract verify erd1contractaddress... --packaged-src contract_source.json --verifier-url https://verifier.example.com
