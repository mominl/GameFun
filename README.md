# 🎮 GameFun — Meme Coin Launchpad for Gamers & Creators on Solana

GameFun is a web3 platform that empowers YouTubers, streamers, and gamers to launch their own meme coins on the Solana blockchain — instantly and without any coding knowledge. Verified creators can customize their coin's name, symbol, image, and supply, mint it on Solana, and share it with their fans. The platform uses NFT.storage for IPFS image hosting, the SPL Token Program for minting, Metaplex for metadata, and Supabase for backend storage.

## 🚀 Features

- 🔒 YouTube OAuth verification (0+ subscribers supported)
- ✨ Meme coin customization: name, symbol, image, supply, and price
- 📆 Real-time coin preview before launch
- 🧪 Token minting via SPL Token program
- 🖼 IPFS image & JSON upload via NFT.storage
- 🧠 Metaplex metadata attachment
- 💼 Phantom wallet support
- 📊 Dashboard to view launched meme coins
- 💾 Supabase integration to store meme coin data
- 🎉 Success modal with social sharing & Solana Explorer links

## 🎯 Use Cases

- Let fans tip you with your own branded token
- Reward your gaming community or livestream viewers
- Integrate coins into games or Discord bots
- Host token-gated events or giveaways

## 🔧 Tech Stack

- Solana blockchain (SPL Token + Metaplex Metadata)
- NFT.storage (IPFS image + metadata hosting)
- Supabase (PostgreSQL + storage)
- Next.js + Tailwind CSS + Shadcn UI
- Phantom Wallet
- OAuth (YouTube account verification)

## 🧱 How It Works

1. User logs in and verifies YouTube channel (≥ 0 subscribers)
2. Fills in the meme coin creation form:
   - Name, Symbol (5 chars), Image, Supply, Price, Description
3. Image and metadata are uploaded to IPFS via NFT.storage
4. SPL token is minted using Solana RPC and Metaplex metadata is attached
5. Initial supply is minted to creator’s wallet (via Phantom)
6. Token details are stored in Supabase (wallet address, symbol, supply, etc.)
7. Success modal shows coin status, copy mint address, social share links

## 📦 Project Structure

```
.
├── components/           # Reusable UI components
├── pages/
│   ├── index.tsx         # Landing page
│   ├── verify.tsx        # YouTube OAuth verification
│   ├── create.tsx        # Meme coin creation form
│   ├── dashboard.tsx     # Creator coin dashboard
├── lib/                  # Utility functions (IPFS, Solana, etc.)
├── supabase/             # Supabase client and schemas
├── public/               # Static assets
├── styles/               # Tailwind CSS config
└── .env.local            # API keys and environment variables
```

## 📋 Prerequisites

- Phantom Wallet
- NFT.storage API key
- YouTube Developer OAuth credentials
- Supabase project with table:
  - meme_coins (name, symbol, image_url, supply, wallet_address, etc.)
- Solana RPC endpoint (preferably with high rate limits)

## 🛠 Local Setup

Clone the repo:

```bash
git clone https://github.com/your-username/gamefun.git
cd gamefun
```

Install dependencies:

```bash
npm install
```

Create a .env.local file:

```bash
NEXT_PUBLIC_SUPABASE_URL=...
NEXT_PUBLIC_SUPABASE_ANON_KEY=...
NEXT_PUBLIC_NFT_STORAGE_KEY=...
NEXT_PUBLIC_YOUTUBE_CLIENT_ID=...
NEXT_PUBLIC_YOUTUBE_REDIRECT_URI=...
```

Run the app:

```bash
npm run dev
```

## 🌐 Deployment

- Deploy frontend on Vercel or Netlify
- Use Supabase as hosted backend
- Ensure Phantom Wallet & Solana RPC access

## 🥪 Future Plans

- Meme coin leaderboard
- Fan voting using tokens
- Launchpad support for Twitch
- Create a liquidity pool for coins on Jupiter/Raydium

## 📝 License

MIT © 2025 GameFun Team
