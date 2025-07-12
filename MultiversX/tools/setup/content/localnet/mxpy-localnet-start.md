# mxpy localnet start

Start a localnet.

## Usage

```bash
mxpy localnet start [--configfile CONFIGFILE] [--stop-after-seconds STOP_AFTER_SECONDS]
```

## Parameters

- `--configfile CONFIGFILE`  
  Optional configuration file describing the localnet.

- `--stop-after-seconds STOP_AFTER_SECONDS`  
  Stop the localnet after a given number of seconds (default: 31536000).

## Example

```bash
mxpy localnet start
mxpy localnet start --configfile localnet-config.json --stop-after-seconds 3600
