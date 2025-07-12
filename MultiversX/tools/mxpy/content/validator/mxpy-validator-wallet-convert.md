# mxpy validator-wallet convert

Convert a validator pem file to a hex secret key.

## Usage

```bash
mxpy validator-wallet convert --infile INFILE [--index INDEX]
```

## Parameters

- `--infile INFILE`  
  (string) The pem file of the wallet.
- `--index INDEX`  
  (integer, optional) The index of the validator in case the file contains multiple validators (default: 0).

## Example

```bash
mxpy validator-wallet convert --infile validator.pem --index 0
