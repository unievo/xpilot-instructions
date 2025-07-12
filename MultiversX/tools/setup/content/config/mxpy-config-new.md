# mxpy config new

Creates a new configuration and sets it as the active configuration.

## Usage

```bash
mxpy config new name [--template TEMPLATE]
```

## Parameters

- `name`  
  The name of the configuration entry.

- `--template TEMPLATE`  
  Template from which to create the new config.

## Example

```bash
mxpy config new devnet
mxpy config new testnet --template default
