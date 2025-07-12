# mxpy validator-wallet verify-message-signature

Verify a previously signed message.

## Usage

```bash
mxpy validator-wallet verify-message-signature --pubkey PUBKEY --message MESSAGE --signature SIGNATURE
```

## Parameters

- `--pubkey PUBKEY`  
  (string) The hex string representing the validator's public key.
- `--message MESSAGE`  
  (string) The previously signed message (readable text, as it was signed).
- `--signature SIGNATURE`  
  (string) The signature in hex format.

## Example

```bash
mxpy validator-wallet verify-message-signature --pubkey 0123abcd... --message "hello" --signature 89ef...
