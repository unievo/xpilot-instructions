# mxpy dns register

Send a register transaction to the appropriate DNS contract from given user and with given name.

## Usage

```bash
mxpy dns register [options]
```

## Parameters

- `--name NAME`  
  The name to register.

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

- `--proxy PROXY`  
  URL of the proxy.

- `--nonce NONCE`  
  Nonce for the transaction. If not provided, fetched from network.

- `--gas-price GAS_PRICE`  
  Gas price (default: 1000000000).

- `--gas-limit GAS_LIMIT`  
  Gas limit.

- `--value VALUE`  
  Value to transfer (default: 0).

- `--chain CHAIN`  
  Chain identifier.

- `--version VERSION`  
  Transaction version (default: 2).

- `--options OPTIONS`  
  Transaction options (default: 0).

- `--relayer RELAYER`  
  Bech32 address of the relayer.

- `--guardian GUARDIAN`  
  Bech32 address of the guardian.

- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  URL of the guardian service.

- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  2FA code for the guardian.

- `--guardian-pem GUARDIAN_PEM`  
  Guardian PEM file, if keyfile not provided.

- `--guardian-keyfile GUARDIAN_KEYFILE`  
  Guardian JSON keyfile, if PEM not provided.

- `--guardian-ledger`  
  Sign transaction using guardian ledger.

- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  Guardian address index (default: 0).

- `--relayer-pem RELAYER_PEM`  
  Relayer PEM file, if keyfile not provided.

- `--relayer-keyfile RELAYER_KEYFILE`  
  Relayer JSON keyfile, if PEM not provided.

- `--relayer-ledger`  
  Sign transaction using relayer ledger.

- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  Relayer address index (default: 0).

- `--outfile OUTFILE`  
  Where to save the output (default: stdout).

- `--send`  
  Broadcast the transaction (default: False).

- `--simulate`  
  Simulate the transaction (default: False).

## Example

```bash
mxpy dns register --name my_name --proxy proxy --sender alice --send
mxpy dns register --name my_name --proxy proxy --sender alice --simulate --outfile result.json
