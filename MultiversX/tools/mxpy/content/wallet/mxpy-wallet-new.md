# mxpy wallet new

Create a new wallet and print its mnemonic; optionally save as password-protected JSON (recommended) or PEM (not recommended).

## Usage

```bash
mxpy wallet new [--format FORMAT] [--outfile OUTFILE] [--address-hrp ADDRESS_HRP] [--shard SHARD]
```

## Parameters

- `--format {raw-mnemonic,keystore-mnemonic,keystore-secret-key,pem}`  
  The format of the generated wallet file (default: None).

- `--outfile OUTFILE`  
  The output path and base file name for the generated wallet files (default: None).

- `--address-hrp ADDRESS_HRP`  
  The human-readable part of the address, when format is keystore-secret-key or pem (default: erd).

- `--shard SHARD`  
  The shard in which the address will be generated - optional (default: random).

- `-h, --help`  
  Show help message and exit.


## Rules:
- If format is not provided show all available wallet formats as options and recommend using keystore-secret-key.
- Keystore files must have a .json extension, pem files a .pem extension, raw-mnemonic files a .txt extension, append the correct extension to the outfile if not provided.
- Specify a hrp for other networks than devnet, testnet, and mainnet, you can get the information from available instructions or ask the user if not known.

## Example

Create a new wallet and save as a password-protected JSON file:

```bash
mxpy wallet new --format keystore-secret-key --outfile mywallet.json
```

Create a new PEM wallet for a specific shard:

```bash
mxpy wallet new --format pem --outfile mywallet.pem --shard 1
