# sc-meta test-gen

Generates Rust integration tests based on scenarios provided in the scenarios folder of each contract.

## Usage

```bash
sc-meta test-gen [OPTIONS]
```

## Parameters

- `--path <PATH>`  
  Target directory where to generate contract integration tests. Will be current directory if not specified.

- `--ignore <IGNORE>`  
  Ignore all directories with these names. Default: target.

- `--create`  
  Creates test files if they don't exist.

## Example

```bash
sc-meta test-gen --create
