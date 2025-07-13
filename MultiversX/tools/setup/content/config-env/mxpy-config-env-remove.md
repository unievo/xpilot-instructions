# mxpy config-env remove

Deletes an environment from the env file. Use `mxpy config-env switch` to switch to another env.

## Usage

```bash
mxpy config-env remove --env ENV
```

## Parameters

- `--env ENV`  
  The name of the environment to operate on.

## Example

```bash
mxpy config-env remove --env devnet
mxpy config-env remove --env testnet
