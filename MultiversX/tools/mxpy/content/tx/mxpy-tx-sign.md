# mxpy tx sign

Sign a previously saved transaction.

## Usage

```bash
mxpy tx sign [options]
```

## Parameters

- `--pem PEM`  
  Path to the PEM file, if keyfile not provided.
- `--keyfile KEYFILE`  
  Path to a JSON keyfile, if PEM not provided.
- `--passfile PASSFILE`  
  Path to a file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--ledger`  
  Boolean flag for signing transaction using Ledger.
- `--sender-wallet-index SENDER_WALLET_INDEX`  
  Address index for PEM files, mnemonic keyfiles, or Ledger devices (default: 0).
- `--sender-username SENDER_USERNAME`  
  Username of the sender.
- `--hrp HRP`  
  HRP used to convert the address to its bech32 representation.
- `--infile INFILE`  
  Input file (a previously saved transaction).
- `--outfile OUTFILE`  
  Where to save the output (the signed transaction) (default: stdout).
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
  File containing guardian keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--guardian-ledger`  
  Boolean flag for signing transaction using Ledger (guardian).
- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  Address index for guardian PEM files, mnemonic keyfiles, or Ledger devices (default: 0).
- `--relayer-pem RELAYER_PEM`  
  PEM file for relayer, if keyfile not provided.
- `--relayer-keyfile RELAYER_KEYFILE`  
  JSON keyfile for relayer, if PEM not provided.
- `--relayer-passfile RELAYER_PASSFILE`  
  File containing relayer keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.
- `--relayer-ledger`  
  Boolean flag for signing transaction using Ledger (relayer).
- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  Address index for relayer PEM files, mnemonic keyfiles, or Ledger devices (default: 0).
- `-h, --help`  
  Show help message and exit.

## Example

```bash
mxpy tx sign --pem alice.pem --infile tx.json --outfile signed-tx.json
