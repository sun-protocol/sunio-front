# Sunio-front

[English](./README.md) | [中文](./README_CN.md)

SUN.io is an integrated DeFi platform built on the [TRON](https://tron.network/) blockchain, offering token swapping, liquidity provision, yield farming, stablecoin swaps, and decentralized governance. As the core DeFi hub of the TRON ecosystem, SUN.io connects multiple protocols — SunSwap (V1/V2/V3/V4), stablecoin pools, staking, and a DAO governance system — into a single, unified interface.

## Features

- **Token Swap** — SUN Smart Router optimizes TRON network swaps by selecting the best trading paths and liquidity pools, reducing slippage, and adapting to market changes for fast and favorable trades.
- **Liquidity Pools** — When you add liquidity, you are given pool tokens representing your position. These tokens automatically earn fees proportional to your share of the pool, and can be redeemed at any time.
- **Yield Farming & Staking** — Multiple staking options for you to earn more rewards
- **Governance (DAO)** — Vote on proposals, delegate voting power, and participate in protocol governance
- **PSM (Peg Stability Module)** — Swap between USDD and other stablecoins at 1:1 ratio
- **Scan** — Explore tokens, trading pairs, liquidity data, volume, and trending tokens on-chain
- **SunPump** — Token launchpad and meme coin platform
- **Multi-Wallet Support** — TronLink, TokenPocket, BitKeep, OKX Wallet, Ledger, imToken, Binance Wallet, and WalletConnect

## Tech Stack

| Category | Technology |
|---|---|
| Framework | React 17 |
| State Management | MobX 6 |
| UI Components | Ant Design 5, @sun-frontend/react-ui |
| Blockchain | TronWeb 6, @tronweb3/tronwallet-adapters |
| Charts | D3.js, ECharts, Recharts |

## BTFS
[SUN](https://sun.on.btfs.io/#/home)

## Deployment

This repository contains pre-built static files ready to be served by any web server.

### Nginx

```nginx
server {
    listen 80;
    server_name your-domain.com;
    root /path/to/build;
    index index.html;

    location / {
        try_files $uri $uri/ /index.html;
    }
}
```

### Any Static File Server

The build output can also be served via any static hosting provider (e.g., AWS S3 + CloudFront, Vercel, Netlify, IPFS).

## Supported Wallets

- [TronLink](https://www.tronlink.org/)
- [TokenPocket](https://www.tokenpocket.pro/)
- [BitKeep (Bitget Wallet)](https://web3.bitget.com/)
- [OKX Wallet](https://www.okx.com/web3)
- [Ledger](https://www.ledger.com/)
- [imToken](https://token.im/)
- [Binance Wallet](https://www.binance.com/en/web3wallet)
- [WalletConnect](https://walletconnect.com/)

## Internationalization

SUN.io supports three languages:

- English (`en-US`)
- Simplified Chinese (`zh-CN`)
- Traditional Chinese (`zh-TC`)

Language can be switched via URL parameter (e.g., `?lang=en-US`) or through the in-app language selector.

## Security

If you discover a security vulnerability, please report it responsibly. Do **not** open a public issue. Instead, reach out to the team via the official channels listed at [sun.io](https://sun.io).

## Links

- Website: [https://sun.io](https://sun.io)
- forum：[https://forum.sun.io/](https://forum.sun.io/)
- Documentation：[https://docs.sun.io](https://docs.sun.io)
- Twitter：[https://x.com/OfficialSUNio](https://x.com/OfficialSUNio)
- Telegram：[https://t.me/officialsunecosystem](https://t.me/officialsunecosystem)
- [Whitepaper](https://sun.io/docs/SUN_V3_Whitepaper_cn.pdf)
- [Whitepaper(Mica)](https://sf.sun.io/sun_mica_whitepaper_2025_10_28_1.pdf)
