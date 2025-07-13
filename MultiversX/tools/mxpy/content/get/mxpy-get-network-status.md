# mxpy get network-status

Get the network status.

## Usage

```bash
mxpy get network-status [--proxy PROXY] [--shard {0,1,2,4294967295}]
```

## Parameters

- `--proxy PROXY`  
  The proxy URL.

- `--shard {0,1,2,4294967295}`  
  The shard to get the status for (default: 4294967295, which is methachain).

## Example

```bash
mxpy get network-status --proxy https://devnet-gateway.multiversx.com
mxpy get network-status --shard 0 --proxy https://devnet-gateway.multiversx.com
