# Sunio-front

[English](./README.md) | [中文](./README_CN.md)

SUN.io 是构建在 [TRON](https://tron.network/) 区块链上的一站式 DeFi 平台，提供代币兑换、流动性提供、流动性挖矿、稳定币兑换及去中心化治理等功能。作为 TRON 生态的核心 DeFi 枢纽，SUN.io 将 SUN Smart Router、稳定币池、质押和 DAO 治理系统整合于统一界面中。

## 功能特性

- **代币兑换** — SUN Smart Router优化TRON网络交易，智能选择最佳路径和流动性池，减少滑点，快速完成交易并获得最优汇率。
- **流动性池** — 您在增加流动性时会获得代表您仓位的资金池代币。这些代币会按您在资金池的占比自动赚取费用，且能够随时兑现。
- **流动性挖矿与质押** — 多种质押方式，获取更多收益
- **治理（DAO）** — 参与提案投票、委托投票权，参与协议治理
- **PSM（锚定稳定模块）** — 在 USDD 与其他稳定币之间进行 1:1 兑换
- **浏览器** — 浏览链上代币、交易对、流动性数据、交易量及热门代币
- **SunPump** — 代币发射台及 Meme 币平台
- **多钱包支持** — TronLink、TokenPocket、BitKeep、OKX Wallet、Ledger、imToken、Binance Wallet 及 WalletConnect

## 技术栈

| 类别 | 技术 |
|---|---|
| 框架 | React 17 |
| 状态管理 | MobX 6 |
| UI 组件 | Ant Design 5、@sun-frontend/react-ui |
| 区块链 | TronWeb 6、@tronweb3/tronwallet-adapters、@sunio/sun-sdk |
| 图表 | D3.js、ECharts、Recharts |

## 部署

本仓库包含预构建的静态文件，可直接通过任意 Web 服务器部署。

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

### 其他静态文件服务

构建产物也可通过任意静态托管服务部署（如 AWS S3 + CloudFront、Vercel、Netlify、IPFS 等）。

## 支持的钱包

- [TronLink](https://www.tronlink.org)
- [Binance Wallet](https://www.binance.com/en/web3wallet)
- [MetaMask](https://metamask.io)
- [WalletConnect](https://walletconnect.com)
- [BitKeep (Bitget Wallet)](https://web3.bitget.com)
- [OKX Wallet](https://web3.okx.com)
- [TokenPocket](https://www.tokenpocket.pro)
- [Ledger](https://www.ledger.com)

## 国际化

SUN.io 支持三种语言：

- English（`en-US`）
- 简体中文（`zh-CN`）
- 繁体中文（`zh-TC`）

可通过 URL 参数（如 `?lang=zh-CN`）或应用内语言切换器切换语言。

## 安全

如果您发现安全漏洞，请负责任地进行报告。**请勿**创建公开的 Issue，而是通过 [sun.io](https://sun.io) 上列出的官方渠道联系团队。

## 相关链接

- 官网：[https://sun.io](https://sun.io)
- 论坛：[https://forum.sun.io/](https://forum.sun.io/)
- 文档：[https://docs.sun.io](https://docs.sun.io)
- Twitter：[https://x.com/OfficialSUNio](https://x.com/OfficialSUNio)
- Telegram：[https://t.me/officialsunecosystem](https://t.me/officialsunecosystem)
- [白皮书](https://sun.io/docs/SUN_V3_Whitepaper_cn.pdf)
- [白皮书(Mica)](https://sf.sun.io/sun_mica_whitepaper_2025_10_28_1.pdf)
