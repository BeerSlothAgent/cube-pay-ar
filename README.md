# CubePay Virtual Terminal - Monorepo

A unified codebase for the CubePay virtual terminal payment system, integrating AR viewer, AgentSphere marketplace, E-commerce shop, and On/Off ramp functionality.

## 🏗️ Repository Structure

```
cube-pay-ar/
├── apps/
│   ├── ar-viewer/          # Main AR viewer & AgentSphere marketplace
│   ├── eshop/              # E-commerce shop (submodule)
│   └── on-off-ramp/        # Payment gateway on/off ramp (submodule)
├── packages/
│   ├── shared/             # Shared utilities, types, and components
│   └── payment-engine/     # Core payment processing engine
├── docs/                   # Documentation and guides
└── sql/                    # Database schemas and migrations
```

## 📦 Applications

### AR Viewer (`apps/ar-viewer`)
- **Purpose**: AR-based agent viewer with QR payment integration
- **Tech Stack**: React, Three.js, Vite
- **Features**: 
  - 3D agent visualization
  - AR QR code scanning
  - AgentSphere marketplace
  - Multi-chain wallet integration (EVM, Solana, Hedera)
  - Payment modal with QR code generation

### E-shop (`apps/eshop`)
- **Purpose**: E-commerce storefront with crypto payments
- **Tech Stack**: React, TypeScript, Vite
- **Integration**: Uses CubePay virtual terminal for checkout

### On/Off Ramp (`apps/on-off-ramp`)
- **Purpose**: Fiat to crypto conversion gateway
- **Integration**: Payment processing for fiat transactions

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Git

### Installation

1. **Clone the repository with submodules:**
```bash
git clone --recursive https://github.com/BeerSlothAgent/cube-pay-ar.git
cd cube-pay-ar
```

2. **Install dependencies for all apps:**
```bash
npm run install:all
```

Or install individually:
```bash
# AR Viewer
cd apps/ar-viewer && npm install

# E-shop
cd apps/eshop && npm install

# On/Off Ramp
cd apps/on-off-ramp && npm install
```

### Development

Run individual applications:

```bash
# AR Viewer
npm run dev:ar-viewer

# E-shop
npm run dev:eshop

# On/Off Ramp
npm run dev:on-off-ramp
```

### Building

Build all applications:
```bash
npm run build:all
```

Or build individually:
```bash
npm run build:ar-viewer
npm run build:eshop
npm run build:on-off-ramp
```

## 🔧 Configuration

### Environment Variables

Each application has its own `.env` file:

- `apps/ar-viewer/.env` - Supabase, wallet configs
- `apps/eshop/.env` - Shop API keys
- `apps/on-off-ramp/.env` - Payment gateway credentials

See `.env.example` in each app directory.

## 🏛️ Architecture

### Monorepo Benefits
- **Unified development**: Make changes across all apps in a single branch
- **Atomic commits**: Commit related changes together
- **Shared packages**: Reuse code via `packages/`
- **Simplified CI/CD**: Build and deploy all apps together

### Integration Points

The virtual terminal integrates across all apps:
- **Payment Engine**: Shared across all applications
- **QR Generation**: Used by AR viewer and e-shop
- **Wallet Connect**: Unified wallet connection logic
- **Database**: Shared Supabase instance for agent data

## 📚 Documentation

- [API Documentation](./docs/API_Documentation.md)
- [Database Schemas](./docs/Schemas.md)
- [Backend Integration](./docs/Backend.md)
- [Changelog](./docs/Changelog.md)

## 🔄 Submodules

This repo uses git submodules for `eshop` and `on-off-ramp`:

```bash
# Update submodules
git submodule update --remote

# Initialize submodules (if cloned without --recursive)
git submodule init
git submodule update
```

## 🛠️ Tech Stack

- **Frontend**: React 19, Vite
- **3D/AR**: Three.js, React Three Fiber
- **Blockchain**: 
  - EVM: ThirdWeb, ethers.js
  - Solana: @solana/web3.js
  - Hedera: Hashpack integration
- **Database**: Supabase
- **Styling**: Tailwind CSS, Radix UI
- **QR Codes**: qrcode.react

## 🔗 Chainlink CCIP Routes

### Supported Cross-Chain Routes

