# mxpy contract query

Query a Smart Contract (call a pure function).

## Usage

```bash
mxpy contract query [contract address] --function [function] [options]
```

## Parameters

- `contract`  
  The bech32 address of the Smart Contract.

- `--abi ABI`  
  The ABI file of the Smart Contract.

- `--proxy PROXY`  
  The URL of the proxy.

- `--function FUNCTION`  
  The function to call.

- `--arguments ARGUMENTS [ARGUMENTS ...]`  
  Arguments for the contract transaction, as [number, bech32-address, ascii string, boolean] or hex-encoded.

- `--arguments-file ARGUMENTS_FILE`  
  A JSON file containing the arguments. ONLY if abi file is provided.

- `-h, --help`  
  Show help message and exit.

## Example

Query a smart contract function:

```bash
mxpy contract query {contract_address}  --proxy https://devnet-gateway.multiversx.com --function getValue  [--arguments 42]
```
