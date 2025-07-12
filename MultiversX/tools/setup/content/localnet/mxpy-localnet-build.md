# mxpy localnet build

Build necessary software for running a localnet.

## Usage

```bash
mxpy localnet build [options]
```

## Parameters

- `--configfile CONFIGFILE`  
  (string) Optional configuration file describing the localnet.
- `--software {node,seednode,proxy} [{node,seednode,proxy} ...]`  
  (list) The software to build. Default: node, seednode, proxy.

## Example

```bash
mxpy localnet build --software node proxy --configfile my-localnet-config.toml
