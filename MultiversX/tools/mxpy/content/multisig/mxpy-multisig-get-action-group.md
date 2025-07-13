# mxpy multisig get-action-group

Perform a smart contract query to get the actions in a group.

## Usage

```bash
mxpy multisig get-action-group --contract CONTRACT --group GROUP [--abi ABI] [--proxy PROXY]
```

## Parameters

- `--contract CONTRACT`  
  Bech32 address of the Multisig Smart Contract.

- `--group GROUP`  
  The group id.

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy multisig get-action-group --contract msig1 --group 1 --proxy https://devnet-gateway.multiversx.com
