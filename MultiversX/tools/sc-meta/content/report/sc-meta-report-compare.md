# sc-meta report compare

Compare two contract reports.

## Usage

```bash
sc-meta report compare --baseline <BASELINE> --new <NEW> --output <OUTPUT>
```

## Parameters

- `-b, --baseline <BASELINE>`  
  Path to the previous version of code report JSON file that will be used for comparison.

- `-n, --new <NEW>`  
  Path to the current version of the code report JSON file that will be compared.

- `-o, --output <OUTPUT>`  
  Path to the Markdown file where the comparison results will be written.

- `-h, --help`  
  Print help.

- `-V, --version`  
  Print version.

## Example

```bash
sc-meta report compare --baseline report_v1.json --new report_v2.json --output comparison.md
