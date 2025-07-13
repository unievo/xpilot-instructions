# mxpy multisig is-signed-by

Perform a smart contract query to check if an action is signed by a user.

## Usage

```bash
mxpy multisig is-signed-by --contract CONTRACT --action ACTION --user USER [--abi ABI] [--proxy PROXY]
```

## Parameters

- `--contract CONTRACT`  
  Bech32 address of the Multisig Smart Contract.

- `--action ACTION`  
  The id of the action.

- `--user USER`  
  Bech32 address of the user.

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy multisig is-signed-by --contract msig1 --action 42 --user erd1... --proxy https://devnet-gateway.multiversx.com
