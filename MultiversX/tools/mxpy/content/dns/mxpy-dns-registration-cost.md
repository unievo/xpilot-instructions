# mxpy dns registration-cost

Gets the registration cost from a DNS smart contract, by default the one with shard id 0.

## Usage

```bash
mxpy dns registration-cost [--shard-id SHARD_ID] --proxy PROXY
```

## Parameters

- `--shard-id SHARD_ID`  
  Shard id of the contract to call (default: 0).

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy dns registration-cost --proxy https://gateway.multiversx.com
