# mxpy validator-wallet sign-message

Sign a message.

## Usage

```bash
mxpy validator-wallet sign-message --message MESSAGE --pem PEM [--index INDEX]
```

## Parameters

- `--message MESSAGE`  
  (string) The message you want to sign.
- `--pem PEM`  
  (string) The path to a validator pem file.
- `--index INDEX`  
  (integer, optional) The index of the validator in case the file contains multiple validators (default: 0).

## Example

```bash
mxpy validator-wallet sign-message --message "hello" --pem validator.pem --index 0
