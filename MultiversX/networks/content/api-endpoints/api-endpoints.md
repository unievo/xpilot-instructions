## API Endpoints

### Fields data filtering
In order to filter and fetch only specific fields from the response, the fields parameter can be used:
`/accounts?fields=address,balance` for arrays
`/economics?fields=price,marketCap` for object

### Extract
In order to extract a scalar value from an object response, the extract parameter can be used:
`/economics?extract=price`

### Cleanup
If the value of an attribute is undefined, "" (empty string), null, [ ] (empty array) the attribute will be omitted.

### Pagination
Requests that return multiple items will be paginated to 25 items by default.
For a different number of items or for the next pages use `?from=` and `size=` can be used.

### Getting items count
 - To get the total number of items available for a specific list, use available `count` endpoints. Not all lists have a count available.
 - If no count endpoint is available and a count is needed, a list endpoint can be used, but always filtering list endpoint results. For filtering, specify a short length data field, preferably of number type (based on the responses schema), in the `/endpoint?fields={field}` parameter, to limit the data returned. Use commands such as `curl -s "/endpoint?fields={field}" | jq '. | length'`, or other tools to get the count, applying pagination if necessary.

### Endpoints details
Never act on prior knowledge and always read from the following linked files to get all details on the required endpoints and for full parameters schemas.

- [Returns general information about API deployment](mx-api-about-get-endpoints.json)
- [Returns all accounts/count available on blockchain](mx-api-accounts-get-endpoints.json)
- [Returns NFT/SFT/MetaESDT collections/count where the account owns one or more NFTs](mx-api-accounts-collections-get-endpoints.json)
- [Returns contracts/count details for a given account](mx-api-accounts-contracts-get-endpoints.json)
- [Returns deferred payments from legacy staking](mx-api-accounts-deferred-get-endpoints.json)
- [Summarizes all delegation positions with staking providers, together with unDelegation positions](mx-api-accounts-delegation-get-endpoints.json)
- [Returns staking information related to the legacy delegation pool](mx-api-accounts-delegation-legacy-get-endpoints.json)
- [Returns contract deploys/count details for a given account](mx-api-accounts-deploys-get-endpoints.json)
- [Returns account esdts balance/count history](mx-api-accounts-esdthistory-get-endpoints.json)
- [Return account EGLD balance/count history](mx-api-accounts-history-get-endpoints.json)
- [Returns all active / queued nodes where the account is owner](mx-api-accounts-keys-get-endpoints.json)
- [Returns a list of all available NFTs/SFTs/MetaESDTs/count owned by the provided address](mx-api-accounts-nfts-get-endpoints.json)
- [Returns smart contract results/count where the account is sender or receiver](mx-api-accounts-results-get-endpoints.json)
- [Returns NFT/SFT/MetaESDT collections/count where the account is owner or has some special roles assigned to it](mx-api-accounts-roles-get-endpoints.json)
- [Summarizes total staked amount for the given provider, as well as when and how much unbond will be performed](mx-api-accounts-stake-get-endpoints.json)
- [Returns a list of all available fungible tokens/count for a given address, together with their balance](mx-api-accounts-tokens-get-endpoints.json)
- [Returns details of all transactions/count where the account is sender or receiver](mx-api-accounts-transactions-get-endpoints.json)
- [Returns both transfers/count triggerred by a user account (type = Transaction), as well as transfers/count triggerred by smart contracts (type = SmartContractResult), thus providing a full picture of all in/out value transfers for a given account](mx-api-accounts-transfers-get-endpoints.json)
- [Returns all upgrades details for a specific contract address](mx-api-accounts-upgrades-get-endpoints.json)
- [Returns contract verification details](mx-api-accounts-verification-get-endpoints.json)
- [Returns all nodes in the node queue where the account is owner](mx-api-accounts-waiting-list-get-endpoints.json)
- [Returns all smart contracts/count available on blockchain](mx-api-applications-get-endpoints.json)
- [Returns a list of all blocks/count from all shards](mx-api-blocks-get-endpoints.json)
- [Returns non-fungible/semi-fungible/meta-esdt collections/count](mx-api-collections-get-endpoints.json)
- [Returns network-specific constants that can be used to automatically configure dapps](mx-api-constants-get-endpoints.json)
- [Contract Assets (Post)](mx-api-contract-assets-post-endpoints.json)
- [Returns configuration used in dapps](mx-api-dapp-get-endpoints.json)
- [Returns delegation staking contract information](mx-api-delegation-get-endpoints.json)
- [Returns legacy delegation contract global information](mx-api-delegation-legacy-get-endpoints.json)
- [Returns general economics information](mx-api-economics-get-endpoints.json)
- [Returns Network Events](mx-api-events-get-endpoints.json)
- [Returns a list of all node validator identities, used to group nodes by the same entity. "Free-floating" nodes that do not belong to any identity will also be returned](mx-api-identities-get-endpoints.json)
- [Returns remaining unbonding period for a given bls key](mx-api-keys-get-endpoints.json)
- [Returns economics details of xExchange](mx-api-mex-get-endpoints.json)
- [Returns xExchange Pairs, active liquidity pools available on xExchange](mx-api-mex-pairs-get-endpoints.json)
- [Returns all distinct miniblocks](mx-api-miniblocks-get-endpoints.json)
- [Returns a list of Non-Fungible / Semi-Fungible / MetaESDT tokens/count available on blockchain](mx-api-nfts-get-endpoints.json)
- [Triggers NFT media/metadata reprocessing for collection owners](mx-api-nfts-post-endpoints.json)
- [Returns a list/count of nodes of type observer or validator with statuses ("new", "unknown", "waiting", "eligible", "jailed", "queued", "leaving", "inactive", "auction")](mx-api-nodes-get-endpoints.json)
- [Returns the transactions that are currently in the memory pool](mx-api-pool-get-endpoints.json)
- [Returns a list of all staking providers](mx-api-providers-get-endpoints.json)
- [Performs a vm query on a given smart contract and returns its results](mx-api-query-post-endpoints.json)
- [Returns all smart contract results/count available on the blockchain](mx-api-results-get-endpoints.json)
- [Returns a list of all rounds/count available on blockchain](mx-api-rounds-get-endpoints.json)
- [Returns all available shards](mx-api-shards-get-endpoints.json)
- [Returns general staking information](mx-api-stake-get-endpoints.json)
- [Returns general network statistics](mx-api-stats-get-endpoints.json)
- [Returns all distinct NFT tags/count](mx-api-tags-get-endpoints.json)
- [Returns all tokens/count available on the blockchain](mx-api-tokens-get-endpoints.json)
- [Returns a list of transactions/count available on the blockchain](mx-api-transactions-get-endpoints.json)
- [Posts a signed transaction on the blockchain](mx-api-transactions-post-endpoints.json)
- [Returns both transfers/count triggerred by a user account (type = Transaction), and transfers/count triggerred by smart contracts (type = SmartContractResult), to have all in/out value transfers for a given account](mx-api-transfers-get-endpoints.json)
- [Returns account details for a given username. Performs a redirect on the proper account address](mx-api-usernames-get-endpoints.json)
- [Returns node waiting list/count](mx-api-waiting-list-get-endpoints.json)
- [Returns config used for accessing websocket on the same cluster](mx-api-websocket-get-endpoints.json)
- [List with all API endpoints](api-endpoints-list.json)
