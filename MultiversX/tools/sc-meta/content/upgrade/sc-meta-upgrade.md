# sc-meta upgrade

Upgrades a contract to the latest framework version. Multiple contract crates are allowed.

## Usage

```bash
sc-meta upgrade [OPTIONS]
```

## Parameters

- `--path <PATH>`  
  Target directory where to upgrade contracts. Will be current directory if not specified.

- `--ignore <IGNORE>`  
  Ignore all directories with these names. Default: target

- `--to <OVERRIDE_TARGET_VERSION>`  
  Overrides the version to upgrade to. By default it will be the last version out.

- `-n, --no-check`  
  Skips 'cargo check' after upgrade

## Example

```bash
sc-meta upgrade