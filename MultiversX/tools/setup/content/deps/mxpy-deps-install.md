# mxpy deps install

Install dependencies or multiversx-sdk modules.

## Usage

```bash
mxpy deps install {all|golang|testwallets} [--overwrite]
```

## Parameters

- `{all|golang|testwallets}` (string)  
  The dependency to install.
- `--overwrite` (flag)  
  Whether to overwrite an existing installation.

## Example

```bash
mxpy deps install golang --overwrite
