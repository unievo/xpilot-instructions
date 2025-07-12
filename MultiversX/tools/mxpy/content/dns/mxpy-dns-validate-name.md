# mxpy dns validate-name

Asks one of the DNS contracts to validate a name. Useful before registering it.

## Usage

```bash
mxpy dns validate-name name [--shard-id SHARD_ID] [--proxy PROXY]
```

## Parameters

- `name`  
  The name for which to check.

- `--shard-id SHARD_ID`  
  Shard id of the contract to call (default: 0).

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy dns validate-name my_name
mxpy dns validate-name my_name --shard-id 1 --proxy https://gateway.multiversx.com
