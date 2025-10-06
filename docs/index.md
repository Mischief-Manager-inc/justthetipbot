---
layout: default
title: JustTheTip Bot
---

# JustTheTip Discord Crypto Tipping Bot

A Discord tip bot supporting Solana (SOL) and multiple cryptocurrencies. Allows users to tip, withdraw, airdrop, and donate crypto via Discord commands.

## Features

- **Multi-coin support**: SOL, USDC (Solana), LTC, BTC (testnet), BCH
- **Secure tipping**: Tip users directly in Discord
- **Airdrops**: Create community airdrops for engagement
- **Wallet integration**: Register and withdraw to external wallets  
- **Privacy focused**: Sensitive information sent via DM
- **Safety features**: Rate limiting, input validation, and persistent storage

## Quick Start

### Setup
1. Install dependencies: `npm install`
2. Configure environment variables (see `.env.example`)
3. Run the bot: `node bot.js`

### Commands
- `!balance` — Show your balances
- `!tip @user amount coin` — Tip a user (e.g. `!tip @bob 0.1 sol`)
- `!registerwallet coin address` — Register your wallet address
- `!withdraw address amount coin` — Withdraw to external wallet
- `!deposit` — Get deposit instructions
- `!airdrop amount coin` — Create an airdrop for others to collect
- `!collect` — Collect from the latest airdrop
- `!burn amount coin` — Donate to support development
- `!help` — Show help message

## External Wallet Helper

For advanced wallet integration and management, check out our [External Wallet Helper application](../justthetip---external-wallet-helper/).

## Security

- **Never share your private keys**
- **Use secure key management for production**
- **All actions are logged for audit and debugging**
- **The bot does not hold real cryptocurrency on behalf of users**

## Support

For questions and support, contact: [jmenichole007@outlook.com](mailto:jmenichole007@outlook.com)

---

MIT License