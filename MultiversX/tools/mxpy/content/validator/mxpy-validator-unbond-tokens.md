# mxpy validator unbond-tokens

It will unBond tokens, if provided value is bigger than topUp value will unBond nodes.

## Usage

```bash
mxpy validator unbond-tokens [options]
```

## Parameters

- `--proxy PROXY`  
  string, the URL of the proxy
- `--pem PEM`  
  string, the PEM file, if keyfile not provided
- `--keyfile KEYFILE`  
  string, a JSON keyfile, if PEM not provided
- `--passfile PASSFILE`  
  string, a file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--ledger`  
  bool, flag for signing transaction using ledger
- `--sender-wallet-index SENDER_WALLET_INDEX`  
  int, the address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0)
- `--sender-username SENDER_USERNAME`  
  string, the username of the sender
- `--hrp HRP`  
  string, the hrp used to convert the address to its bech32 representation
- `--nonce NONCE`  
  int, the nonce for the transaction. If not provided, is fetched from the network.
- `--recall-nonce`  
  bool, whether to recall the nonce when creating the transaction (OBSOLETE)
- `--gas-price GAS_PRICE`  
  int, the gas price (default: 1000000000)
- `--gas-limit GAS_LIMIT`  
  int, the gas limit
- `--value VALUE`  
  int, the value to transfer (default: 0)
- `--chain CHAIN`  
  string, the chain identifier
- `--version VERSION`  
  int, the transaction version (default: 2)
- `--options OPTIONS`  
  int, the transaction options (default: 0)
- `--relayer RELAYER`  
  string, the bech32 address of the relayer
- `--guardian GUARDIAN`  
  string, the bech32 address of the guardian
- `--send`  
  bool, whether to broadcast the transaction (default: False)
- `--simulate`  
  bool, whether to simulate the transaction (default: False)
- `--outfile OUTFILE`  
  string, where to save the output (signed transaction, hash) (default: stdout)
- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  string, the url of the guardian service
- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  string, the 2fa code for the guardian
- `--guardian-pem GUARDIAN_PEM`  
  string, the PEM file, if keyfile not provided
- `--guardian-keyfile GUARDIAN_KEYFILE`  
  string, a JSON keyfile, if PEM not provided
- `--guardian-passfile GUARDIAN_PASSFILE`  
  string, a file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--guardian-ledger`  
  bool, flag for signing transaction using ledger
- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  int, the address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0)
- `--relayer-pem RELAYER_PEM`  
  string, the PEM file, if keyfile not provided
- `--relayer-keyfile RELAYER_KEYFILE`  
  string, a JSON keyfile, if PEM not provided
- `--relayer-passfile RELAYER_PASSFILE`  
  string, a file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--relayer-ledger`  
  bool, flag for signing transaction using ledger
- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  int, the address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0)
- `--unbond-value UNBOND_VALUE`  
  int, the unbond value

## Example

```bash
mxpy validator unbond-tokens --proxy https://gateway.example.com --pem wallet.pem --unbond-value 1000000000000000000 --send
