# mxpy validator-wallet verify-message-signature

Verify a previously signed message.

## Usage

```bash
mxpy validator-wallet verify-message-signature --pubkey PUBKEY --message MESSAGE --signature SIGNATURE
```

## Parameters

- `--pubkey PUBKEY`  
  Hex string representing the validator's public key.

- `--message MESSAGE`  
  Previously signed message (readable text, as it was signed).

- `--signature SIGNATURE`  
  Signature in hex format.

## Example

```bash
mxpy validator-wallet verify-message-signature --pubkey abcd1234 --message "hello world" --signature deadbeef
