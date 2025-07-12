# mxpy dns version

Asks the contract for its version.

## Usage

```bash
mxpy dns version [options]
```

## Parameters

- `--shard-id SHARD_ID`  
  Shard id of the contract to call (default: 0).
- `--all`  
  Prints a list of all DNS contracts and their current versions (default: False).
- `--proxy PROXY`  
  The URL of the proxy.

## Example

```bash
mxpy dns version --all --proxy https://devnet-api.multiversx.com
