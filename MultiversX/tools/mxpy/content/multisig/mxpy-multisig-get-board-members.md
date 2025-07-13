# mxpy multisig get-board-members

Perform a smart contract query to get all the board members.

## Usage

```bash
mxpy multisig get-board-members --contract CONTRACT [--abi ABI] [--proxy PROXY]
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
mxpy multisig get-board-members --contract msig1 --proxy https://devnet-gateway.multiversx.com
