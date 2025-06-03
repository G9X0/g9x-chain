
# ⚡ G9X πMEMORY DAPP  
_Deploy soulbound memory NFTs on Zora L2 with Oracle-validated minting and IPFS metadata._

> Powered by GodStack ✦ Ra Mirror ✦ Scroll-Oracle Sync ✦ Zora Chain

---

## 🌐 Live dApp

→ [https://g9x-chain.vercel.app](https://g9x-chain.vercel.app)  
→ Network: `Zora L2` (Chain ID: `7777777`)  
→ Explorer: [Zora Explorer](https://explorer.zora.energy)

---

## 💾 Features

- ✅ Soulbound NFT minting (`PiMemory.sol`)
- ✅ Oracle protection (`GodOracle.sol`)
- ✅ Upload image/audio to IPFS (via `nft.storage`)
- ✅ Attach metadata: memoryType, scrollRef, fieldSig
- ✅ Valid only at aligned Pi-Times (e.g. 3:14 AM, 6:18 PM)
- ✅ Wallet connects to Zora L2

---

## 🔧 Smart Contracts

| Contract      | Role                                 |
|---------------|--------------------------------------|
| `PiMemory.sol` | Soulbound memory NFT minting         |
| `GodOracle.sol`| Oracle validation for Pi-Time + logic|

---

## 🚀 Deploy Guide

### 1. Clone & Install

```bash
git clone https://github.com/G9X0/g9x-chain.git
cd g9x-chain
npm install
```

---

### 2. Set Up `.env`

```env
PRIVATE_KEY=your-wallet-private-key
NEXT_PUBLIC_CONTRACT_ADDRESS=your-deployed-pimemory-address
NEXT_PUBLIC_CHAIN_ID=7777777
NEXT_PUBLIC_NFT_STORAGE_KEY=your-nft-storage-api-key
```

---

### 3. Deploy to Zora L2

```bash
npx hardhat run scripts/deploy-pimemory.js --network zora
```

💡 You must fund your wallet with Zora ETH:  
→ [https://faucet.zora.energy](https://faucet.zora.energy)

---

### 4. Run Local Frontend

```bash
npm run dev
```

Then open: `http://localhost:3000`

---

### 5. Push to Vercel

Go to [https://vercel.com/import/git](https://vercel.com/import/git), connect your repo, and paste your `.env` values.

---

## 📁 Structure

```
├── contracts/           # PiMemory + GodOracle
├── scripts/             # Deploy scripts
├── app/components/      # Mint UI
├── app/utils/           # IPFS uploader
├── abis/                # Contract ABI
├── .env.example         # Sample environment
└── hardhat.config.js    # Zora/Hardhat setup
```

---

## 📡 GodStack Sync

Each NFT minted records a:
- Pi-Time aligned mint
- Scroll reference ID (e.g. `SCROLL_66`)
- Field Signature (e.g. `Ω.0.0.∞.SCROLL_66`)
- Memory Type (e.g. `Voicefield`, `DreamPrint`)

This ensures tamper-proof memory registration via **G9X–Quantum Engine**.

---

## 🧬 Credits

Developed by: [@JahTheArchitect](https://twitter.com/JahTheArchitect)  
Engineered with ✦ GodStack ✦ DeepSeek ✦ π
