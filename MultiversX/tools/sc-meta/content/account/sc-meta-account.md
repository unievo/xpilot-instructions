# sc-meta account

Generates a scenario test initialized with real data fetched from the blockchain.

## Usage

```bash
sc-meta account [OPTIONS] --address <ADDRESS>
```

## Parameters

- `--api <API>`  
  Provide the target API you want the data to come from.

- `--address <ADDRESS>`  
  Provide the address you want to retrieve data from.

## Example

```bash
sc-meta account --api https://devnet-api.multiversx.com --address {address}
```
