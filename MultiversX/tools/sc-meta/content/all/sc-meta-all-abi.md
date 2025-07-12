# sc-meta all abi

Generates the contract ABI and nothing else.

## Usage

```bash
sc-meta all abi [OPTIONS]
```

## Parameters

- `--path <PATH>`  
  Target directory where to call all contract meta crates. Will be current directory if not specified.

- `--ignore <IGNORE>`  
  Ignore all directories with these names. Default: target

- `--no-abi-git-version`  
  Skips loading the Git version into the ABI

- `--target-dir-meta <TARGET_DIR_META>`  
  For the meta crates, allows specifying the target directory where the Rust compiler will build the intermediary files. Sharing the same target directory can speed up building multiple contract crates at once.

- `--target-dir-all <TARGET_DIR_ALL>`  
  Overrides both the --target-dir-meta and the --target-dir-wasm args.

## Example

```bash
sc-meta all abi
