# sc-meta test

Runs cargo test.

## Usage

```bash
sc-meta test [OPTIONS]
```

## Parameters

- `-p, --path <PATH>`  
  Target directory where to generate contract integration tests. Will be current directory if not specified.

- `-g, --go`  
  Runs Rust and Go tests. Default: false.

- `-c, --chain-simulator`  
  Runs interactor tests using chain simulator. Default: false.

- `-s, --scen`  
  Runs scenarios. Default: false. If scen and go are both specified, scen overrides the go argument.

- `-n, --nocapture`  
  Prints the entire output of the vm. Default: false.


## Example

```bash
sc-meta test
