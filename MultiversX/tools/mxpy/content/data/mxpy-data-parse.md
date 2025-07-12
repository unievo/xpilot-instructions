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
  The Python-Dictionary expression to evaluate in order to extract the data.

## Example

```bash
mxpy data parse --file data.json --expression "['key']"
