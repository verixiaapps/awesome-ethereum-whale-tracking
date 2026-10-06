# Awesome Ethereum Whale Tracking [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, datasets, APIs, and research for tracking Ethereum whale activity.

Whale tracking — the practice of monitoring large on-chain actors to infer market behavior — has matured from a niche enthusiast pursuit into a core workflow for traders, researchers, journalists, and protocol teams. This list collects the resources that actually work: live dashboards, queryable datasets, RPC providers, open-source libraries, attribution sources, alert feeds, and the educational material worth your time.

**Scope:** Ethereum mainnet and Ethereum-aligned L2s (Base, Arbitrum, Optimism, Linea, Scroll, Blast). Tools that cover Ethereum alongside other chains are included; chains-only tools (Bitcoin, Solana, Tron) are out of scope.

**Inclusion criteria:** active project, public URL, demonstrable value for understanding or reacting to whale behavior. No paid placements. Honest descriptions including pricing tier.

**Disclaimer:** This list is for informational purposes only. Nothing here constitutes financial advice. On-chain activity is not predictive of future price action. Always do your own research.

---

## Contents

- [Live Whale Trackers — Premium Institutional](#live-whale-trackers--premium-institutional)
- [Live Whale Trackers — Free / Freemium](#live-whale-trackers--free--freemium)
- [Datasets](#datasets)
- [APIs and RPC Providers](#apis-and-rpc-providers)
- [Open-Source Libraries](#open-source-libraries)
- [Wallet Labeling and Attribution](#wallet-labeling-and-attribution)
- [Real-Time Alerting](#real-time-alerting)
- [MEV and On-Chain Forensics](#mev-and-on-chain-forensics)
- [Research and Educational Content](#research-and-educational-content)
- [Block Explorers](#block-explorers)
- [Contributing](#contributing)

---

## Live Whale Trackers — Premium Institutional

Subscription products focused on institutional-grade wallet labeling, deep historical data, and enterprise compliance.

- [Arkham Intelligence](https://www.arkhamintelligence.com) — Wallet de-anonymization, entity attribution, intelligence dashboards. Free tier with paid plans ($149-$999/mo).
- [Chainalysis](https://www.chainalysis.com) — Enterprise compliance + investigation tooling. Used by regulators and large institutions. Custom pricing.
- [Glassnode](https://glassnode.com) — On-chain metrics, market intelligence, and whale cohort analysis. Free tier with paid plans ($39-$799/mo).
- [Messari](https://messari.io) — Crypto research, market data, and asset-level fundamentals. Free tier with paid plans.
- [Nansen](https://www.nansen.ai) — Institutional wallet labeling and on-chain analytics with the largest known wallet-label database. Paid only ($150-$2,000/mo).
- [Token Terminal](https://tokenterminal.com) — Protocol-level revenue, fees, and fundamentals. Free + paid tiers.

## Live Whale Trackers — Free / Freemium

Tools accessible without payment (or with a meaningful free tier).

- [DeBank](https://debank.com) — Portfolio tracking, watchlists, and per-wallet DeFi position views. Free.
- [Deep Blue Alpha](https://deepbluealpha.io) — Ethereum whale tracking with live DEX flows, exchange flow separation, conviction scoring, and a confirmed-pick scoreboard. Free tier; founder Pro at $9.99/mo and founder Alpha at $19.99/mo.
- [DefiLlama](https://defillama.com) — Protocol TVL, fees, and per-protocol whale flows. Free.
- [DexCheck](https://dexcheck.ai) — Whale tracking + multi-chain alpha signals. Free tier + paid.
- [Dune](https://dune.com) — Community-built SQL dashboards covering hundreds of whale-tracking use cases. Free to query and view.
- [Etherscan](https://etherscan.io) — Canonical Ethereum block explorer with per-address transaction history and basic whale-tracking primitives. Free.
- [Lookonchain](https://www.lookonchain.com) — Whale trade alerts and analysis published primarily as a public X feed. Free.
- [Whale Alert](https://whale-alert.io) — Large transaction alerts across major chains. Free X feed + paid API.
- [Zerion](https://zerion.io) — DeFi portfolio tracker with wallet-following features. Free.

## Datasets

Bulk or queryable on-chain data sources suitable for analysis, modeling, and research.

- [Allium](https://www.allium.so) — Enterprise blockchain data warehouse with whale-oriented tables. Custom pricing.
- [Deep Blue Alpha Ethereum Whale Activity Dataset](https://deepbluealpha.io/dataset) — Daily-updated CSV sample of the top 1,000 tracked whale wallets with their last 30 days of on-chain trades. CC-BY-4.0 license, free download.
- [Dune Spellbook](https://github.com/duneanalytics/spellbook) — Open-source SQL definitions powering Dune dashboards. MIT licensed.
- [Etherscan Bulk Exports](https://etherscan.io/exportData) — Per-address CSV exports of transaction history. Free.
- [Flipside Crypto](https://flipsidecrypto.xyz) — SQL access to on-chain data across major chains. Free tier with paid options.
- [Footprint Analytics](https://www.footprint.network) — Multi-chain analytics platform with downloadable datasets. Free tier.
- [Google Cloud Public Datasets — Ethereum](https://console.cloud.google.com/marketplace/details/ethereum/crypto-ethereum-blockchain) — Full Ethereum dataset queryable via BigQuery. Pay per query.
- [Kaggle Cryptocurrency Datasets](https://www.kaggle.com/datasets?tags=13225-Cryptocurrencies) — Community-contributed datasets, varying quality and freshness.

## APIs and RPC Providers

Infrastructure for building your own whale-tracking tools.

- [Alchemy](https://www.alchemy.com) — RPC + enhanced data APIs with strong reliability. Free tier.
- [Ankr](https://www.ankr.com) — Decentralized RPC infrastructure across many chains. Free tier.
- [Covalent](https://www.covalenthq.com) — Unified blockchain data API with normalized responses. Free tier.
- [DexScreener API](https://docs.dexscreener.com/api/reference) — DEX trading pair data + real-time pricing across many chains. Free.
- [Etherscan API](https://docs.etherscan.io) — Address, transaction, and contract data direct from the canonical explorer. Free tier (5 req/sec).
- [Infura](https://www.infura.io) — RPC provider operated by ConsenSys. Free tier.
- [Moralis](https://moralis.io) — Web3 backend APIs with NFT, token, and wallet endpoints. Free tier.
- [QuickNode](https://www.quicknode.com) — High-performance RPC + APIs with low-latency endpoints. Free tier.
- [The Graph](https://thegraph.com) — Decentralized indexing for blockchain data via subgraphs. Pay-per-query.
- [HostDeFi x402 API](https://hostdefi.com/features/x402-rpc) — Machine-payable token-risk and JSON-RPC API on 82 chains; per-call USDC, no API key. Free web token scanner at hostdefi.com/scan.

## Open-Source Libraries

Libraries for building on-chain analysis tools.

- [ethers.js](https://github.com/ethers-io/ethers.js) — Compact JavaScript Ethereum library. MIT licensed.
- [ethers.rs](https://github.com/gakonst/ethers-rs) — Rust Ethereum library with strong typing. Apache-2.0 / MIT.
- [Foundry](https://github.com/foundry-rs/foundry) — Rust toolkit for Ethereum development with forking and simulation. Apache-2.0 / MIT.
- [Hardhat](https://github.com/NomicFoundation/hardhat) — JavaScript development environment with mainnet forking for whale-trade simulation. MIT licensed.
- [viem](https://github.com/wevm/viem) — Modern TypeScript Ethereum library, lightweight alternative to ethers. MIT licensed.
- [wagmi](https://github.com/wevm/wagmi) — React hooks for Ethereum, built on viem. MIT licensed.
- [web3.js](https://github.com/web3/web3.js) — Original JavaScript Ethereum library. LGPL-3.0.
- [web3.py](https://github.com/ethereum/web3.py) — Python Ethereum client library. MIT licensed.

## Wallet Labeling and Attribution

Sources for identifying who is behind an Ethereum address.

- [Arkham Entity Explorer](https://intel.arkm.com) — Comprehensive wallet-to-entity attribution with public free access.
- [Etherscan Address Labels](https://etherscan.io/labelcloud) — Public labels for exchanges, protocols, and known wallets, visible per-address.
- [Etherscan Public Notes](https://etherscan.io) — User-contributed labels appearing on individual address pages.
- [Nansen Wallet Labels](https://www.nansen.ai/research) — Institutional-grade wallet attribution behind the Nansen paywall.
- [OpenLabels Initiative](https://github.com/openlabelsinitiative/OLI) — Community-driven, open-licensed Ethereum address labels.

## Real-Time Alerting

Push notifications and feeds for whale activity.

- [Deep Blue Alpha on Telegram](https://t.me/DeepBlueAlphaIO) — Broadcast channel for whale alerts and hourly reports. Free.
- [Deep Blue Alpha on X](https://x.com/DeepBlueAlpha) — Hourly whale reports, news briefs, and confirmed-pick updates. Free.
- [Etherscan Alerts](https://etherscan.io) — Configurable email alerts for any address. Free.
- [Forta Network](https://forta.org) — Decentralized threat-detection bots, many monitoring whale behavior. Free.
- [Lookonchain on X](https://x.com/lookonchain) — Curated whale trade alerts and analysis. Free.
- [Whale Alert on X](https://x.com/whale_alert) — Large transactions across BTC, ETH, and many other chains. Free.

## MEV and On-Chain Forensics

Adjacent territory — MEV (maximal extractable value) tooling overlaps heavily with whale-trade detection.

- [Flashbots](https://www.flashbots.net) — Research and infrastructure for MEV transparency.
- [MEV-Inspect-py](https://github.com/flashbots/mev-inspect-py) — Open-source MEV classification at scale. Apache-2.0.
- [Phalcon](https://phalcon.blocksec.com) — Transaction debugger and exploit forensics. Free tier.
- [Tenderly](https://tenderly.co) — Transaction simulation, debugging, and on-chain monitoring. Free tier + paid.

## Research and Educational Content

Long-form material worth reading for context on whale behavior and on-chain analysis methodology.

- [a16z crypto](https://a16zcrypto.com/posts) — Crypto research from Andreessen Horowitz's crypto team.
- [Bankless](https://newsletter.banklesshq.com) — Ethereum-focused newsletter and research.
- [Deep Blue Alpha Research](https://deepbluealpha.io/research) — Methodology, whale-behavior studies, and on-chain analysis guides.
- [DefiLlama Blog](https://defillama.com/news) — Protocol-level analysis and rankings methodology.
- [Glassnode Insights](https://insights.glassnode.com) — On-chain analytics research published by the Glassnode team.
- [Messari Research](https://messari.io/research) — Crypto research reports across asset categories.
- [The Block Research](https://www.theblockresearch.com) — Institutional crypto research and data.

## Block Explorers

Foundational tools — every whale-tracking workflow starts at one of these.

- [Beaconcha.in](https://beaconcha.in) — Ethereum consensus-layer explorer (validators, staking).
- [Blockchair](https://blockchair.com) — Multi-chain explorer with cross-chain search.
- [Etherscan](https://etherscan.io) — Canonical Ethereum execution-layer explorer.
- [Ethplorer](https://ethplorer.io) — Alternative Ethereum explorer with token-centric views.
- [OKLink](https://www.oklink.com) — Multi-chain explorer with whale tagging.

---

## Contributing

Suggestions for new resources are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) first. Every entry must be active, public, and add genuine value for someone tracking Ethereum whales.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the maintainers have waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE).
