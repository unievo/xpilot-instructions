# mxpy config-wallet remove

Removes a wallet from the config using the alias. No default wallet will be set. Use `config-wallet switch` to set a new wallet.

## Usage

```bash
mxpy config-wallet remove [--alias ALIAS]
```

## Parameters

- `--alias ALIAS`  
  The alias of the wallet.

## Example

```bash
mxpy config-wallet remove --alias alice
