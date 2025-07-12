# mxpy wallet bech32

Helper for encoding and decoding bech32 addresses.

## Usage

```bash
mxpy wallet bech32 [value] [--encode | --decode] [--hrp HRP]
```

## Parameters

- `value`  
  The value to encode or decode.

- `--encode`  
  Whether to encode the value.

- `--decode`  
  Whether to decode the value.

- `--hrp HRP`  
  The human-readable part; only used for encoding to bech32 (default: erd).

- `-h, --help`  
  Show help message and exit.

## Examples

Encode a hex address to bech32:

```bash
mxpy wallet bech32 0123456789abcdef --encode --hrp erd
```

Decode a bech32 address to hex:

```bash
mxpy wallet bech32 erd1... --decode
