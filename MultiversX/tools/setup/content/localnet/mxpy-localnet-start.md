# mxpy localnet start

Start a localnet.

## Usage

```bash
mxpy localnet start [options]
```

## Parameters

- `--configfile CONFIGFILE`  
  (string) Optional configuration file describing the localnet.
- `--stop-after-seconds STOP_AFTER_SECONDS`  
  (integer) Stop the localnet after a given number of seconds. Default: 31536000.

## Example

```bash
mxpy localnet start --stop-after-seconds 600 --configfile my-localnet-config.toml
