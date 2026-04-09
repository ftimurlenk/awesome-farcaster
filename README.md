<div align="center">

# 🟣 Awesome Farcaster

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A carefully curated list of **awesome Farcaster resources** — clients, SDKs, Mini Apps, tools, analytics, bots, and learning materials for builders and users alike.

*Farcaster is a sufficiently decentralized social protocol. This list covers its full ecosystem.*

[Protocol](#-protocol) · [Clients](#-clients) · [Mini Apps](#-mini-apps) · [Remix / Farcade](#-remix--farcade-gaming) · [SDKs](#-sdks--libraries) · [APIs](#-apis--infrastructure) · [Frames](#-frames) · [Bots](#-bots) · [Analytics](#-analytics) · [Tools](#-tools) · [Learning](#-learning) · [Community](#-community)

</div>

---

## 📖 What is Farcaster?

Farcaster is a decentralized social networking protocol that enables permissionless building and distribution of social applications. It combines **on-chain identity** (Ethereum) with **off-chain message storage** (Snapchain), allowing users to maintain portable social identities across multiple clients.

- 🔗 Website: [farcaster.xyz](https://farcaster.xyz)
- 📄 Spec: [Farcaster Protocol](https://github.com/farcasterxyz/protocol)
- 🐦 Twitter/X: [@farcaster_xyz](https://twitter.com/farcaster_xyz)

---

## 🔵 Protocol

> Core infrastructure and protocol-level resources.

- [Farcaster Protocol](https://github.com/farcasterxyz/protocol) — Official protocol specification and design documents.
- [Snapchain](https://docs.farcaster.xyz/reference/snapchain/) — Farcaster's high-performance message layer (10,000+ TPS, 780ms finality). Launched April 2025.
- [Hubble](https://github.com/farcasterxyz/hub-monorepo) — First implementation of a Farcaster Hub node.
- [Farcaster Contracts](https://docs.farcaster.xyz/reference/contracts/) — Solidity contracts for on-chain identity and key registry.
- [FName Registry](https://docs.farcaster.xyz/reference/fname/api) — Farcaster username registration API.
- [Replicator](https://docs.farcaster.xyz/reference/replicator/) — Tool for syncing Farcaster data to a local Postgres database.

---

## 📱 Clients

> Applications built on top of the Farcaster protocol.

### Official
- [Farcaster](https://warpcast.com) — The flagship client by Merkle Manufactory (formerly Warpcast). iOS, Android, Web.

### Third-Party
- [Supercast](https://supercast.xyz) — All-in-one Farcaster client for pros and teams.
- [Recaster](https://recaster.org) — Client with extensive UI controls and configuration.
- [Nook](https://nook.social) — Open-source web and mobile Farcaster client.
- [Herocast](https://herocast.xyz) — Professionalized, multi-feed power-user client.
- [Yup](https://yup.io) — Multi-network decentralized social client (Farcaster + Lens).
- [Kiosk](https://kioskapp.xyz) — Farcaster exploration through quests, gaming and education.
- [Flink](https://flink.fyi) — Client with onchain features like anonymous posting and airdrop claiming.

---

## 🚀 Mini Apps

> Full-screen web apps running natively inside Farcaster clients. Formally launched in Warpcast navigation April 2025.

### 🎮 Games
- [Flappycaster](https://flappycaster.com) — Farcaster-native Flappy Bird. The OG Farcaster mini-game.
- [FarHero](https://farhero.xyz) — 3D Farcaster trading card battle game.
- [Farworld](https://farworld.gg) — Onchain Farcaster monsters — collect, battle, evolve.

### 💰 DeFi & Finance
- [Clanker](https://clanker.world) — Deploy an ERC-20 token on Base by tagging @clanker in a cast.
- [Morpho](https://morpho.org) — DeFi lending and borrowing deposits from your feed.

### 🎨 NFT & Collectibles
- [Mint](https://mint.fun) — Streamlined NFT minting interface for Farcaster protocol drops.
- [Zora](https://zora.co) — NFT creation and discovery with Farcaster integration.

### 🎧 Media & Content
- [Pods](https://pods.media) — Onchain podcast platform with a full embedded Mini App.
- [FC Audio Chat](https://fcaudiochat.xyz) — Clubhouse-style audio rooms, natively on Farcaster.

### 📊 Social & Identity
- [Onchain Alignment Chart](https://alignment.wtf) — Analyze your onchain activity and get a mintable persona score.
- [Interface](https://interface.social) — Humanizes wallet addresses using Farcaster usernames and profile pictures.
- [Rewards](https://warpcast.com/~/rewards) — Warpcast weekly USDC rewards for top active casters.

### 🛠️ Utilities
- [Yoink!](https://yoink.party) — Viral flag-claiming game; also a well-documented Mini App SDK reference. ([GitHub](https://github.com/horsefacts/yoink))
- [miniapps.zone](https://miniapps.zone) — Community-maintained directory of Farcaster Mini Apps.

---

## 🎮 Remix / Farcade Gaming

> Remix (formerly Farcade) is an AI-powered mini-game platform deeply integrated with Farcaster — often described as "TikTok for games." It raised $6.75M from Archetype, Coinbase Ventures, Variant, and Zynga co-founder Justin Waldron. Originally built on Farcaster, it now distributes games across Base, Farcaster, World App, Telegram, and Coinbase Wallet.

### 🔗 Platform
- [Remix](https://remix.gg) — The main platform. Create, remix, and play HTML5 browser games. Sign in with Farcaster, World, MetaMask, or WalletConnect.
- [Remix on Farcaster](https://warpcast.com/~/mini-apps) — #1 gaming Mini App on both Farcaster and World App. 570,000+ players, 800+ games, 17M+ plays.
- [Farcade (Archive)](https://farcade.io) — Original Farcade branding, now redirects to Remix.

### ⚡ Snap Apps
Snap Apps (SNAPs) are standalone apps spun out of top-performing Remix games — distributed across Base, Farcaster, World App, and the web with their own URL and listing.

**Eligibility requirements to become a Snap App:**
- 1,000+ total plays
- 500+ unique players
- 25+ favorites
- 4+ star rating

Once eligible, converting to a Snap App is **completely free**. Snap Apps get push notifications, analytics, custom domains, and cross-platform discoverability.

### 🛠 Developer SDK
- [@farcade/game-sdk](https://www.npmjs.com/package/@farcade/game-sdk) — Official SDK for integrating HTML5 games with Remix. Handles game lifecycle, haptic feedback, mute state, multiplayer, and in-app purchases.
- [farcade/game-sdk on GitHub](https://github.com/farcade/game-sdk) — Source code and documentation.

**Core SDK integration pattern:**
```javascript
// SDK is injected automatically by Remix when game is uploaded
const sdk = window.FarcadeSDK;

await sdk.ready(); // Hide splash screen, signal game is loaded

sdk.actions.gameOver({ score: 1500 }); // Submit score / end session

sdk.onPlayAgain(() => { resetGame(); }); // Handle replay

sdk.onToggleMute(({ isMuted }) => { setMuted(isMuted); }); // Audio control

sdk.actions.hapticFeedback(); // Trigger haptics on mobile (use sparingly)
```

> **Note:** When you upload your game code to Remix, the SDK `<script>` tag is injected automatically — you do not need to add it manually.

### 🎮 Game Development Tips for Remix
- Build **single-file HTML5 games** — Remix hosts everything in one `.html` file
- Use **Canvas API** or **Phaser 3** for game rendering
- Keep games **under 5MB** for fast load times
- Design for **mobile-first** — most players are on phones
- Add **sound effects** and respect the `onToggleMute` callback
- Call `sdk.actions.gameOver()` every session — this powers leaderboards and analytics
- Use `hapticFeedback()` for impactful moments (collisions, level-ups, deaths)
- Aim for **short session loops** (30–90 seconds) for maximum replays

### 📦 Supported Game Technologies
| Tech | Notes |
|---|---|
| Vanilla HTML5 Canvas | ✅ Recommended for simplicity |
| Phaser 3 | ✅ Most popular choice in the ecosystem |
| PixiJS | ✅ Works great for 2D rendering |
| Three.js | ⚠️ Works but heavy — optimize carefully |
| Unity WebGL | ❌ Not supported (too large) |
| React | ⚠️ Possible but overkill for most games |

### 💰 Monetization
- **In-app purchases** — Sell items, skins, or power-ups via `sdk.actions.purchase()`
- **Ad revenue share** — Remix takes a platform cut from ads served in your game
- **Boosted visibility** — Pay for promoted placement in the Remix feed
- **Snap App launch** — Eligible games get standalone distribution, increasing earning potential

### 🏆 Game Jams & Events
- Remix regularly hosts **game jams** with USDC prizes — follow [@remixgg](https://warpcast.com/remixgg) on Farcaster for announcements
- Past collaborations: Pudgy Penguins ($20K jam), various Base ecosystem partners

### 📰 Further Reading
- [Farcade Rebrands to Remix — PlayToEarn](https://playtoearn.com/news/farcade-rebrands-to-remix-and-launches-snap-apps)
- [Remix Raises $5M Seed — Blockworks](https://blockworks.co/news/remix-5m-seed-funding)
- [What Are Snap Apps? — iGaming.org](https://igaming.org/gaming-news/farcade-rebrands-to-remix-and-launches-snap-apps/)

---

## 🛠 SDKs & Libraries

> Build on Farcaster with these developer tools.

### Official
- [@farcaster/miniapp-sdk](https://github.com/farcasterxyz/miniapps) — Official JavaScript SDK for Mini Apps. Auth, wallet, notifications, client communication.
- [@farcaster/create-mini-app](https://miniapps.farcaster.xyz/docs/getting-started) — CLI to scaffold a new Mini App project.
- [farcaster-js](https://github.com/standard-crypto/farcaster-js) — General-purpose JavaScript/TypeScript interface to Farcaster.
- [farcaster-py](https://github.com/a16z/farcaster-py) — General-purpose Python interface for the Warpcast API.

### Third-Party
- [@neynar/nodejs-sdk](https://github.com/neynarxyz/nodejs-sdk) — Official Neynar Node.js SDK: read/write APIs, webhooks, notifications.
- [@neynar/react](https://github.com/neynarxyz/react) — React hooks and UI components including `useMiniApp()` hook.
- [frog](https://frog.fm) — TypeScript framework for building Farcaster Frames with great DX.
- [frames.js](https://framesjs.org) — Open-source Frames library with built-in debugger.
- [farcaster-solidity](https://github.com/pavlovdog/farcaster-solidity) — Solidity libraries for verifying Farcaster messages on-chain.
- [AuthKit / SIWF](https://docs.farcaster.xyz/auth-kit/) — Sign In with Farcaster — add Farcaster login to any app.
- [react-farcaster-embed](https://github.com/pugson/react-farcaster-embed) — React component for embedding Farcaster casts on your site.

### Wallet & Web3
- [Wagmi](https://wagmi.sh) — React hooks for Ethereum. Standard pairing for Farcaster Mini Apps.
- [viem](https://viem.sh) — TypeScript Ethereum interface, compatible with Farcaster's injected EIP-1193 wallet.
- [OnchainKit](https://onchainkit.xyz) — Coinbase's toolkit with Frame components and Base integrations.
- [RainbowKit](https://rainbowkit.com) — Wallet connection UI, works with Farcaster embedded wallets.

---

## 🔌 APIs & Infrastructure

> Services for reading and writing Farcaster data at scale.

- [Neynar](https://neynar.com) — The leading Farcaster infrastructure platform. APIs, webhooks, indexers, AuthKit, analytics.
- [Airstack](https://airstack.xyz) — Composable Web3 APIs combining Farcaster + ENS + Base + Zora + XMTP data in one query.
- [Pinata](https://pinata.cloud/farcaster) — Free and open Farcaster APIs for casts, users, and channels.
- [Warpcast API](https://docs.warpcast.com) — Official Warpcast client API (public, primarily read-focused).
- [Phrasetown API](https://phrasetown.com) — Third-party Farcaster client with a useful public API.
- [Neynar SQL Playground](https://data.neynar.com) — Query real-time Farcaster data with raw SQL.
- [Dune Analytics](https://dune.com/browse/dashboards?q=farcaster) — Community dashboards for onchain Farcaster metrics.

---

## 🖼 Frames

> Interactive embed cards within Farcaster casts. The predecessor to Mini Apps, still widely used.

- [Farcaster Frames Spec](https://docs.farcaster.xyz/developers/frames/) — Official Frames protocol specification.
- [Frog](https://frog.fm) — Most popular framework for building Frames in TypeScript.
- [frames.js](https://framesjs.org) — Open-source Frames library with a rich local debugger.
- [OnchainKit Frames](https://onchainkit.xyz) — Coinbase's Frames toolkit, optimized for Base.
- [Thirdweb Frames Starter](https://thirdweb.com/frames) — Quick-start Frame template.
- [Farcaster.vote](https://farcaster.vote) — Verifiable, decentralized polls using Frames.
- [Composecast](https://composecast.xyz) — Privacy-preserving, MIT-licensed compose cast gateway Frame.

---

## 🤖 Bots

> Automated accounts you can @mention in casts to trigger actions.

| Bot | Example Usage | Description |
|---|---|---|
| @remindme | `@remindme 3 days` | Set a reminder on any cast |
| @launch | `@launch My Project` | Post to Launchcaster |
| @perl | `@perl Design` | Save a cast as a bookmark |
| @mintit | `@mintit` | Mint any cast as an NFT |
| @alert | via Alertcaster | Get notified for keyword matches |
| @survey | `@survey` | Bookmark for Ponder surveys |
| @paragraph | — | Summarizes Paragraph articles in your feed |
| @bountybot | `@bountybot $50 Fix this bug` | Create a public bounty |
| @translate | `@translate Turkish` | Translate any cast to a language |

### Open-Source Bot Resources
- [Neynar Farcaster Examples](https://github.com/neynarxyz/farcaster-examples) — Collection of open-source bots and Mini Apps.
- [Farcaster Survey Bot](https://github.com/farcasterxyz/survey-bot) — Open-source NodeJS bot for posting surveys.
- [fario CLI](https://github.com/vrypan/fario) — Python command-line tools for Farcaster power users.

---

## 📊 Analytics

> Data dashboards and tracking for Farcaster protocol and users.

- [Farcaster Network](https://farcaster.network) — Protocol-wide dashboard: DAU, casts per day, channel growth.
- [Casterscan](https://casterscan.com) — Block explorer for Farcaster casts, profiles, and hubs. ([GitHub](https://github.com/casterscanning/casterscan))
- [Farcaster Insights](https://farcasterinsights.com) — Network-level analytics and protocol metrics.
- [CastSense](https://castsense.com) — User and channel-level engagement analytics.
- [Trendcaster](https://trendcaster.com) — Personal analytics: follower growth, top casts, engagement rates.
- [Intelligent](https://intelligent.so) — Advanced creator analytics and audience management.
- [SQLCaster](https://sqlcaster.com) — Query Farcaster data with raw SQL.
- [Eigencaster](https://eigencaster.com) — Farcaster profile ranking using EigenTrust algorithm.
- [Neynar SQL Playground](https://data.neynar.com) — Real-time SQL access to the full Farcaster dataset.

---

## 🧰 Tools & Utilities

> Everyday tools for Farcaster users and developers.

### User Tools
- [Sharecaster](https://sharecaster.com) — Create clean, preview-rich shareable links to any cast.
- [Searchcaster](https://searchcaster.xyz) — Raycast extension for searching Farcaster.
- [CastStorage](https://caststorage.com) — Monitor your Farcaster hub storage usage.
- [fcstr](https://fcstr.xyz) — Generate RSS, Atom, and JSON feeds for users and channels.
- [Fardrop](https://fardrop.xyz) — Build token allowlists from your Farcaster followers.
- [Hatecast](https://hatecast.xyz) — Track follows and unfollows.
- [Farcaster Circle](https://farcaster.adamamcbride.com) — Visualize your cast interaction network.
- [Farcaster.vote](https://farcaster.vote) — Create verifiable, decentralized polls.

### Developer Tools
- [Warpcast Dev Mode](https://warpcast.com/~/developers) — Official tools: manifest builder, Mini App preview, embed auditor.
- [Neynar Debugger](https://docs.neynar.com/docs/debugging-tools) — Debug Farcaster API calls and webhooks.
- [Cast Syndication](https://github.com/pugson/syndicate-farcaster) — Syndicate Farcaster casts to a static site or blog via JavaScript.
- [farcaster-scraper](https://github.com/neynarxyz/farcaster-scraper) — CLI for scraping Farcaster content via Neynar.

---

## 📚 Learning

> Docs, tutorials, and guides to get you building on Farcaster.

### Official Documentation
- [Farcaster Docs](https://docs.farcaster.xyz) — Complete protocol documentation: spec, Hub API, contracts, auth.
- [Mini Apps Docs](https://miniapps.farcaster.xyz) — Build, test, and deploy Farcaster Mini Apps.
- [Neynar Docs](https://docs.neynar.com) — API reference, tutorials, and code examples.

### Guides & Tutorials
- [Getting Started — Mini Apps](https://miniapps.farcaster.xyz/docs/getting-started) — Official quick-start using `@farcaster/create-mini-app`.
- [Convert a Web App to a Mini App](https://docs.neynar.com/docs/convert-web-app-to-mini-app) — Add `sdk.actions.ready()` to any web app and ship it.
- [Build on Farcaster: The Ultimate 101](https://dtech.vision/farcaster/start/) — Bots, Mini Apps, agents, viral growth loops — comprehensive walkthrough.
- [What Are Farcaster Mini Apps?](https://www.onchainsite.xyz/blog/what-are-farcaster-miniapps) — Conceptual and technical deep-dive.
- [20 Mini Apps to Try](https://www.bankless.com/read/20-farcaster-mini-apps) — Builder inspiration roundup by Bankless (April 2025).
- [Neynar Farcaster Examples](https://github.com/neynarxyz/farcaster-examples) — Open-source Mini App examples to fork and learn from.
- [a16z Awesome Farcaster](https://github.com/a16z/awesome-farcaster) — The original curated list maintained by a16z.

### Videos
- [Farcaster YouTube](https://www.youtube.com/@farcasterxyz) — Official videos, protocol updates, and ecosystem demos.

---

## 🌐 Community

> DAOs, events, channels, and community groups.

- [Purple DAO](https://purple.construction) — DAO dedicated to funding and proliferating the Farcaster ecosystem.
- [FarCon](https://farcon.xyz) — Annual Farcaster unconference for physical community connection.
- [/dev channel](https://warpcast.com/~/channel/dev) — Builder-focused channel on Farcaster.
- [/farcaster channel](https://warpcast.com/~/channel/farcaster) — Main Farcaster community channel.
- [/base channel](https://warpcast.com/~/channel/base) — Base Network community, deeply integrated with Farcaster.
- [Farcaster Discord](https://discord.gg/farcaster) — Official developer Discord server.

### Tokens & Economy
- [DEGEN](https://www.degen.tips) — Community memecoin native to Farcaster. Gas token for the Degen L3 chain. $50M+ airdropped to active casters.
- [Farcaster Pro](https://warpcast.com/pro) — $120/year subscription; 10K-char casts, 100% of revenue redistributed to creators weekly.
- [Warpcast Rewards](https://warpcast.com/~/rewards) — $25,000+ USDC distributed weekly to top active casters.

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a PR.

**To add a resource:**
1. Fork this repo
2. Add your link under the correct category
3. Format: `[Name](url) — Short, clear description.`
4. Open a pull request with a brief explanation

Please ensure the resource is: working, genuinely useful, and not already listed.

---

## 📄 License

[MIT](LICENSE) © [ftimurlenk](https://github.com/ftimurlenk)

---

<div align="center">

⭐ **Star this repo** if it's useful — it helps other Farcaster builders find it!

Made with 💜 for the Farcaster builder community

</div>
