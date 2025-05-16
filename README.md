# GameFun 🎮🪙

Empowering creators with on-chain community currencies

GameFun is a decentralized platform where verified YouTubers, Twitch streamers, and gamers can launch their own meme coins on the Solana blockchain. These coins represent the creator's brand and community identity — and can be collected, traded, and supported by their fans and subscribers.

---

✨ **Key Features**

* 🔗 YouTube/Twitch OAuth verification
* 🪙 Meme Coin Creator (with image, metadata, supply, price, etc.)
* 🖼️ Image + metadata storage via NFT.Storage (IPFS)
* ⚙️ SPL Token minting + Metaplex metadata attachment
* 🔐 Phantom wallet integration
* 📊 Real-time dashboard for each coin
* 📤 Fans can buy/sell meme coins as collectibles
* 🛒 Marketplace interface for coin discovery and trading

---

🛍️ **Use Case: Token Marketplace for Subscribers**

Subscribers can support their favorite creators by buying their meme coins. These tokens are tradable—allowing fans to speculate, collect, or engage in creator-led ecosystems. Each coin is visible in a marketplace dashboard where supply, pricing, and creator profiles are transparent.

---

🛠️ **Tech Stack**

* Solana Blockchain
* SPL Token + Metaplex Token Metadata
* NFT.storage (IPFS image + JSON)
* Supabase (Database & Auth)
* Phantom Wallet (Web3 Auth)
* React + Tailwind CSS (Frontend)

---

🚀 **How It Works**

1. Creators sign in via YouTube or Twitch OAuth
2. They create their meme coin (name, symbol, image, supply, etc.)
3. Image and metadata are uploaded to IPFS
4. SPL token is minted with the metadata attached
5. Coin is launched and listed on the marketplace
6. Fans can view, collect, and trade creator tokens

---

📦 **Installation**

```bash
git clone https://github.com/yourusername/gamefun.git
cd gamefun

npm install
```

Create a `.env` file with your credentials:

```
VITE_SUPABASE_URL=your-supabase-url
VITE_SUPABASE_ANON_KEY=your-anon-key
VITE_NFT_STORAGE_API_KEY=your-nft-storage-api-key
VITE_SOLANA_RPC_URL=https://api.mainnet-beta.solana.com
VITE_APP_DOMAIN=http://localhost:5173
```

Start the development server:

```bash
npm run dev
```

---

✅ **Project Status**

* ✔ MVP complete
* 🚧 Token trading UI in progress
* 🚀 Integration with Raydium and Jupiter coming soon

---

🧠 **Inspiration**

GameFun was built to empower creators and let their communities support them not just with views, but with on-chain loyalty and ownership. It brings social energy to blockchain in a fun and simple way.

---

📜 **License**

MIT

---

Let me know if you want me to help add badges, roadmap, contributors, or demo video links!
