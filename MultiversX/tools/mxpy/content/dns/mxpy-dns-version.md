# mxpy dns version

Asks the contract for its version.

## Usage

```bash
mxpy dns version [--shard-id SHARD_ID] [--all] --proxy PROXY
```

## Parameters

- `--shard-id SHARD_ID`  
  Shard id of the contract to call (default: 0).

- `--all`  
  Prints a list of all DNS contracts and their current versions (default: False).

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy dns version --proxy https://gateway.multiversx.com
