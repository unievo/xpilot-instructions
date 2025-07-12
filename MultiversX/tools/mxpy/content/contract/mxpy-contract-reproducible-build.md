# mxpy contract reproducible-build

Build a Smart Contract and get the same output as a previously built Smart Contract.

## Usage

```bash
mxpy contract reproducible-build [project directory] [options]
```

## Parameters

- `project`  
  The project directory (default: current directory).

- `--debug`  
  Set debug flag (default: False).

- `--no-optimization`  
  Bypass optimizations (for clang) (default: False).

- `--no-wasm-opt`  
  Do not optimize wasm files after the build (default: False).

- `--cargo-target-dir CARGO_TARGET_DIR`  
  For rust projects, forward the parameter to Cargo.

- `--wasm-symbols`  
  For rust projects, does not strip the symbols from the wasm output. Useful for analysing the bytecode. Creates larger wasm files. Avoid in production (default: False).

- `--wasm-name WASM_NAME`  
  For rust projects, optionally specify the name of the wasm bytecode output file.

- `--wasm-suffix WASM_SUFFIX`  
  For rust projects, optionally specify the suffix of the wasm bytecode output file.

- `--docker-image DOCKER_IMAGE`  
  The docker image tag used to build the contract.

- `--contract CONTRACT`  
  Contract to build (contract name, as found in Cargo.toml).

- `--no-docker-interactive`  
  Disable interactive mode for Docker.

- `--no-docker-tty`  
  Disable TTY for Docker.

- `--no-default-platform`  
  Do not set DOCKER_DEFAULT_PLATFORM environment variable to 'linux/amd64'.

- `-h, --help`  
  Show help message and exit.

## Example

Build a contract reproducibly:

```bash
mxpy contract reproducible-build ./my-contract --docker-image multiversx/sdk-rust-contract-builder:latest
