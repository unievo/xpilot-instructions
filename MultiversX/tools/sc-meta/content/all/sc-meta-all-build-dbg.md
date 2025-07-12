# sc-meta all build-dbg

Builds contract(s) with symbols and WAT.

## Usage

```bash
sc-meta all build-dbg [OPTIONS]
```

## Parameters

- `--target-dir-wasm <TARGET_DIR_WASM>`  
  For the wasm crate, allows specifying the target directory where the Rust compiler will build the intermediary files. Sharing the same target directory can speed up building multiple contract crates at once. Has alias `target-dir` for backwards compatibility.

- `--twiggy-top`  
  Generate a twiggy top report after building.

- `--twiggy-paths`  
  Generate a twiggy paths report after building.

- `--twiggy-monos`  
  Generate a twiggy monos report after building.

- `--twiggy-dominators`  
  Generate a twiggy dominators report after building.

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
sc-meta all build-dbg
