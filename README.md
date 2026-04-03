<div align="center">

```
██╗   ██╗███╗   ███╗██╗   ██╗████████╗██╗   ██╗ ██████╗ ███╗   ██╗
██║   ██║████╗ ████║██║   ██║╚══██╔══╝██║   ██║██╔════╝ ████╗  ██║
██║   ██║██╔████╔██║██║   ██║   ██║   ██║   ██║██║  ███╗██╔██╗ ██║
██║   ██║██║╚██╔╝██║██║   ██║   ██║   ██║   ██║██║   ██║██║╚██╗██║
╚██████╔╝██║ ╚═╝ ██║╚██████╔╝   ██║   ╚██████╔╝╚██████╔╝██║ ╚████║
 ╚═════╝ ╚═╝     ╚═╝ ╚═════╝    ╚═╝    ╚═════╝  ╚═════╝ ╚═╝  ╚═══╝
```

**`Rust Engineer · Polymarket Specialist · Prediction Market Infrastructure`**

</div>

---

## About

Rust engineer with a deep focus on prediction market systems and trading infrastructure. I build the tooling that serious Polymarket participants rely on — execution engines, market data pipelines, automated trading strategies, and CLOB integrations that perform under pressure.

If it touches Polymarket at the infrastructure level — order management, position tracking, market resolution, liquidity analysis — I've built it or broken it trying.

- 🦀 **Core:** Rust — async I/O, lock-free data structures, zero-cost abstractions
- 📊 **Domain:** Polymarket CLOB, prediction market mechanics, probability modeling
- ⛓ **Chains:** Polygon (Polymarket's native chain), Ethereum, EVM tooling
- 🔩 **Systems:** Low-latency execution, WebSocket orderbook feeds, RPC management
- 🐳 **Infra:** Linux bare-metal, Docker, CI/CD, observability pipelines

---

## Tech Stack

### Rust Ecosystem
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tokio](https://img.shields.io/badge/Tokio-6E4AFF?style=flat-square&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/Axum-1a1a1a?style=flat-square&logo=rust&logoColor=white)
![Actix](https://img.shields.io/badge/Actix-1E1E1E?style=flat-square&logo=rust&logoColor=white)
![Serde](https://img.shields.io/badge/Serde-DEA584?style=flat-square&logo=rust&logoColor=black)
![Rayon](https://img.shields.io/badge/Rayon-FF6F00?style=flat-square&logo=rust&logoColor=white)

### Prediction Markets & Blockchain
![Polymarket](https://img.shields.io/badge/Polymarket-0070f3?style=flat-square&logoColor=white)
![Polygon](https://img.shields.io/badge/Polygon-8247E5?style=flat-square&logo=polygon&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)
![ethers-rs](https://img.shields.io/badge/ethers--rs-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)

### Data & Storage
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![TimescaleDB](https://img.shields.io/badge/TimescaleDB-FDB515?style=flat-square&logoColor=black)

### Infrastructure
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)

### Other Languages
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-FFD43B?style=flat-square&logo=python&logoColor=blue)

---

## Polymarket Depth

```
┌─────────────────────────────────────────────────────────────────────┐
│  CLOB Integration           Market Analysis         Execution        │
│  ─────────────────          ───────────────         ─────────        │
│  · REST + WS API            · Probability curves    · Order routing  │
│  · Order book streaming     · Resolution tracking   · Slippage mgmt  │
│  · Position management      · Liquidity modeling    · Fill detection  │
│  · Auth & signing (L1/L2)   · Market correlation    · Retry logic     │
│                                                                       │
│  Automation                 Infrastructure          Analytics         │
│  ──────────                 ──────────────          ─────────         │
│  · Market making bots       · Multi-key management  · P&L tracking   │
│  · Condition monitoring     · RPC failover          · Exposure calc   │
│  · Auto-rebalancing         · Event-driven arch     · Historical data  │
│  · Alert pipelines          · TimescaleDB storage   · Backtest engine  │
└─────────────────────────────────────────────────────────────────────┘
```

---

## GitHub Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=crellios&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true&count_private=true&rank_icon=github" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=crellios&layout=compact&theme=github_dark&hide_border=true&langs_count=6" />

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=crellios&theme=github-dark-blue&hide_border=true)](https://git.io/streak-stats)

</div>

---

## Philosophy

```rust
/// The only acceptable latency is the one the network imposes.
/// Everything else is your problem to fix.
async fn execute(order: Order) -> Result<Fill, ExecError> {
    let signed = wallet.sign(order).await?;
    clob.submit(signed).await?.into_fill()
}
```

Prediction markets are probabilistic systems sitting on top of deterministic blockchains. The edge lives in the gap between market price and true probability — and capturing that edge consistently requires infrastructure that is faster, more reliable, and more correct than the competition.

I write Rust because the guarantees matter. No GC pauses during a fill. No race conditions in the orderbook. No silent integer overflows in position math.

---

## Currently

- 🔭 Building a multi-market automated trading system on Polymarket with custom pricing models
- 📦 Maintaining open-source Rust tooling for Polymarket CLOB integration
- 🌱 Researching market microstructure and liquidity dynamics in prediction markets
- 💬 Open to serious collaboration on prediction market infrastructure or trading systems

---

</div>
