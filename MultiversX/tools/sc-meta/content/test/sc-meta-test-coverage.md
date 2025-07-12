# sc-meta test-coverage

Run test coverage and output report.

## Usage

```bash
sc-meta test-coverage [OPTIONS] --output <OUTPUT>
```

## Parameters

- `-o, --output <OUTPUT>`  
  Output file path.

- `-f, --format <FORMAT>`  
  Output format. Possible values: markdown, json.

- `-i, --ignore-filename-regex <IGNORE_FILENAME_REGEX>`  
  Ignore files by path patterns.

## Example

```bash
sc-meta test-coverage --output coverage.md --format markdown
