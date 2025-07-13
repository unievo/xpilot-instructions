# mxpy get storage

Get the storage (key-value pairs) of an account.

## Usage

```bash
mxpy get storage [--alias ALIAS] [--address ADDRESS] [--proxy PROXY]
```

## Parameters

- `--alias ALIAS`  
  The alias of the wallet if configured in address config.

- `--address ADDRESS`  
  The bech32 address.

- `--proxy PROXY`  
  The proxy URL.

## Example

```bash
mxpy get storage --address erd1abc... --proxy https://devnet-gateway.multiversx.com
mxpy get storage --alias alice
