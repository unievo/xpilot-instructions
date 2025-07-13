# mxpy multisig parse-propose-action

Parses the propose action transaction to extract proposal ID.

## Usage

```bash
mxpy multisig parse-propose-action --abi ABI --hash HASH [--proxy PROXY]
```

## Parameters

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--hash HASH`  
  The transaction hash of the propose action.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy multisig parse-propose-action --abi multisig.abi.json --hash 0xabcdef123456 --proxy https://devnet-gateway.multiversx.com
