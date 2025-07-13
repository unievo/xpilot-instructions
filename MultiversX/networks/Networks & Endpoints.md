# MultiversX Networks Information

## Network details

### Mainnet

- hrp: `erd`
- native token: `EGLD`
- native token decimals: 18
- gateway: `https://gateway.multiversx.com`
- api: `https://api.multiversx.com`
- wallet: `https://wallet.multiversx.com`
- explorer: `https://explorer.multiversx.com`

### Devnet

- hrp: `erd`
- native token: `xEGLD`
- native token decimals: 18
- gateway: `https://devnet-gateway.multiversx.com`
- api: `https://devnet-api.multiversx.com`
- wallet: `https://devnet-wallet.multiversx.com`
- explorer: `https://devnet-explorer.multiversx.com`

### Testnet

- hrp: `erd`
- native token: `xEGLD`
- native token decimals: 18
- gateway: `https://testnet-gateway.multiversx.com`
- api: `https://testnet-api.multiversx.com`
- wallet: `https://testnet-wallet.multiversx.com`
- explorer: `https://testnet-explorer.multiversx.com`

### Vibechain (VibeOX)

- hrp: `vibe`
- native token: `VIBE`
- native token decimals: 18
- gateway: `https://vibeox-gateway.multiversx.com`
- api: `https://vibeox-api.multiversx.com`
- wallet: `https://vibeox-wallet.multiversx.com`
- explorer: `https://vibeox-explorer.multiversx.com`

## API Endpoints

The endpoints include account management, token, collections and NFT operations, staking, delegation, smart contracts, transactions, transfers, blocks, rounds, shards, nodes, validators, identities, staking providers, network events, economics, xExchange details, app configurations, statistics, memory pool, VM queries.

- Always read the [API Endpoints details](./content/api-endpoints/api-endpoints.md) for full details on the endpoints and parameter schemas.

## Network Explorer 

The explorer urls are provided for links to display existing data, not for data retrieval. 
Use the API endpoints for data retrieval.

- Dashboard: {explorerUrl}
- Accounts (wallet addresses and contract addresses) : {explorerUrl}/accounts/
- Account (transactions) : {explorerUrl}/accounts/{address}
- Account tokens : {explorerUrl}/accounts/{address}/tokens
- Account NFTs : {explorerUrl}/accounts/{address}/nfts
- Account contracts : {explorerUrl}/accounts/{address}/contracts
- Applications (contracts) : {explorerUrl}/applications/
- Blocks : {explorerUrl}/blocks/
- Block : {explorerUrl}/blocks/{blockHash}
- Transactions : {explorerUrl}/transactions/
- Transaction : {explorerUrl}/transactions/{txHash}
- Tokens : {explorerUrl}/tokens/
- Token : {explorerUrl}/tokens/{identifier}
- Collections : {explorerUrl}/collections/
- Collection : {explorerUrl}/collections/{collection}
- NFTs : {explorerUrl}/nfts/
- NFT : {explorerUrl}/nfts/{nftIdentifier}
- Validators : {explorerUrl}/validators/
- Validator : {explorerUrl}/identities/{identity}
- Analytics : {explorerUrl}/analytics/
