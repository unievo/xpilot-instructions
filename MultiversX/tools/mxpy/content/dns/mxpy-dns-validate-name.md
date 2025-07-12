# mxpy dns validate-name

Asks one of the DNS contracts to validate a name. Can be useful before registering it.

## Usage

```bash
mxpy dns validate-name [name] [options]
```

## Parameters

- `name`  
  The name for which to check.
- `--shard-id SHARD_ID`  
  Shard id of the contract to call (default: 0).
- `--proxy PROXY`  
  The URL of the proxy.

## Example

```bash
mxpy dns validate-name mydomain --shard-id 0 --proxy https://devnet-api.multiversx.com
