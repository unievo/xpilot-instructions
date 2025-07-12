# mxpy staking-provider redelegate-rewards

Redelegate the rewards earned for delegating.

## Usage

```bash
mxpy staking-provider redelegate-rewards [options]
```

## Parameters

- `--delegation-contract DELEGATION_CONTRACT`  
  address of the delegation contract

- `--proxy PROXY`  
  the URL of the proxy

- `--sender SENDER`  
  the alias of the wallet set in the address config

- `--pem PEM`  
  the PEM file, if keyfile not provided

- `--keyfile KEYFILE`  
  a JSON keyfile, if PEM not provided

- `--passfile PASSFILE`  
  DEPRECATED, do not use it anymore. Instead, you'll be prompted to enter the password.

- `--ledger`  
  bool flag for signing transaction using ledger

- `--sender-wallet-index SENDER_WALLET_INDEX`  
  the address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0)

- `--sender-username SENDER_USERNAME`  
  the username of the sender

- `--hrp HRP`  
  The hrp used to convert the address to its bech32 representation

- `--nonce NONCE`  
  the nonce for the transaction. If not provided, is fetched from the network.

- `--gas-price GAS_PRICE`  
  the gas price (default: 1000000000)

- `--gas-limit GAS_LIMIT`  
  the gas limit

- `--value VALUE`  
  the value to transfer (default: 0)

- `--chain CHAIN`  
  the chain identifier

- `--version VERSION`  
  the transaction version (default: 2)

- `--options OPTIONS`  
  the transaction options (default: 0)

- `--relayer RELAYER`  
  the bech32 address of the relayer

- `--guardian GUARDIAN`  
  the bech32 address of the guardian

- `--send`  
  whether to broadcast the transaction (default: False)

- `--simulate`  
  whether to simulate the transaction (default: False)

- `--outfile OUTFILE`  
  where to save the output (signed transaction, hash) (default: stdout)

- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  the url of the guardian service

- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  the 2fa code for the guardian

- `--guardian-pem GUARDIAN_PEM`  
  the PEM file, if keyfile not provided

- `--guardian-keyfile GUARDIAN_KEYFILE`  
  a JSON keyfile, if PEM not provided

- `--guardian-passfile GUARDIAN_PASSFILE`  
  DEPRECATED, do not use it anymore. Instead, you'll be prompted to enter the password.

- `--guardian-ledger`  
  bool flag for signing transaction using ledger

- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  the address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0)

- `--relayer-pem RELAYER_PEM`  
  the PEM file, if keyfile not provided

- `--relayer-keyfile RELAYER_KEYFILE`  
  a JSON keyfile, if PEM not provided

- `--relayer-passfile RELAYER_PASSFILE`  
  DEPRECATED, do not use it anymore. Instead, you'll be prompted to enter the password.

- `--relayer-ledger`  
  bool flag for signing transaction using ledger

- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  the address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0)
