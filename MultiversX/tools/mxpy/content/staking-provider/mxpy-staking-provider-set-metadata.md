# mxpy staking-provider set-metadata

Set metadata for a delegation contract. Must be called by the contract owner.

## Usage

```bash
mxpy staking-provider set-metadata [options]
```

## Parameters

- `--name NAME`  
  String. Name field in staking provider metadata.
- `--website WEBSITE`  
  String. Website field in staking provider metadata.
- `--identifier IDENTIFIER`  
  String. Identifier field in staking provider metadata.
- `--delegation-contract DELEGATION_CONTRACT`  
  String. Address of the delegation contract.
- `--proxy PROXY`  
  String. The URL of the proxy.
- `--pem PEM`  
  String. The PEM file, if keyfile not provided.
- `--keyfile KEYFILE`  
  String. A JSON keyfile, if PEM not provided.
- `--passfile PASSFILE`  
  String. File containing keyfile's password, if keyfile provided.
- `--ledger`  
  Flag. Sign transaction using ledger.
- `--sender-wallet-index SENDER_WALLET_INDEX`  
  Integer. Address index for PEM, mnemonic keyfiles, or Ledger (default: 0).
- `--sender-username SENDER_USERNAME`  
  String. Username of the sender.
- `--hrp HRP`  
  String. HRP used for bech32 address.
- `--nonce NONCE`  
  Integer. Nonce for the transaction. If not provided, fetched from network.
- `--recall-nonce`  
  Flag. Obsolete. Whether to recall the nonce when creating the transaction.
- `--gas-price GAS_PRICE`  
  Integer. Gas price (default: 1000000000).
- `--gas-limit GAS_LIMIT`  
  Integer. Gas limit.
- `--value VALUE`  
  Integer. Value to transfer (default: 0).
- `--chain CHAIN`  
  String. Chain identifier.
- `--version VERSION`  
  Integer. Transaction version (default: 2).
- `--options OPTIONS`  
  Integer. Transaction options (default: 0).
- `--relayer RELAYER`  
  String. Bech32 address of the relayer.
- `--guardian GUARDIAN`  
  String. Bech32 address of the guardian.
- `--send`  
  Flag. Broadcast the transaction (default: False).
- `--simulate`  
  Flag. Simulate the transaction (default: False).
- `--outfile OUTFILE`  
  String. Where to save the output (default: stdout).
- `--guardian-service-url GUARDIAN_SERVICE_URL`  
  String. URL of the guardian service.
- `--guardian-2fa-code GUARDIAN_2FA_CODE`  
  String. 2FA code for the guardian.
- `--guardian-pem GUARDIAN_PEM`  
  String. Guardian PEM file, if keyfile not provided.
- `--guardian-keyfile GUARDIAN_KEYFILE`  
  String. Guardian JSON keyfile, if PEM not provided.
- `--guardian-passfile GUARDIAN_PASSFILE`  
  String. File containing guardian keyfile's password.
- `--guardian-ledger`  
  Flag. Sign transaction using ledger for guardian.
- `--guardian-wallet-index GUARDIAN_WALLET_INDEX`  
  Integer. Address index for guardian PEM, mnemonic keyfiles, or Ledger (default: 0).
- `--relayer-pem RELAYER_PEM`  
  String. Relayer PEM file, if keyfile not provided.
- `--relayer-keyfile RELAYER_KEYFILE`  
  String. Relayer JSON keyfile, if PEM not provided.
- `--relayer-passfile RELAYER_PASSFILE`  
  String. File containing relayer keyfile's password.
- `--relayer-ledger`  
  Flag. Sign transaction using ledger for relayer.
- `--relayer-wallet-index RELAYER_WALLET_INDEX`  
  Integer. Address index for relayer PEM, mnemonic keyfiles, or Ledger (default: 0).

## Example

```bash
mxpy staking-provider set-metadata --name "ProviderName" --website "https://provider.com" --identifier "provider-id" --delegation-contract erd1... --proxy https://devnet-gateway.multiversx.com --pem owner.pem --send
