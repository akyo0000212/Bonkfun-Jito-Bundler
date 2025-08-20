# 🐶 Bonk.fun Multi-Wallet Bundle Trading Bot

A fast and reliable Solana bundle trading bot for **bonkfun** and **bonk.fun**-style token launches. This bot uses **Jito bundles** to create tokens and execute **multi-wallet buys in a single atomic block**. Built with **Raydium SDK v2**, it's designed for seamless one-block execution and fast inclusion.

## 🚀 Features

- ✅ Supports **dynamic multi-wallet bundling** (12+ wallets)
- ✅ Atomically creates tokens and buys from multiple wallets in **one block**
- ✅ Uses **Jito** relayer for secure and efficient bundle submission
- ✅ Executes trades via **Raydium SDK v2**
- ✅ Optimized for priority compute unit pricing

---

## 📸 Sample Bundles on Jito Explorer

These are just examples — the bot supports **any number of wallets**:

| Wallet Count | Jito Bundle                                                                                                  |
| ------------ | ------------------------------------------------------------------------------------------------------------ |
| 2 Wallets    | [🔗 View](https://explorer.jito.wtf/bundle/56ac378f193c9b90a4b6d2c52096a2d783653f300c343d59976691b2a6fcb184) |
| 9 Wallets    | [🔗 View](https://explorer.jito.wtf/bundle/8116172ad6bea279b6873020ac412eb36c9777b311b96ab38c58204637166bf1) |
| 12 Wallets   | [🔗 View](https://explorer.jito.wtf/bundle/eb6d075d4f3e065d5e127ec76c328e00e08d3608ee858a15fa13a21c8f922d98) |

---

## ⚙️ How It Works

1. Creates a new token (like BONK)
2. Prepares swap transactions from multiple wallets
3. Wraps them into a **single atomic bundle** using Jito
4. Submits the bundle for inclusion in the same block

---

## 🛠 Tech Stack

- [Solana Web3.js](https://solana-labs.github.io/solana-web3.js/)
- [Raydium SDK v2](https://github.com/raydium-io/raydium-sdk)
- [Jito-Solana](https://jito.network/)
- Custom bundler and transaction coordinator

---

## ⚡ Performance Tuning

Boost confirmation speed by adjusting compute unit pricing:

```ts
ComputeBudgetProgram.setComputeUnitPrice({ microLamports: 200_000 }); // High priority
```

Use higher values during congestion, or lower for savings.

---

## 🧪 Planned Features

- Auto-retry on bundle failure
- Live bundle result dashboard
- Strategy modules for flexible launch styles
- Telegram / Discord alerts

