# mxpy get account

Get info about an account.

## Usage

```bash
mxpy get account [--alias ALIAS] [--address ADDRESS] [--proxy PROXY] [--balance]
```

## Parameters

- `--alias ALIAS`  
  The alias of the wallet if configured in address config.

- `--address ADDRESS`  
  The bech32 address.

- `--proxy PROXY`  
  The proxy URL.

- `--balance`  
  Whether to only fetch the balance of the address.

## Example

```bash
mxpy get account --address erd1abc... --proxy https://devnet-gateway.multiversx.com
mxpy get account --alias alice --balance
