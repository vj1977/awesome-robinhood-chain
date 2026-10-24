# Awesome Robinhood Chain [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for Robinhood Chain — the Arbitrum Orbit Layer 2 for tokenized real-world assets. Chain ID **4663** (mainnet) / **46630** (testnet).

Robinhood Chain launched its public mainnet on **July 1, 2026**. It is a permissionless, EVM-compatible Layer 2 built on Arbitrum technology, settling on Ethereum with ETH as the native gas token, purpose-built for tokenized stocks, ETFs, and other real-world assets.

**Disclaimer:** this list is community-maintained and not affiliated with or endorsed by Robinhood. Inclusion is not an endorsement. Nothing here is investment advice.

## Contents

- [Official Resources](#official-resources)
- [Network Access](#network-access)
- [Explorers](#explorers)
- [Data & Analytics](#data--analytics)
- [Monitoring & Verification](#monitoring--verification)
- [Stock Tokens](#stock-tokens)
- [DeFi on Robinhood Chain](#defi-on-robinhood-chain)
- [Collectibles](#collectibles)
- [Infrastructure](#infrastructure)
- [Developer Guides](#developer-guides)
- [Machine-Readable Data](#machine-readable-data)
- [Background & Coverage](#background--coverage)

## Official Resources

- [Robinhood Chain Documentation](https://docs.robinhood.com/chain/) - Official docs: connecting, stock tokens, contracts, deployment.
- [Robinhood Chain Portal](https://robinhood.com/us/en/chain/) - Official marketing and ecosystem site.
- [Ecosystem Directory](https://robinhood.com/us/en/chain/ecosystem/) - Official catalog of partners building on the chain.
- [Network Status](https://status.robinhoodchain.offchain.io/) - Official uptime and incident page (email/Slack/webhook/RSS subscriptions).
- [Canonical Token Contracts](https://docs.robinhood.com/chain/contracts/) - The official registry of canonical stock-token contracts. A matching ticker at any other address is not canonical.

## Network Access

- **Chain ID:** `4663` (mainnet), `46630` (testnet)
- **Public RPC:** `https://rpc.mainnet.chain.robinhood.com` (rate-limited; not recommended as sole production endpoint)
- **Sequencer feed:** `wss://feed.mainnet.chain.robinhood.com`
- **Gas token:** ETH
- [Connecting guide](https://docs.robinhood.com/chain/connecting/) - Official network details and wallet setup.
- [Alchemy](https://www.alchemy.com/) - Recommended production RPC provider; also Data API and gasless transaction infrastructure.

## Explorers

- [Blockscout (official)](https://robinhoodchain.blockscout.com) - The official block explorer, with API access for contracts, tokens, transfers, and logs.
- [Testnet Explorer](https://explorer.testnet.chain.robinhood.com) - Official testnet Blockscout instance.

## Data & Analytics

- [L2Beat](https://l2beat.com/scaling/projects/robinhood) - Risk analysis, stage assessment, and total value secured.
- [DeFiLlama](https://defillama.com/chain/robinhood-chain) - TVL, stablecoins, DEX volume, and fees.
- [growthepie](https://www.growthepie.com/chains/robinhood) - Transactions, active addresses, and chain fundamentals.
- [RWA.xyz](https://app.rwa.xyz/stocks) - Tokenized-stock asset class tracking across chains.
- [Dune](https://dune.com/blockchains/robinhood) - Official Dune integration; community dashboards for chain activity.

## Monitoring & Verification

- [CHAIN4663 RWA WATCH](https://chain4663.com) - Independent, deterministic monitor for canonical stock tokens: corporate actions and multipliers, oracle health, contract verification, live status, and alerts. Not affiliated with Robinhood.
- [Contract verifier](https://chain4663.com/verify) - Check whether an address is in the currently accepted canonical registry (anti-impersonation).
- [Chain status center](https://chain4663.com/service) - Independent availability and component-health tracking with incident history.
- [Corporate-actions calendar](https://chain4663.com/calendar) - Scheduled and applied multiplier events, with iCal subscription.

## Stock Tokens

- [Stock Tokens overview](https://docs.robinhood.com/chain/stock-tokens/) - What the tokens are and how they work.
- [Building with Stock Tokens](https://docs.robinhood.com/chain/building-with-stock-tokens/) - Interfaces: `uiMultiplier()`, `newUIMultiplier()`, `effectiveAt()`, `oraclePaused()`, and corporate-action mechanics.
- [Oracles & Price Feeds](https://docs.robinhood.com/chain/oracles-and-price-feeds/) - Chainlink feeds, 24/5 update schedule, staleness and sequencer checks.
- Key facts: ERC-20, 18 decimals; issued by Robinhood Assets (Jersey) Ltd as tokenized debt instruments tracking underlying equities; holders receive economic exposure, not shareholder rights; not available to U.S. persons.
- Core contracts: WETH `0x0Bd7D308f8E1639FAb988df18A8011f41EAcAD73`, USDG `0x5fc5360D0400a0Fd4f2af552ADD042D716F1d168`.

## DeFi on Robinhood Chain

- [Uniswap](https://uniswap.org/) - Public DEX deployment.
- [Morpho](https://morpho.org/) - Decentralized lending and borrowing.
- [Lighter](https://lighter.xyz/) - Perpetuals DEX.
- [Rialto](https://robinhood.com/us/en/chain/ecosystem/) - PropAMM-driven spot exchange.
- USDG (Paxos) and USDe (Ethena) stablecoins circulate on-chain.

## Collectibles

- [Stockmon](https://www.stockmon.app/genesis) — Creature collections with Genesis originals and Aetheryn descendants on Robinhood Chain.

## Infrastructure

- [Chainlink](https://chain.link/) - Official oracle provider (price feeds, CCIP cross-chain).
- [LayerZero](https://layerzero.network/) - Omnichain messaging and asset bridging.
- [Fireblocks](https://www.fireblocks.com/) / [BitGo](https://www.bitgo.com/) - Institutional custody.
- [Paxos](https://paxos.com/) - USDG stablecoin infrastructure.
- [TRM Labs](https://www.trmlabs.com/) - Compliance and risk analytics.
- [Zerion](https://zerion.io/) - Wallet data API.
- [Allium](https://www.allium.so/) - Onchain data indexing.

## Developer Guides

- [Deploy a smart contract](https://docs.robinhood.com/chain/deploy-smart-contracts/) - Foundry/Hardhat deployment (permissionless).
- [Run a full node](https://docs.robinhood.com/chain/) - Official node guide.
- [QuickNode: read stock-token data onchain](https://www.quicknode.com/guides/robinhood/read-stock-tokens-data-onchain) - Tutorial for querying canonical token state.
- [Transaction finality](https://docs.robinhood.com/chain/transaction-finality/) - Confirmation and finality model.

## Machine-Readable Data

- [Canonical token list](https://chain4663.com/tokenlist.json) - Uniswap-standard token list of canonical stock tokens.
- [Open data exports](https://chain4663.com/data) - CSV/JSON snapshots of registry, state, and events.
- [REST API](https://chain4663.com/openapi.yaml) - OpenAPI spec for assets, events, actions, verification, and status.
- [MCP server](https://chain4663.com/llms.txt) - Model Context Protocol endpoint for AI agents (`https://chain4663.com/mcp`).
- [Address labels](https://chain4663.com/data/address-labels.json) - Canonical and observed-collision label feed.

## Background & Coverage

- [Robinhood Chain mainnet announcement](https://robinhood.com/us/en/newsroom/robinhood-accelerates-global-expansion-robinhood-chain-mainnet-stock-tokens-agentic-trading/) - Official launch newsroom post (July 2026).
- [Arbitrum: Robinhood Chain mainnet](https://blog.arbitrum.io/robinhood-chain-mainnet/) - Technology-stack announcement.
- [Chainlink partnership](https://www.prnewswire.com/news-releases/robinhood-chain-launches-and-adopts-chainlink-to-unlock-access-to-the-onchain-economy-for-millions-of-users-302816242.html) - Official oracle adoption.
- [Dune: Robinhood Chain is live on Dune](https://dune.com/blog/robinhood-chain-is-live-on-dune) - Data-platform integration.

## Contributing

Contributions welcome — open a PR. Entries must be factual, working, and relevant to Robinhood Chain. No token shills, no paid placements.

## License

[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) — public domain.
