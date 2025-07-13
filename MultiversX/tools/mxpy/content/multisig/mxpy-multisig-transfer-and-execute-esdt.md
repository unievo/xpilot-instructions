# mxpy multisig transfer-and-execute-esdt

Propose transferring ESDTs and optionally calling a smart contract.

## Usage

```bash
mxpy multisig transfer-and-execute-esdt --contract CONTRACT [--token-transfers TOKEN_TRANSFERS ...] [--receiver RECEIVER] [--function FUNCTION] [--arguments ARGUMENTS ...] [options]
```

## Parameters

- `--contract CONTRACT`  
  Bech32 address of the Multisig Smart Contract.

- `--token-transfers TOKEN_TRANSFERS [TOKEN_TRANSFERS ...]`  
  Token transfers for transfer & execute, as [token, amount].  
  E.g. --token-transfers NFT-123456-0a 1 ESDT-987654 100000000

- `--receiver RECEIVER`  
  Address of the receiver.

- `--function FUNCTION`  
  Function to call.

- `--arguments ARGUMENTS [ARGUMENTS ...]`  
  Arguments for the contract transaction, as [number, bech32-address, ascii string, boolean] or hex-encoded.  
  E.g. --arguments 42 0x64 1000 0xabba str:TOK-a1c2ef true addr:erd1[..]

- `--arguments-file ARGUMENTS_FILE`  
  JSON file containing the arguments. ONLY if abi file is provided.  
  E.g. [{ 'to': 'erd1...', 'amount': 10000000000 }]

- `--contract-abi CONTRACT_ABI`  
  ABI file of the contract to call.

- `--opt-gas-limit OPT_GAS_LIMIT`  
  Optional gas limit for the async call.

- `--abi ABI`  
  ABI file of the Multisig Smart Contract.

- `--outfile OUTFILE`  
  Where to save the output (default: stdout).

- `--sender SENDER`  
  Alias of the wallet set in the address config.

- `--pem PEM`  
  PEM file, if keyfile not provided.

- `--keyfile KEYFILE`  
  JSON keyfile, if PEM not provided.

- `--ledger`  
  Sign transaction using ledger.

- `--sender-wallet-index SENDER_WALLET_INDEX`  
  Address index for PEM/keyfile/mnemonic/Ledger (default: 0).

- `--sender-username SENDER_USERNAME`  
  Username of the sender.

- `--hrp HRP`  
  HRP used to convert address to bech32.

- `--proxy PROXY`  
  URL of the proxy.

- `--nonce NONCE`  
  Nonce for the transaction. If not provided, fetched from network.

- `--gas-price GAS_PRICE`  
  Gas price (default: 1000000000).

- `--gas-limit GAS_LIMIT`  
  Gas limit.

- `--value VALUE`  
  Value to transfer (default: 0).

- `--chain CHAIN`  
  Chain identifier.

- `--version VERSION`  
  Transaction version (default: 2).

- `--options OPTIONS`  
  Transaction options (default: 0).

- `--relayer RELAYER`  
  Bech32 address of the relayer.

- `--guardian GUARDIAN`  
  Bech32 address of the guardian.

- `--send`  
  Broadcast the transaction (default: False).

- `--simulate`  
  Simulate the transaction (default: False).

- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  URL of the guardian service.

- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  2FA code for the guardian.

- `--guardian-pem GUARDIAN_PEM`  
  Guardian PEM file, if keyfile not provided.

- `--guardian-keyfile GUARDIAN_KEYFILE`  
  Guardian JSON keyfile, if PEM not provided.

- `--guardian-ledger`  
  Sign transaction using guardian ledger.

- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  Guardian address index (default: 0).

- `--relayer-pem RELAYER_PEM`  
  Relayer PEM file, if keyfile not provided.

- `--relayer-keyfile RELAYER_KEYFILE`  
  Relayer JSON keyfile, if PEM not provided.

- `--relayer-ledger`  
  Sign transaction using relayer ledger.

- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  Relayer address index (default: 0).

- `--wait-result`  
  Wait for the transaction result (only valid if --send is set).

- `--timeout TIMEOUT`  
  Max seconds to wait for result (only valid if --wait-result is set).

## Example

```bash
mxpy multisig transfer-and-execute-esdt --contract msig1 --token-transfers ESDT-987654 1000 --receiver erd1... --function transferFunds --arguments 1000 --sender alice --send
