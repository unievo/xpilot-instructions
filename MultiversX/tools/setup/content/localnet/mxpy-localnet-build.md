# mxpy localnet build

Build necessary software for running a localnet.

## Usage

```bash
mxpy localnet build [--configfile CONFIGFILE] [--software {node,seednode,proxy} [{node,seednode,proxy} ...]]
```

## Parameters

- `--configfile CONFIGFILE`  
  Optional configuration file describing the localnet.

- `--software {node,seednode,proxy} [{node,seednode,proxy} ...]`  
  The software to build (default: ['node', 'seednode', 'proxy']).

## Example

```bash
mxpy localnet build
mxpy localnet build --configfile localnet-config.json --software node proxy
