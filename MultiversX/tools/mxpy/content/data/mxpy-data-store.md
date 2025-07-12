# mxpy data store

Stores a key-value pair within a partition.

## Usage

```bash
mxpy data store --key KEY --value VALUE [--partition PARTITION] [--use-global]
```

## Parameters

- `--key KEY`  
  The key.

- `--value VALUE`  
  The value to save.

- `--partition PARTITION`  
  The storage partition (default: *).

- `--use-global`  
  Use the global storage (default: False).

## Example

```bash
mxpy data store --key username --value alice --partition users
mxpy data store --key config --value "enabled" --use-global
