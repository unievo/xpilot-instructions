# mxpy config-env set

Sets an env value for the specified environment.

## Usage

```bash
mxpy config-env set NAME VALUE [--env ENV]
```

## Parameters

- `NAME`  
  The name of the configuration entry.

- `VALUE`  
  The new value.

- `--env ENV`  
  The name of the environment to operate on.

## Example

```bash
mxpy config-env set proxy https://devnet-gateway.multiversx.com
mxpy config-env set chain D --env devnet
