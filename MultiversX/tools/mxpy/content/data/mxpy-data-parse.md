# mxpy data parse

Parses values from a given file.

## Usage

```bash
mxpy data parse --file FILE --expression EXPRESSION
```

## Parameters

- `--file FILE`  
  Path of the file to parse.

- `--expression EXPRESSION`  
  Python-Dictionary expression to evaluate for extracting data.

## Example

```bash
mxpy data parse --file input.json --expression "{'key': value}"
