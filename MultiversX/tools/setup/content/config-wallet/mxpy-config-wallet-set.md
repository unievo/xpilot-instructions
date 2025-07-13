# mxpy config-wallet set

Sets a config value for the specified wallet.

## Usage

```bash
mxpy config-wallet set key value [--alias ALIAS]
```

## Parameters

- `key`  
  The key to set for the specified wallet (e.g. index).

- `value`  
  The value to set for the specified key.

- `--alias ALIAS`  
  The alias of the wallet.

## Example

```bash
mxpy config-wallet set index 0 --alias alice
