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

## 🤝 Contributing

1. Create a feature branch
2. Make your changes
3. Commit with descriptive messages
4. Push and create a pull request

## 📄 License

MIT License - see LICENSE file for details

## 👥 Team

BeerSlothAgent - [GitHub](https://github.com/BeerSlothAgent)
