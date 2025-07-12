# mxpy tx relay

Relay a previously saved transaction.

## Usage

```bash
mxpy tx relay [options]
```

## Parameters

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
- `--infile INFILE`  
  Input file (a previously saved transaction).
- `--outfile OUTFILE`  
  Where to save the output (the relayer signed transaction) (default: stdout).
- `--send`  
  Whether to broadcast the transaction (default: False).
- `--simulate`  
  Whether to simulate the transaction (default: False).
- `--proxy PROXY`  
  URL of the proxy.
- `-h, --help`  
  Show help message and exit.

## Example

```bash
mxpy tx relay --relayer-pem relayer.pem --infile tx.json --send
