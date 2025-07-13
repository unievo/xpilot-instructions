# mxpy config-env delete

Deletes an env value from the specified environment.

## Usage

```bash
mxpy config-env delete NAME [--env ENV]
```

## Parameters

- `NAME`  
  The name of the configuration entry.

- `--env ENV`  
  The name of the environment to operate on.

## Example

```bash
mxpy config-env delete proxy
mxpy config-env delete chain --env devnet
