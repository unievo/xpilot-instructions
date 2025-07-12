# sc-meta report compile

Generates the contract report.

## Usage

```bash
sc-meta report compile --path <PATH> --output <OUTPUT>
```

## Parameters

- `-p, --path <PATH>`  
  Target directory where to generate code report.

- `-o, --output <OUTPUT>`  
  Path to the Markdown or JSON file where the report results will be written.

- `-h, --help`  
  Print help.

- `-V, --version`  
  Print version.

## Example

```bash
sc-meta report compile --path ./contracts --output report.md
