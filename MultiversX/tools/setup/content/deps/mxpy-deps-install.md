# mxpy deps install

Install dependencies or multiversx-sdk modules.

## Usage

```bash
mxpy deps install {all,golang,testwallets} [--overwrite]
```

## Parameters

- `{all,golang,testwallets}`  
  The dependency to install.

- `--overwrite`  
  Overwrite an existing installation.

## Example

```bash
mxpy deps install all
mxpy deps install golang --overwrite
mxpy deps install testwallets
