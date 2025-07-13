# mxpy multisig get-user-role

Perform a smart contract query to get the role of a user.

## Usage

```bash
mxpy multisig get-user-role --contract CONTRACT --user USER [--abi ABI] [--proxy PROXY]
```

## Parameters

- `--contract CONTRACT`  
  Bech32 address of the Multisig Smart Contract.

- `--user USER`  
  Bech32 address of the user.

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy multisig get-user-role --contract msig1 --user erd1... --proxy https://devnet-gateway.multiversx.com