CubePay supports Chainlink CCIP for secure cross-chain transfers across the following networks:

| Source Network | Destination Network | CCIP Router Address | Status |
|----------------|---------------------|---------------------|---------|
| Ethereum Sepolia | Polygon Amoy | `0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59` | ✅ Active |
| Polygon Amoy | Ethereum Sepolia | `0x9C32fCB86BF0f4a1A8921a9Fe46de3198bb884B2` | ✅ Active |
| Avalanche Fuji | Ethereum Sepolia | `0xF694E193200268f9a4868e4Aa017A0118C9a8177` | ✅ Active |
| Ethereum Sepolia | Avalanche Fuji | `0x0BF3dE8c5D3e8A2B34D2BEeB17ABfCeBaf363A59` | ✅ Active |
| Arbitrum Sepolia | Ethereum Sepolia | `0x2a9C5afB0d0e4BAb2BCdaE109EC4b0c4Be15a165` | ✅ Active |
| Base Sepolia | Ethereum Sepolia | `0xD3b06cEbF099CE7DA4AcCf578aaebFDBd6e88a93` | ✅ Active |
| Optimism Sepolia | Ethereum Sepolia | `0x114A20A10b43D4115e5aeef7345a1A71d2a60C57` | ✅ Active |

### CCIP Chain Selectors

```javascript
const CCIP_CHAIN_SELECTORS = {
  ETHEREUM_SEPOLIA: "16015286601757825753",
  POLYGON_AMOY: "16281711391670634445",
  AVALANCHE_FUJI: "14767482510784806043",
  ARBITRUM_SEPOLIA: "3478487238524512106",
  BASE_SEPOLIA: "10344971235874465080",
  OPTIMISM_SEPOLIA: "5224473277236331295"
};
```

## 💰 USDC Contract Addresses

### Testnet Contracts

| Network | USDC Contract Address | Decimals |
|---------|----------------------|----------|
| **Ethereum Sepolia** | `0x1c7D4B196Cb0C7B01d743Fbc6116a902379C7238` | 6 |
| **Polygon Amoy** | `0x41E94Eb019C0762f9Bfcf9Fb1E58725BfB0e7582` | 6 |
| **Avalanche Fuji** | `0x5425890298aed601595a70AB815c96711a31Bc65` | 6 |
| **Arbitrum Sepolia** | `0x75faf114eafb1BDbe2F0316DF893fd58CE46AA4d` | 6 |
| **Base Sepolia** | `0x036CbD53842c5426634e7929541eC2318f3dCF7e` | 6 |
| **Optimism Sepolia** | `0x5fd84259d66Cd46123540766Be93DFE6D43130D7` | 6 |

### Mainnet Contracts

| Network | USDC Contract Address | Decimals |
|---------|----------------------|----------|
| **Ethereum Mainnet** | `0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48` | 6 |
| **Polygon** | `0x3c499c542cEF5E3811e1192ce70d8cC03d5c3359` | 6 |
| **Avalanche C-Chain** | `0xB97EF9Ef8734C71904D8002F8b6Bc66Dd9c48a6E` | 6 |
| **Arbitrum One** | `0xaf88d065e77c8cC2239327C5EDb3A432268e5831` | 6 |
| **Base** | `0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913` | 6 |
| **Optimism** | `0x0b2C639c533813f4Aa9D7837CAf62653d097Ff85` | 6 |

### Additional Supported Networks

| Network | USDC Contract Address | Decimals |
|---------|----------------------|----------|
| **Solana Devnet** | `4zMMC9srt5Ri5X14GAgXhaHii3GnPAEERYPJgZJDncDU` | 6 |
| **Solana Mainnet** | `EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v` | 6 |
| **Hedera Testnet** | `0.0.429274` | 6 |
| **Hedera Mainnet** | `0.0.456858` | 6 |

> **Note**: Always verify contract addresses before making transactions. USDC uses 6 decimals across all networks.

## 🤝 Contributing

1. Create a feature branch
2. Make your changes
3. Commit with descriptive messages
4. Push and create a pull request

## 📄 License

MIT License - see LICENSE file for details

## 👥 Team

BeerSlothAgent - [GitHub](https://github.com/BeerSlothAgent)
