# mxpy multisig get-pending-actions

Perform a smart contract query to get the pending actions full info.

## Usage

```bash
mxpy multisig get-pending-actions --contract CONTRACT [--abi ABI] [--proxy PROXY]
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
mxpy multisig get-pending-actions --contract msig1 --proxy https://devnet-gateway.multiversx.com
