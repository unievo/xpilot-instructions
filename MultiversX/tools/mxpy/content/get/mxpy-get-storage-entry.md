# mxpy get storage-entry

Get a specific storage entry (key-value pair) of an account.

## Usage

```bash
mxpy get storage-entry [--alias ALIAS] [--address ADDRESS] [--proxy PROXY] --key KEY
```

## Parameters

- `--alias ALIAS`  
  The alias of the wallet if configured in address config.

- `--address ADDRESS`  
  The bech32 address.

- `--proxy PROXY`  
  The proxy URL.

- `--key KEY`  
  The storage key to read from.

## Example

```bash
mxpy get storage-entry --address erd1abc... --key myKey --proxy https://devnet-gateway.multiversx.com
mxpy get storage-entry --alias alice --key myKey
