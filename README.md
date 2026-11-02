# solanachevySOL

**Solana-only fork of [CloddsBot](https://github.com/alsk1992/CloddsBot)**  
Focused exclusively on the Solana ecosystem.

> Original: Open Source AI trading agent (Claude-powered)  
> This fork: **Only Solana** — no EVM, no Polymarket/Kalshi, no CEX futures (Binance/Bybit/Hyperliquid/MEXC), no Bittensor.

## Scope (Solana only)

| Category | Supported |
|----------|-----------|
| **DEXs / Swaps** | Jupiter, Raydium, Orca, Meteora, Pump.fun, Bags.fm |
| **Lending / DeFi** | Kamino, MarginFi, Solend |
| **Perps (on-chain)** | Drift, Percolator |
| **Token Launch** | Meteora Dynamic Bonding Curves, Pump.fun |
| **MEV** | Jito |
| **Payments** | x402 (Solana USDC) |
| **Other** | Whale tracking (Solana), risk engine, skills system, WebChat, Telegram/Discord, MCP |

## What was removed / disabled
- All EVM chains (ETH, Base, Arbitrum, Optimism, Polygon, etc.)
- Uniswap / 1inch / PancakeSwap / Virtuals
- Polymarket, Kalshi, Betfair, Smarkets, Manifold, Metaculus, PredictIt, Opinion.xyz, Predict.fun
- CEX Futures: Binance, Bybit, Hyperliquid, MEXC, Lighter
- Bittensor / TAO mining
- Cross-chain bridges (except pure Solana flows)

## Status

- Base fork exists at: https://github.com/phatloc136852-oss/CloddsBot
- This repo (`solanachevySOL`) is the **named Solana-focused target**.
- Full code stripping (removing non-Solana skills, adapters, config options) is a significant refactor of a large TypeScript codebase.  
  Current state: repository created + scoped README. Codebase still contains the full original tree until further cleanup commits.

## Quick Start (same as upstream for now)

```bash
git clone https://github.com/phatloc136852-oss/solanachevySOL.git
cd solanachevySOL
npm install
cp .env.example .env
# Add ANTHROPIC_API_KEY
npm run build && npm start
```

Or from the full fork:

```bash
git clone https://github.com/phatloc136852-oss/CloddsBot.git
```

## License

MIT (same as original CloddsBot)

---

**Maintained for SolanaChevy** — Solana memecoin / trading agent use cases.
