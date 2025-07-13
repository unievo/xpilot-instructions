# mxpy multisig get-action-last-index

Perform a smart contract query to get the index of the last action.

## Usage

```bash
mxpy multisig get-action-last-index --contract CONTRACT [--abi ABI] [--proxy PROXY]
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
mxpy multisig get-action-last-index --contract msig1 --proxy https://devnet-gateway.multiversx.com
