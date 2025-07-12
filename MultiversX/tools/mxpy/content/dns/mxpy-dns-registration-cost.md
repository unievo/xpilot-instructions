# mxpy dns registration-cost

Gets the registration cost from a DNS smart contract, by default the one with shard id 0.

## Usage

```bash
mxpy dns registration-cost [options]
```

## Parameters

- `--shard-id SHARD_ID`  
  Shard id of the contract to call (default: 0).
- `--proxy PROXY`  
  The URL of the proxy.

## Example

```bash
mxpy dns registration-cost --shard-id 0 --proxy https://devnet-api.multiversx.com
