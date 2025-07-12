# sc-meta all twiggy

Builds contract(s) and generate twiggy reports.

## Usage

```bash
sc-meta all twiggy [OPTIONS]
```

## Parameters

- `--target-dir-wasm <TARGET_DIR_WASM>`  
  For the wasm crate, allows specifying the target directory where the Rust compiler will build the intermediary files. Sharing the same target directory can speed up building multiple contract crates at once. Has alias `target-dir` for backwards compatibility.

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
sc-meta all twiggy
