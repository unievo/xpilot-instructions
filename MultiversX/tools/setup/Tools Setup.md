# mxpy v11.0.0 - Tools Setup

mxpy is a CLI tool for interacting with the Blockchain (in general) and with Smart Contracts (in particular).

## Setup
- [Install or upgrade mxpy](./content/mxpy-install-upgrade.md)
    
## Top-level Options
- `-h,` Show help message
- `-v,` Show version number
- `--verbose` Enable verbose output

## Config mxpy
- [Dump configuration](./content/config/mxpy-config-dump.md)
- [Get configuration value](./content/config/mxpy-config-get.md)
- [Set configuration value](./content/config/mxpy-config-set.md)
- [Delete configuration value](./content/config/mxpy-config-delete.md)
- [Create new configuration](./content/config/mxpy-config-new.md)
- [Switch configuration](./content/config/mxpy-config-switch.md)
- [List configurations](./content/config/mxpy-config-list.md)
- [Reset configuration](./content/config/mxpy-config-reset.md)
## Config Env
- [Delete an env value from the specified environment.](./content/config-env/mxpy-config-env-delete.md)
- [Dumps the active environment.](./content/config-env/mxpy-config-env-dump.md)
- [Gets an env value from the specified environment.](./content/config-env/mxpy-config-env-get.md)
- [List available environments.](./content/config-env/mxpy-config-env-list.md)
- [Creates a new environment and sets it as the active environment.](./content/config-env/mxpy-config-env-new.md)
- [Deletes an environment from the env file. Use `mxpy config-env switch` to switch to another env.](./content/config-env/mxpy-config-env-remove.md)
- [Deletes the environment file. Default env will be used.](./content/config-env/mxpy-config-env-reset.md)
- [Sets an env value for the specified environment.](./content/config-env/mxpy-config-env-set.md)
- [Switch to a different environment.](./content/config-env/mxpy-config-env-switch.md)
## Config Wallet
- [Deletes a config value from the specified wallet.](./content/config-wallet/mxpy-config-wallet-delete.md)
- [Dumps the active wallet.](./content/config-wallet/mxpy-config-wallet-dump.md)
- [Gets a config value from the specified wallet.](./content/config-wallet/mxpy-config-wallet-get.md)
- [List configured wallets.](./content/config-wallet/mxpy-config-wallet-list.md)
- [Creates a new wallet config and sets it as the active wallet.](./content/config-wallet/mxpy-config-wallet-new.md)
- [Removes a wallet from the config using the alias. No default wallet will be set. Use `config-wallet switch` to set a new wallet.](./content/config-wallet/mxpy-config-wallet-remove.md)
- [Deletes the config file. No default wallet will be set.](./content/config-wallet/mxpy-config-wallet-reset.md)
- [Sets a config value for the specified wallet.](./content/config-wallet/mxpy-config-wallet-set.md)
- [Switch to a different wallet.](./content/config-wallet/mxpy-config-wallet-switch.md)
## Dependencies
- [Install dependencies](./content/deps/mxpy-deps-install.md)
- [Check dependencies](./content/deps/mxpy-deps-check.md)
## Localnet Commands
- [Setup localnet](./content/localnet/mxpy-localnet-setup.md)
- [Create new localnet configuration](./content/localnet/mxpy-localnet-new.md)
- [Download prerequisites](./content/localnet/mxpy-localnet-prerequisites.md)
- [Build localnet software](./content/localnet/mxpy-localnet-build.md)
- [Start localnet](./content/localnet/mxpy-localnet-start.md)
- [Configure localnet](./content/localnet/mxpy-localnet-config.md)
- [Clean localnet](./content/localnet/mxpy-localnet-clean.md)


# sc-meta v0.59.0 - Tools Setup

MultiversX Rust smart contract management CLI tool.

## Setup
- [Install or upgrade sc-meta](./content/sc-meta-install-upgrade.md)

## Top-level Options
- `-h,` Show help message
- `-V,` Show version number
- `--verbose` Enable verbose output

## Tools installation
- [Install all tools](./content/install/sc-meta-install-all.md)
- [Install mx-scenario-go](./content/install/sc-meta-install-mx-scenario-go.md)
- [Install wasm32 target](./content/install/sc-meta-install-wasm32.md)
- [Install wasm-opt tool](./content/install/sc-meta-install-wasm-opt.md)
- [Install debugger script](./content/install/sc-meta-install-debugger.md)
## Chain Simulator
- [Install chain simulator](./content/cs/sc-meta-cs-install.md)
- [Start chain simulator](./content/cs/sc-meta-cs-start.md)
- [Stop chain simulator](./content/cs/sc-meta-cs-stop.md)