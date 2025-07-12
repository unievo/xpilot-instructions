# mxpy contract upgrade

Upgrade a previously-deployed Smart Contract.

## Usage

```bash
mxpy contract upgrade [contract address] --bytecode [WASM file] [options]
```

## Parameters

- `contract`  
  The bech32 address of the Smart Contract.

- `--abi ABI`  
  The ABI file of the Smart Contract.

- `--outfile OUTFILE`  
  Where to save the output (default: stdout).

- `--bytecode BYTECODE`  
  The file containing the WASM bytecode.

- `--metadata-not-upgradeable`  
  Mark the contract as NOT upgradeable (default: upgradeable).

- `--metadata-not-readable`  
  Mark the contract as NOT readable (default: readable).

- `--metadata-payable`  
  Mark the contract as payable (default: not payable).

- `--metadata-payable-by-sc`  
  Mark the contract as payable by SC (default: not payable by SC).

- `--pem PEM`  
  The PEM file, if keyfile not provided.

- `--keyfile KEYFILE`  
  A JSON keyfile, if PEM not provided.

- `--passfile PASSFILE`  
  A file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.

- `--ledger`  
  Bool flag for signing transaction using ledger.

- `--sender-wallet-index SENDER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).

- `--sender-username SENDER_USERNAME`  
  The username of the sender.

- `--hrp HRP`  
  The hrp used to convert the address to its bech32 representation.

- `--proxy PROXY`  
  The URL of the proxy.

- `--nonce NONCE`  
  The nonce for the transaction. If not provided, is fetched from the network.

- `--recall-nonce`  
  Whether to recall the nonce when creating the transaction (OBSOLETE).

- `--gas-price GAS_PRICE`  
  The gas price (default: 1000000000).

- `--gas-limit GAS_LIMIT`  
  The gas limit.

- `--value VALUE`  
  The value to transfer (default: 0).

- `--chain CHAIN`  
  The chain identifier.

- `--version VERSION`  
  The transaction version (default: 2).

- `--options OPTIONS`  
  The transaction options (default: 0).

- `--relayer RELAYER`  
  The bech32 address of the relayer.

- `--guardian GUARDIAN`  
  The bech32 address of the guardian.

- `--arguments ARGUMENTS [ARGUMENTS ...]`  
  Arguments for the contract transaction, as [number, bech32-address, ascii string, boolean] or hex-encoded.

- `--arguments-file ARGUMENTS_FILE`  
  A JSON file containing the arguments. ONLY if abi file is provided.

- `--wait-result`  
  Signal to wait for the transaction result - only valid if --send is set.

- `--timeout TIMEOUT`  
  Max num of seconds to wait for result - only valid if --wait-result is set.

- `--send`  
  Whether to broadcast the transaction (default: False).

- `--simulate`  
  Whether to simulate the transaction (default: False).

- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  The url of the guardian service.

- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  The 2fa code for the guardian.

- `--guardian-pem GUARDIAN_PEM`  
  The PEM file, if keyfile not provided.

- `--guardian-keyfile GUARDIAN_KEYFILE`  
  A JSON keyfile, if PEM not provided.

- `--guardian-passfile GUARDIAN_PASSFILE`  
  A file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.

- `--guardian-ledger`  
  Bool flag for signing transaction using ledger.

- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).

- `--relayer-pem RELAYER_PEM`  
  The PEM file, if keyfile not provided.

- `--relayer-keyfile RELAYER_KEYFILE`  
  A JSON keyfile, if PEM not provided.

- `--relayer-passfile RELAYER_PASSFILE`  
  A file containing keyfile's password, if keyfile provided. If not provided, you'll be prompted to enter the password.

- `--relayer-ledger`  
  Bool flag for signing transaction using ledger.

- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).

- `-h, --help`  
  Show help message and exit.

## Rules:
- Before upgrading read the contract file that contains the #[multiversx_sc::contract] annotation to determine if the contract has init arguments in the "init" function. If init arguments not known, ask for their values and specify them in --arguments.
- Use --simulate with --gas-limit=600000000 to obtain an estimation of the gas limit (look for "txGasUnits": in the simulation "cost" result)
- Successful upgrade response should have a "status": "success" transaction and a log entry with an "identifier": "SCUpgrade" section.
- Even though the transaction state can be successful, the upgrade might still fail due to other reasons, look for "identifier": "internalVMErrors" in the response for failed upgrades.
- If the transaction fails with not enough gas error, and already used --simulate to have an estimation for the gas limit, use a 2X on the last used gas limit.


## Example

Upgrade a contract with new bytecode:

```bash
mxpy contract upgrade {contract_address} --bytecode newcontract.wasm --pem wallet.pem --proxy https://devnet-gateway.multiversx.com --gas-limit 50000000 --send --wait-result

