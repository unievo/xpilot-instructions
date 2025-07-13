# mxpy config-env get

Gets an env value from the specified environment.

## Usage

```bash
mxpy config-env get NAME [--env ENV]
```

## Parameters

- `NAME`  
  The name of the configuration entry.

- `--env ENV`  
  The name of the environment to operate on.

## Example

```bash
mxpy config-env get proxy
mxpy config-env get chain --env devnet
