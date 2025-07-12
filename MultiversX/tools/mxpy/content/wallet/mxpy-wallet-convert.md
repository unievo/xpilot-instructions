# mxpy wallet convert

Convert a wallet from one format to another.

## Usage

```bash
mxpy wallet convert --infile [input file] --outfile [output file] --in-format [input format] --out-format [output format] [options]
```

## Parameters

- `--infile INFILE`  
  Path to the input file.

- `--outfile OUTFILE`  
  Path to the output file.

- `--in-format {raw-mnemonic,keystore-mnemonic,keystore-secret-key,pem}`  
  The format of the input file.

- `--out-format {raw-mnemonic,keystore-mnemonic,keystore-secret-key,pem,address-bech32,address-hex,secret-key}`  
  The format of the output file.

- `--address-index ADDRESS_INDEX`  
  The address index, if input format is raw-mnemonic, keystore-mnemonic or pem (with multiple entries) and the output format is keystore-secret-key or pem.

- `--address-hrp ADDRESS_HRP`  
  The human-readable part of the address, when the output format is keystore-secret-key or pem (default: erd).

- `-h, --help`  
  Show help message and exit.

## Example

Convert a PEM file to a bech32 address:

```bash
mxpy wallet convert --infile wallet.pem --in-format pem --out-format address-bech32 --outfile address.txt
