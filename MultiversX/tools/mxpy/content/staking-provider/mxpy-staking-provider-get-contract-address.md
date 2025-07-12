# mxpy staking-provider get-contract-address

Get created contract address by transaction hash.

## Usage

```bash
mxpy staking-provider get-contract-address [options]
```

## Parameters

- `--create-tx-hash CREATE_TX_HASH`  
  String. The transaction hash.
- `--proxy PROXY`  
  String. The URL of the proxy.

## Example

```bash
mxpy staking-provider get-contract-address --create-tx-hash abcd1234... --proxy https://devnet-gateway.multiversx.com
