# mxpy validator-wallet convert

Convert a validator pem file to a hex secret key.

## Usage

```bash
mxpy validator-wallet convert --infile INFILE [--index INDEX]
```

## Parameters

- `--infile INFILE`  
  PEM file of the wallet.

- `--index INDEX`  
  Index of the validator if the file contains multiple validators (default: 0).

## Example

```bash
mxpy validator-wallet convert --infile validator.pem
mxpy validator-wallet convert --infile validator.pem --index 1
