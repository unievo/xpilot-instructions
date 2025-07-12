# mxpy tx send

Send a previously saved transaction.

## Usage

```bash
mxpy tx send [options]
```

## Parameters

- `--infile INFILE`  
  Input file (a previously saved transaction).
- `--outfile OUTFILE`  
  Where to save the output (the hash) (default: stdout).
- `--proxy PROXY`  
  URL of the proxy.
- `-h, --help`  
  Show help message and exit.

## Example

```bash
mxpy tx send --infile tx.json --proxy https://devnet-gateway.multiversx.com
```
