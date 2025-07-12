# sc-meta all build

Builds contract(s) for deploy on the blockchain.

## Usage

```bash
sc-meta all build [OPTIONS]
```

## Parameters

- `--locked`  
  Require that the Cargo.lock in the wasm crates is up to date.

- `--wasm-symbols`  
  Adds debug symbols in the resulting WASM binary. Adds bloat, but helps with debugging. Do not use in production.

- `--wasm-name <WASM_NAME_OVERRIDE>`  
  Overrides the main contract output name.

- `--wasm-suffix <WASM_NAME_SUFFIX>`  
  Adds given suffix to all built contracts.

- `--no-wasm-opt`  
  Skips applying the wasm-opt tool after building the contracts.

- `--wat`  
  Also generate a WAT file when building.

- `--mir`  
  Also emit MIR files when building.

- `--llvm-ir`  
  Also emit LL (LLVM) files when building.

- `--no-imports`  
  Skips extracting the EI imports after building the contracts.

- `--path <PATH>`  
  Target directory where to call all contract meta crates. Will be current directory if not specified.

- `--ignore <IGNORE>`  
  Ignore all directories with these names. Default: target

- `--target-dir-wasm <TARGET_DIR_WASM>`  
  For the wasm crate, allows specifying the target directory where the Rust compiler will build the intermediary files. Sharing the same target directory can speed up building multiple contract crates at once. Has alias `target-dir` for backwards compatibility.

- `--no-abi-git-version`  
  Skips loading the Git version into the ABI

- `--twiggy-top`  
  Generate a twiggy top report after building.

- `--target-dir-meta <TARGET_DIR_META>`  
  For the meta crates, allows specifying the target directory where the Rust compiler will build the intermediary files. Sharing the same target directory can speed up building multiple contract crates at once.

- `--twiggy-paths`  
  Generate a twiggy paths report after building.

- `--target-dir-all <TARGET_DIR_ALL>`  
  Overrides both the --target-dir-meta and the --target-dir-wasm args.

- `--twiggy-monos`  
  Generate a twiggy monos report after building.

- `--twiggy-dominators`  
  Generate a twiggy dominators report after building.

## Example

```bash
sc-meta all build
