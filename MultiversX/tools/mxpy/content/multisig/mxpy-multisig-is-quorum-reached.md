# mxpy multisig is-quorum-reached

Perform a smart contract query to check if an action has reached quorum.

## Usage

```bash
mxpy multisig is-quorum-reached --contract CONTRACT --action ACTION [--abi ABI] [--proxy PROXY]
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
mxpy multisig is-quorum-reached --contract msig1 --action 42 --proxy https://devnet-gateway.multiversx.com
