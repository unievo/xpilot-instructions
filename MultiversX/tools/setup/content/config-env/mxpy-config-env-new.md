# mxpy config-env new

Creates a new environment and sets it as the active environment.

## Usage

```bash
mxpy config-env new NAME [--template TEMPLATE]
```

## Parameters

- `NAME`  
  The name of the new environment.

- `--template TEMPLATE`  
  An environment from which to create the new environment.

## Example

```bash
mxpy config-env new devnet
mxpy config-env new testnet --template mainnet
