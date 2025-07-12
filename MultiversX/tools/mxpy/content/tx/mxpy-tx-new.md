# mxpy tx new

Create a new transaction.

## Usage

```bash
mxpy tx new [options]
```

## Parameters

- `--sender SENDER`  
  The alias of the wallet set in the address config.
- `--pem PEM`  
  Path to the PEM file, if keyfile not provided.
- `--keyfile KEYFILE`  
  Path to a JSON keyfile, if PEM not provided.
- `--passfile PASSFILE`  
  DEPRECATED. Do not use. You'll be prompted to enter the password.
- `--ledger`  
  Boolean flag for signing transaction using Ledger.
- `--sender-wallet-index SENDER_WALLET_INDEX`  
  Address index for PEM files, mnemonic keyfiles, or Ledger devices (default: 0).
- `--sender-username SENDER_USERNAME`  
  Username of the sender.
- `--hrp HRP`  
  HRP used to convert the address to its bech32 representation.
- `--nonce NONCE`  
  Nonce for the transaction. If not provided, fetched from the network.
- `--receiver RECEIVER`  
  Address of the receiver.
- `--receiver-username RECEIVER_USERNAME`  
  Username of the receiver.
- `--gas-price GAS_PRICE`  
  Gas price (default: 1000000000).
- `--gas-limit GAS_LIMIT`  
  Gas limit.
- `--value VALUE`  
  Value to transfer (default: 0).
- `--data DATA`  
  Payload or memo of the transaction (default: empty).
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
- `--data-file DATA_FILE`  
  Path to a file containing transaction data.
- `--token-transfers TOKEN_TRANSFERS [TOKEN_TRANSFERS ...]`  
  Token transfers for transfer & execute, as [token, amount].  
  Example: `--token-transfers NFT-123456-0a 1 ESDT-987654 100000000`
- `--outfile OUTFILE`  
  Where to save the output (signed transaction, hash) (default: stdout).
- `--send`  
  Whether to broadcast the transaction (default: False).
- `--simulate`  
  Whether to simulate the transaction (default: False).
- `--proxy PROXY`  
  URL of the proxy.
- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  URL of the guardian service.
- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  2FA code for the guardian.
- `--guardian-pem GUARDIAN_PEM`  
  PEM file for guardian, if keyfile not provided.
- `--guardian-keyfile GUARDIAN_KEYFILE`  
  JSON keyfile for guardian, if PEM not provided.
- `--guardian-passfile GUARDIAN_PASSFILE`  
  DEPRECATED. Do not use. You'll be prompted to enter the password.
- `--guardian-ledger`  
  Boolean flag for signing transaction using Ledger (guardian).
- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  Address index for guardian PEM files, mnemonic keyfiles, or Ledger devices (default: 0).
- `--relayer-pem RELAYER_PEM`  
  PEM file for relayer, if keyfile not provided.
- `--relayer-keyfile RELAYER_KEYFILE`  
  JSON keyfile for relayer, if PEM not provided.
- `--relayer-passfile RELAYER_PASSFILE`  
  DEPRECATED. Do not use. You'll be prompted to enter the password.
- `--relayer-ledger`  
  Boolean flag for signing transaction using Ledger (relayer).
- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  Address index for relayer PEM files, mnemonic keyfiles, or Ledger devices (default: 0).
- `--wait-result`  
  Wait for the transaction result. Only valid if --send is set.
- `--timeout TIMEOUT`  
  Max seconds to wait for result. Only valid if --wait-result is set.
- `-h, --help`  
  Show help message and exit.

## Rules:
- Start with 50000 gas limit for simple value transfer transactions.
- For more complex transactions (such as smart contract operations) use --simulate with --gas-limit=600000000 to obtain an estimation of the gas limit (look for "txGasUnits" in the simulation "cost" result).

## Example

```bash
mxpy tx new --pem alice.pem --receiver address --value 1000000000000000000 --chain D --send --wait-result
```

```bash
mxpy tx new --keyfile bob.json --passfile password.txt --receiver address --value 1000000000000000000 --proxy https://testnet-gateway.multiversx.com --send --wait-result
```