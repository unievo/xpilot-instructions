# mxpy get token

Get a token of an account.

## Usage

```bash
mxpy get token [--alias ALIAS] [--address ADDRESS] [--proxy PROXY] --identifier IDENTIFIER
```

## Parameters

- `--alias ALIAS`  
  The alias of the wallet if configured in address config.

- `--address ADDRESS`  
  The bech32 address.

- `--proxy PROXY`  
  The proxy URL.

- `--identifier IDENTIFIER`  
  The token identifier. Works for ESDT and NFT. (e.g. FNG-123456, NFT-987654-0a)

## Example

```bash
mxpy get token --address erd1abc... --identifier FNG-123456 --proxy https://devnet-gateway.multiversx.com
mxpy get token --alias alice --identifier NFT-987654-0a
