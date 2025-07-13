# mxpy governance get-delegated-vote-info

Get info about a delegated vote.

## Usage

```bash
mxpy governance get-delegated-vote-info --contract CONTRACT --user USER [--proxy PROXY]
```

## Parameters

- `--contract CONTRACT`  
  The bech32 address of the contract.

- `--user USER`  
  The bech32 address of the user.

- `--proxy PROXY`  
  URL of the proxy.

## Example

```bash
mxpy governance get-delegated-vote-info --contract erd1contract... --user erd1user... --proxy https://devnet-gateway.multiversx.com
