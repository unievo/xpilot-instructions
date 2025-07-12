# mxpy dns register

Send a register transaction to the appropriate DNS contract from given user and with given name.

## Usage

```bash
mxpy dns register [options]
```

## Parameters

- `--outfile OUTFILE`  
  Path to save the output (default: stdout).
- `--send`  
  Whether to broadcast the transaction (default: False).
- `--simulate`  
  Whether to simulate the transaction (default: False).
- `--pem PEM`  
  The PEM file, if keyfile not provided.
- `--keyfile KEYFILE`  
  A JSON keyfile, if PEM not provided.
- `--passfile PASSFILE`  
  File containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--ledger`  
  Flag for signing transaction using ledger.
- `--sender-wallet-index SENDER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).
- `--sender-username SENDER_USERNAME`  
  The username of the sender.
- `--hrp HRP`  
  The hrp used to convert the address to its bech32 representation.
- `--proxy PROXY`  
  The URL of the proxy.
- `--nonce NONCE`  
  The nonce for the transaction. If not provided, is fetched from the network.
- `--recall-nonce`  
  Whether to recall the nonce when creating the transaction (default: False). This argument is obsolete.
- `--gas-price GAS_PRICE`  
  The gas price (default: 1000000000).
- `--gas-limit GAS_LIMIT`  
  The gas limit.
- `--value VALUE`  
  The value to transfer (default: 0).
- `--chain CHAIN`  
  The chain identifier.
- `--version VERSION`  
  The transaction version (default: 2).
- `--options OPTIONS`  
  The transaction options (default: 0).
- `--relayer RELAYER`  
  The bech32 address of the relayer.
- `--guardian GUARDIAN`  
  The bech32 address of the guardian.
- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  The url of the guardian service.
- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  The 2fa code for the guardian.
- `--guardian-pem GUARDIAN_PEM`  
  The PEM file, if keyfile not provided (guardian).
- `--guardian-keyfile GUARDIAN_KEYFILE`  
  A JSON keyfile, if PEM not provided (guardian).
- `--guardian-passfile GUARDIAN_PASSFILE`  
  File containing keyfile's password, if keyfile provided (guardian). If not provided, you'll be prompted to enter the password.
- `--guardian-ledger`  
  Flag for signing transaction using ledger (guardian).
- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (guardian, default: 0).
- `--relayer-pem RELAYER_PEM`  
  The PEM file, if keyfile not provided (relayer).
- `--relayer-keyfile RELAYER_KEYFILE`  
  A JSON keyfile, if PEM not provided (relayer).
- `--relayer-passfile RELAYER_PASSFILE`  
  File containing keyfile's password, if keyfile provided (relayer). If not provided, you'll be prompted to enter the password.
- `--relayer-ledger`  
  Flag for signing transaction using ledger (relayer).
- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (relayer, default: 0).
- `--name NAME`  
  The name to register.

## Example

```bash
mxpy dns register --pem user.pem --name mydomain --send
