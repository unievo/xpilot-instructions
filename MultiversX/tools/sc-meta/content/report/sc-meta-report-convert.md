# sc-meta report convert

Converts a contract report to a Markdown file.

## Usage

```bash
sc-meta report convert --input <INPUT> --output <OUTPUT>
```

## Parameters

- `-i, --input <INPUT>`  
  Path to the JSON report file that needs to be converted to Markdown format.

- `-o, --output <OUTPUT>`  
  Path to the Markdown file where the report results will be written.

- `-h, --help`  
  Print help.

- `-V, --version`  
  Print version.

## Example

```bash
sc-meta report convert --input report.json --output report.md
