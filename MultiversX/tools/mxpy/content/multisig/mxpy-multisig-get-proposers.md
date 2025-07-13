# mxpy multisig get-proposers

Perform a smart contract query to get all the proposers.

## Usage

```bash
mxpy multisig get-proposers --contract CONTRACT [--abi ABI] [--proxy PROXY]
```

## Parameters

- `--contract CONTRACT`  
  Bech32 address of the Multisig Smart Contract.

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy multisig get-proposers --contract msig1 --proxy https://devnet-gateway.multiversx.com
