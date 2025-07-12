# mxpy contract deploy

Deploy a Smart Contract.

## Usage

```bash
mxpy contract deploy --bytecode BYTECODE --abi ABI [options]
```

## Parameters

- `--bytecode BYTECODE`  
  The file containing the WASM bytecode.

- `--abi ABI`  
  The ABI file of the Smart Contract.

- `--metadata-not-upgradeable`  
  Mark the contract as NOT upgradeable (default: upgradeable).

- `--metadata-not-readable`  
  Mark the contract as NOT readable (default: readable).

- `--metadata-payable`  
  Mark the contract as payable (default: not payable).

- `--metadata-payable-by-sc`  
  Mark the contract as payable by SC (default: not payable by SC).

- `--outfile OUTFILE`  
  Where to save the output (default: stdout).

- `--sender SENDER`  
  The alias of the wallet set in the address config.

- `--pem PEM`  
  The PEM file, if keyfile not provided.

- `--keyfile KEYFILE`  
  A JSON keyfile, if PEM not provided.

- `--passfile PASSFILE`  
  DEPRECATED. Do not use. You'll be prompted to enter the password.

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
  DEPRECATED. Do not use. You'll be prompted to enter the password.

- `--guardian-ledger`  
  Bool flag for signing transaction using ledger.

- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).

- `--relayer-pem RELAYER_PEM`  
  The PEM file, if keyfile not provided.

- `--relayer-keyfile RELAYER_KEYFILE`  
  A JSON keyfile, if PEM not provided.

- `--relayer-passfile RELAYER_PASSFILE`  
  DEPRECATED. Do not use. You'll be prompted to enter the password.

- `--relayer-ledger`  
  Bool flag for signing transaction using ledger.

- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  The address index; can be used for PEM files, keyfiles of type mnemonic or Ledger devices (default: 0).

- `-h, --help`  
  Show help message and exit.

## Rules:
- BYTECODE (must be the full path of the file {CONTRACT-NAME}.wasm, found in the "output" folder from the contract folder. If the file does not exist, build the contract first.) 
- ABI (must be the full path of the file {CONTRACT-NAME}.abi.json and it is found in the "output" folder from the contract folder. If the file does not exist, build the contract first.)
- Important: Before deployment, read the contract file that contains the #[multiversx_sc::contract] annotation to determine if the contract has init arguments in the "init" function. If init arguments not known, ask for their values and specify them in --arguments.
- Use --simulate with --gas-limit=600000000 to obtain an estimation of the gas limit (look for "txGasUnits": in the simulation "cost" result)
- If the transaction fails with not enough gas error, and already used --simulate to have an estimation for the gas limit, use a 2X on the last used gas limit. 
- Successful deployment response should have a "status": "success" transaction and a log entry with an "identifier": "SCDeploy" section. 
- After initial deployment, the contract can only be upgraded to the same address, deploying again would create a new contract instance with a new address. 
- If necessary to upgrade the contract after first deployment, use the upgrade command. 

## Example

Deploy a contract with bytecode and ABI:

```bash
mxpy contract deploy --bytecode mycontract.wasm --abi mycontract.abi.json --pem wallet.pem --proxy https://devnet-gateway.multiversx.com --gas-limit 50000000 --send --wait-result
```

