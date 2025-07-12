# mxpy data load

Loads a key-value pair from a storage partition.

## Usage

```bash
mxpy data load --key KEY [--partition PARTITION] [--use-global]
```

## Parameters

- `--key KEY`  
  The key.

- `--partition PARTITION`  
  The storage partition (default: *).

- `--use-global`  
  Use the global storage (default: False).

## Example

```bash
mxpy data load --key username --partition users
mxpy data load --key config --use-global
