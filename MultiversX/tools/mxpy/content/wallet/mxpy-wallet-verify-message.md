# mxpy wallet verify-message

Verify a previously signed message.

## Usage

```bash
mxpy wallet verify-message --address [bech32 address] --message [message] --signature [hex signature]
```

## Parameters

- `--address ADDRESS`  
  The bech32 address of the signer.

- `--message MESSAGE`  
  The previously signed message (readable text, as it was signed).

- `--signature SIGNATURE`  
  The signature in hex format.

- `-h, --help`  
  Show help message and exit.

## Example

Verify a signed message:

```bash
mxpy wallet verify-message --address erd1... --message "Hello MultiversX" --signature 012345abcdef...
