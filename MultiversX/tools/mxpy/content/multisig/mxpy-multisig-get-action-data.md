# mxpy multisig get-action-data

Perform a smart contract query to get the data of an action.

## Usage

```bash
mxpy multisig get-action-data --contract CONTRACT --action ACTION [--abi ABI] [--proxy PROXY]
```

## Parameters

- `--contract CONTRACT`  
  Bech32 address of the Multisig Smart Contract.

- `--action ACTION`  
  The id of the action.

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy multisig get-action-data --contract msig1 --action 42 --proxy https://devnet-gateway.multiversx.com
