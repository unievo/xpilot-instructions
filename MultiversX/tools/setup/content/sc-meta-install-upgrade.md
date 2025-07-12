To install or upgrade the `sc-meta` tool, run the following command:

```bash
cargo install multiversx-sc-meta --locked
```

The installation depends on the `cargo` tool, which is part of the Rust toolchain. If Rust is not installed, installation instructions are available [here](https://www.rust-lang.org/tools/install).

On Ubuntu (or Windows with WSL), you might need to install the following dependencies of Rust and sc-meta first:

```bash
sudo apt-get install build-essential pkg-config libssl-dev
```

Install Rust as recommended on rust-lang.org:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Afterwards, in a new terminal install sc-meta:

```bash
cargo install multiversx-sc-meta --locked
```

More information and troubleshooting information available [here](https://docs.multiversx.com/sdk-and-tools/troubleshooting/rust-setup/).