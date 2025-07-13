# mxpy validator-wallet sign-message

Sign a message.

## Usage

```bash
mxpy validator-wallet sign-message --message MESSAGE --pem PEM [--index INDEX]
```

## Parameters

- `--message MESSAGE`  
  The message you want to sign.

- `--pem PEM`  
  Path to a validator pem file.

- `--index INDEX`  
  Index of the validator if the file contains multiple validators (default: 0).

## Example

```bash
mxpy validator-wallet sign-message --message "hello world" --pem validator.pem
mxpy validator-wallet sign-message --message "test" --pem validator.pem --index 1
