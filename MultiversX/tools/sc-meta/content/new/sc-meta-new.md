# sc-meta new

Creates a contract by a pre-existing template.

## Usage

```bash
sc-meta new [OPTIONS] --template <TEMPLATE>
```

## Parameters

- `--name <NAME>`  
  The new name the contract is to receive. If missing, the template name will be considered.

- `--template <TEMPLATE>`  
  The contract template to clone.

- `--tag <TAG>`  
  The framework version on which the contracts should be created.

- `--path <PATH>`  
  Target directory where to create the new contract directory. Will be current directory if not specified.

- `--author <AUTHOR>`  
  The author of the contract. If missing, the default author will be considered.

- `-h, --help`  
  Print help.

- `-V, --version`  
  Print version.

## Example

```bash
sc-meta new --template empty --name MyContract --tag v1.0.0 --path ./contracts --author "Alice"
