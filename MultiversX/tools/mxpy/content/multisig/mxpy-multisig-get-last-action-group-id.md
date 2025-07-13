# mxpy multisig get-last-action-group-id

Perform a smart contract query to get the id of the last action in a group.

## Usage

```bash
mxpy multisig get-last-action-group-id --contract CONTRACT [--abi ABI] [--proxy PROXY]
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
mxpy multisig get-last-action-group-id --contract msig1 --proxy https://devnet-gateway.multiversx.com
