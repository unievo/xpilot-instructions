# sc-meta local-deps

Generates a report on the local dependencies of contract crates. Will explore indirect dependencies too.

## Usage

```bash
sc-meta local-deps [OPTIONS]
```

## Parameters

- `--path <PATH>`  
  Target directory where to generate local deps reports. Will be current directory if not specified.

- `--ignore <IGNORE>`  
  Ignore all directories with these names. Default: target.

## Example

```bash
sc-meta local-deps
