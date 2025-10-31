# CubePay AR - Spatial Augmented FinApp

## 🌟 **Next-Generation Payment Platform with AR Integration**

CubePay AR is a revolutionary Spatial Augmented Finance Application that transforms how merchants accept payments through augmented reality, virtual terminals, and blockchain technology. Part of the complete AgentSphere ecosystem, it enables seamless crypto and fiat payments without physical devices.

### 🚀 **Current Repository: Full Spatial Payment System**

**Complete CubePay AR Implementation - Spatial Augmented FinApp**

## 💎 **Revolutionary Payment Features**

### **1. Virtual Terminal Payments** 🖥️
Merchants can deploy their own **virtual payment terminals** directly through AR, eliminating the need for physical card readers or POS devices. Each terminal is:
- Deployed instantly via QR code scanning
- Accessible in augmented reality through any smartphone
- Capable of processing crypto and fiat payments
- Fully customizable with merchant branding

### **2. Revolut Bank Integration** 🏦
Seamless bank QR payment processing through **Revolut Business API**:
- **Bank QR Payments**: Generate instant QR codes for direct bank transfers
- **Virtual Card Payments**: Dynamic virtual card generation for online transactions
- **No Physical Devices Required**: All payments processed through virtual terminals
- **Instant Settlement**: Real-time payment confirmation and fund transfer
- **Multi-Currency Support**: Accept payments in multiple fiat currencies

### **3. Cross-Chain Crypto Payments** ⛓️
Native cryptocurrency payment support across multiple blockchain networks:
- **EVM Networks**: Ethereum, Polygon, Base, Avalanche, Arbitrum, Optimism, Morph
- **Solana**: High-speed SPL token payments
- **Hedera**: Enterprise-grade HBAR and token transfers
- **CCIP Cross-Chain**: Chainlink CCIP-powered cross-chain USDC transfers
- **Multi-Wallet Support**: MetaMask, WalletConnect, Phantom, HashPack

### **4. Cross-Platform Payment Processing** 🌐
Universal payment acceptance across all platforms:
- **Web**: Full desktop and mobile web support
- **Mobile AR**: Native AR experience on iOS and Android
- **Progressive Web App**: Installable mobile experience
- **QR Code Integration**: Instant payment links accessible anywhere

### **5. Revolutionary Tokenization Alternative** 🔄
**Replacing Traditional Card Tokenization** - Instead of storing sensitive card data:
- Merchants deploy their own **virtual terminals** in AR space
- Payments redirect to user's **personally deployed terminal**
- Users control their payment flow through their own infrastructure
- No card data storage or tokenization needed
- Complete payment sovereignty and security

### **6. Device-Free Merchant Operations** 📱
Merchants operate **without any physical payment devices**:
- No card readers required
- No POS terminals to maintain
- No hardware costs or maintenance
- Virtual terminals deployed instantly via AR
- All operations managed through smartphone or web browser

### **7. Dynamic Fee Structure** 💰
Transparent, flexible fee system:
- **Deployment Fees**: One-time AR agent/terminal deployment
- **Interaction Fees**: Per-transaction processing fees
- **Cross-Chain Fees**: CCIP bridge fees for cross-chain transfers
- **Network Gas Fees**: Blockchain transaction costs (paid in native tokens)
- All fees displayed upfront before transaction confirmation

## 🏗️ **Spatial Augmented FinApp Architecture**

```
┌─────────────────────────────────────────────────────────────┐
│              CubePay AR - Spatial FinApp                    │
│         Complete Payment Terminal Ecosystem                 │
└─────────────────────────────────────────────────────────────┘
                              │
        ┌─────────────────────┴─────────────────────┐
        │                                           │
        ▼                                           ▼
┌───────────────────┐                    ┌──────────────────┐
│  Virtual Terminal │                    │  Payment Gateway │
│    Deployment     │                    │   Integration    │
└───────────────────┘                    └──────────────────┘
        │                                           │
        ├─ AR QR Scanning                          ├─ Revolut Bank API
        ├─ 3D Terminal Models                      ├─ Virtual Cards
        ├─ Geolocation Anchoring                   ├─ Bank QR Codes
        └─ Real-time Updates                       └─ Instant Settlement
        │                                           │
        ▼                                           ▼
┌───────────────────────────────────────────────────────────┐
│              Blockchain Payment Processing                │
├───────────────────────────────────────────────────────────┤
│  • EVM Networks (Polygon, Base, Ethereum, etc.)          │
│  • Solana (SPL Tokens)                                   │
│  • Hedera (HBAR, Tokens)                                 │
│  • CCIP Cross-Chain Transfers                            │
│  • Multi-Wallet Support                                  │
└───────────────────────────────────────────────────────────┘
```

## 🎯 **Complete Feature Set**

### **Core Capabilities:**
- ✅ Full-stack web application with React + TypeScript
- ✅ Supabase database for real-time payment tracking
- ✅ AR/QR code payment terminal deployment
- ✅ Multi-blockchain integration (EVM, Solana, Hedera)
- ✅ Revolut virtual card and bank QR payments
- ✅ CCIP cross-chain USDC transfers
- ✅ Interactive map visualization and terminal management
- ✅ Dynamic fee calculation and display
- ✅ Real-time payment status updates

## 🚀 **Quick Start Guide**

### **Prerequisites:**

- Node.js 18+ and npm
- Git
- Modern web browser with WebRTC support
- Smartphone with camera for AR features (optional)
- Wallet: MetaMask, Phantom, or HashPack for crypto payments

### **Installation & Setup:**

1. **Clone and Navigate:**

   ```bash
   git clone https://github.com/BeerSlothAgent/cube-pay-ar.git
   cd cube-pay-ar
   ```

2. **Install Dependencies:**

   ```bash
   npm install
   ```

3. **Environment Variables:**
   Create a `.env` file with:

   ```env
   VITE_SUPABASE_URL=https://ncjbwzibnqrbrvicdmec.supabase.co
   VITE_SUPABASE_ANON_KEY=[your_key]
   VITE_SUPABASE_SERVICE_ROLE_KEY=[your_key]
   VITE_THIRDWEB_CLIENT_ID=[your_key]
   VITE_REVOLUT_SANDBOX_API_KEY=[your_key]
   ```

4. **Start Development Server:**

   ```bash
   npm run dev
   ```

5. **Access Application:**
   Open `http://localhost:5173` in your browser

## � **How It Works**

### **For Merchants:**

1. **Deploy Virtual Terminal** 🖥️
   - Scan QR code or use web interface
   - Terminal appears in AR at your location
   - Customize branding and payment options

2. **Accept Payments** 💳
   - Share terminal QR code with customers
   - Accept crypto or fiat payments instantly
   - No physical devices needed

3. **Manage Terminals** 📊
   - View real-time payment activity
   - Track multiple terminal locations
   - Access transaction history

### **For Customers:**

1. **Scan QR Code** 📱
   - Point camera at merchant's payment QR
   - View terminal in AR (optional)
   - See payment details and fees

2. **Choose Payment Method** 💰
   - Crypto: Select blockchain and token
   - Fiat: Use Revolut bank QR or virtual card
   - Cross-chain: CCIP transfers between networks

3. **Complete Payment** ✅
   - Review fees and total amount
   - Confirm transaction
   - Receive instant confirmation

## 💳 **Supported Payment Methods**

### **Cryptocurrency:**
- **USDC**: EVM networks, Solana
- **Native Tokens**: ETH, MATIC, SOL, HBAR, etc.
- **ERC-20/SPL Tokens**: All standard tokens supported

### **Fiat (via Revolut):**
- **Bank Transfer**: QR code direct bank payments
- **Virtual Cards**: Dynamic card generation for online payments
- **Multiple Currencies**: EUR, USD, GBP, and more

### **Cross-Chain:**
- **CCIP Transfers**: Seamless USDC transfers across chains
- **Multi-Network**: Send from one chain, receive on another
- **Automatic Bridging**: Chainlink CCIP handles the routing

## 🌐 **Supported Blockchain Networks**

### **EVM-Compatible Networks:**
```javascript
// Production Networks
Ethereum Mainnet
Polygon (MATIC)
Base (Coinbase L2)
Avalanche C-Chain
Arbitrum One
Optimism

// Testnet Networks
Polygon Amoy (Testnet)
Base Sepolia
Avalanche Fuji
Arbitrum Sepolia
Morph Holesky Testnet
```

### **Non-EVM Networks:**
- **Solana Devnet/Mainnet**: High-speed SPL token payments
- **Hedera**: Enterprise-grade HBAR and HTS token support

### **CCIP Cross-Chain Routes:**
```javascript
// Supported USDC Bridge Routes
Polygon Amoy ↔ Base Sepolia
Avalanche Fuji ↔ Polygon Amoy
Arbitrum Sepolia ↔ Base Sepolia
Optimism Sepolia ↔ Ethereum Sepolia

// USDC Contract Addresses (Testnet)
Polygon Amoy: 0x41e94eb019c0762f9bfcf9fb1e58725bfb0e7582
Base Sepolia: 0x036CbD53842c5426634e7929541eC2318f3dCF7e
Avalanche Fuji: 0x5425890298aed601595a70ab815c96711a31bc65
Arbitrum Sepolia: 0x75faf114eafb1BDbe2F0316DF893fd58CE46AA4d
```

## 🔐 **Security & Privacy Features**

### **Payment Security:**
- ✅ **No Card Data Storage**: Virtual terminals eliminate tokenization needs
- ✅ **User-Controlled Flow**: Payments redirect to user's own terminals
- ✅ **Blockchain Transparency**: All crypto transactions on-chain and verifiable
- ✅ **Multi-Signature Support**: Enhanced security for high-value transactions
- ✅ **Encrypted Communication**: End-to-end encryption for all payment data

### **Privacy Protection:**
- ✅ **Decentralized Infrastructure**: No central payment processor
- ✅ **Minimal Data Collection**: Only essential transaction information stored
- ✅ **User Sovereignty**: Complete control over payment terminals and data
- ✅ **GDPR Compliant**: Privacy-first architecture

## 🎯 **Use Cases**

### **Retail & Commerce:**
- Pop-up shops and market vendors
- Street food and mobile vendors
- Event ticketing and merchandise
- Service-based businesses

### **Digital & Remote:**
- E-commerce checkout integration
- Subscription and recurring payments
- Digital content and NFT sales
- International remittances

### **Enterprise:**
- B2B payment processing
- Multi-location retail chains
- Franchise payment systems
- Cross-border transactions
    │ • Landing   │  │ • NEAR Smart    │  │ • AR Camera     │
    │ • Landing   │  │ • Smart         │  │ • AR Camera     │
    │ • UI/UX     │  │   Contracts     │  │ • WebXR         │
    │ • Auth      │  │ • Filecoin      │  │ • A-Frame       │
    │ • Hub       │  │ • IPFS Storage  │  │ • GPS/Location  │
    │             │  │ • USDC Payments │  │ • Agent Render  │
    └─────────────┘  └─────────────────┘  └─────────────────┘
```

## 🛠️ **Technology Stack**

### **Frontend & UI:**
- **React 19** + TypeScript - Modern component architecture
- **Vite** - Lightning-fast build tooling
- **Tailwind CSS** - Utility-first styling
- **Framer Motion** - Smooth animations
- **React Router** - Client-side routing
- **shadcn/ui** - Beautiful component library

### **Blockchain & Web3:**
- **ThirdWeb SDK** - Multi-chain wallet integration
- **ethers.js** - Ethereum interaction
- **@solana/web3.js** - Solana blockchain integration
- **@hashgraph/sdk** - Hedera integration
- **Chainlink CCIP** - Cross-chain interoperability
- **MetaMask, WalletConnect, Phantom, HashPack** - Wallet support

### **Payment Processing:**
- **Revolut Business API** - Bank and virtual card payments
- **Revolut Bank QR** - Direct bank transfer QR codes
- **Dynamic Virtual Cards** - On-demand card generation
- **Multi-Currency Support** - Fiat payment processing

### **AR & 3D:**
- **A-Frame** - WebXR framework
- **Three.js** - 3D rendering engine
- **React Three Fiber** - React renderer for Three.js
- **@react-three/drei** - Useful helpers for R3F
- **WebRTC** - Camera access for AR
- **GPS/Geolocation APIs** - Location-based terminals

### **Backend & Database:**
- **Supabase** - Real-time PostgreSQL database
- **PostgreSQL** - Relational data storage
- **Real-time subscriptions** - Live payment updates
- **Row-level security** - Data protection

### **APIs & Services:**
- **Chainlink CCIP** - Cross-chain messaging
- **Revolut API** - Payment processing
- **Assembly AI** - Voice/audio processing (optional)
- **Google Maps API** - Location visualization

## 🚀 **Getting Started**

### **1. Clone All Repositories:**

```bash
# Main repository
git clone https://github.com/BeerSlothAgent/Agent-Sphere-1.git

# Blockchain + Storage + Payment integrations
git clone https://github.com/BeerSlothAgent/geospatila-agent-near-shade-integrations.git

# AR Viewer
git clone https://github.com/BeerSlothAgent/geospatial-agent-ar-viewer.git
```

### **2. Setup Main Repository:**

```bash
cd Agent-Sphere-1
npm install
cp .env.example .env
# Configure your environment variables
npm run dev
```

### **3. Setup Blockchain Integrations:**

```bash
cd geospatila-agent-near-shade-integrations
npm install
# Follow repository-specific setup instructions
```

### **4. Setup AR Viewer:**

```bash
cd geospatial-agent-ar-viewer
npm install
# Follow repository-specific setup instructions
```

## 🌐 **Environment Variables**

### **Main Repository (.env):**

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_key
VITE_THIRDWEB_CLIENT_ID=your_thirdweb_id
```

### **Additional Configuration:**

- See individual repository README files for specific setup instructions
- Each repository has its own environment configuration
- Cross-repository communication is handled via APIs and shared protocols

## 📦 **Project Structure**

```
cube-pay-ar/
├── src/
│   ├── components/           # React components
│   │   ├── ARViewer/        # AR camera and 3D rendering
│   │   ├── PaymentModals/   # Payment UI components
│   │   ├── WalletConnect/   # Wallet integration
│   │   └── Map/             # Location visualization
│   ├── services/            # Business logic
│   │   ├── revolutBankService.ts      # Bank QR payments
│   │   ├── revolutCardService.ts      # Virtual card generation
│   │   ├── evmPaymentService.ts       # EVM blockchain payments
│   │   ├── solanaPaymentService.ts    # Solana payments
│   │   ├── hederaPaymentService.ts    # Hedera payments
│   │   ├── ccipService.ts             # Cross-chain transfers
│   │   └── paymentProcessor.ts        # Unified payment handler
│   ├── lib/                 # Utilities and configs
│   │   ├── supabase.ts      # Database client
│   │   ├── thirdweb.ts      # Blockchain client
│   │   └── chains.ts        # Network configurations
│   └── hooks/               # Custom React hooks
├── public/
│   └── models/              # 3D models for AR terminals
├── eshop-sparkle-assets/    # E-commerce storefront
├── onofframp-cube-paygate/  # Fiat on/off ramp
└── docs/                    # Documentation
```

## 🔧 **Development**

### **Available Scripts:**

```bash
# Development
npm run dev              # Start dev server
npm run dev:backend      # Start backend API server
npm run dev:all          # Start both frontend and backend

# Building
npm run build            # Production build
npm run build:quick      # Quick development build
npm run build:mobile     # Mobile-optimized build
npm run build:netlify    # Netlify deployment build

# Testing & Quality
npm run lint             # Run ESLint
npm run preview          # Preview production build
```

### **Environment Configuration:**

```env
# Supabase Database
VITE_SUPABASE_URL=https://ncjbwzibnqrbrvicdmec.supabase.co
VITE_SUPABASE_ANON_KEY=your_anon_key
VITE_SUPABASE_SERVICE_ROLE_KEY=your_service_key

# ThirdWeb (Blockchain)
VITE_THIRDWEB_CLIENT_ID=your_client_id

# Revolut Payments
VITE_REVOLUT_SANDBOX_API_KEY=your_api_key
VITE_REVOLUT_MERCHANT_ID=your_merchant_id

# Optional
VITE_GOOGLE_MAPS_API_KEY=your_maps_key
ASSEMBLY_AI_API_KEY=your_assemblyai_key
```

## 🚀 **Deployment**

### **Frontend Deployment:**
- **Netlify**: Optimized for static site hosting
- **Vercel**: Excellent for React applications
- **GitHub Pages**: Free static hosting
- **IPFS/Filecoin**: Decentralized hosting

### **Backend Services:**
- **Supabase**: Managed PostgreSQL database
- **Express Server**: Node.js API for webhooks
- **Revolut Webhooks**: Payment notification endpoints

### **Mobile Deployment:**
- **Progressive Web App**: Installable on mobile devices
- **Capacitor/Cordova**: Native mobile app wrapper (optional)
- **WebXR**: AR features work directly in mobile browsers

## 🏆 **Innovation Highlights**

### **Revolutionary Payment Model:**
- ✅ **Eliminates Physical Devices**: No hardware costs for merchants
- ✅ **User-Controlled Payment Flow**: Users deploy their own terminals
- ✅ **Cross-Chain Interoperability**: CCIP-powered seamless transfers
- ✅ **Fiat-Crypto Bridge**: Revolut integration for traditional payments
- ✅ **AR-Enhanced UX**: Spatial payment terminals in real world

### **Blockchain Integration:**
- ✅ **Multi-Chain Support**: EVM, Solana, Hedera compatibility
- ✅ **CCIP Cross-Chain**: Chainlink-powered bridge protocol
- ✅ **Smart Contract Automation**: Trustless payment processing
- ✅ **Real-time Settlement**: Instant blockchain confirmations

### **Spatial Computing:**
- ✅ **AR Payment Terminals**: 3D virtual terminals in physical space
- ✅ **Geolocation Anchoring**: GPS-accurate terminal placement
- ✅ **WebXR Standard**: Works across all AR-capable devices
- ✅ **Progressive Enhancement**: Works with or without AR

## 🗺️ **Roadmap**

### **Phase 1: Core Platform** ✅
- [x] Multi-chain blockchain integration
- [x] Revolut payment processing
- [x] AR terminal deployment
- [x] Basic CCIP cross-chain transfers

### **Phase 2: Enhanced Features** 🚧
- [ ] Advanced AR interactions and animations
- [ ] Multi-terminal management dashboard
- [ ] Recurring payment subscriptions
- [ ] Enhanced analytics and reporting
- [ ] Mobile native app (iOS/Android)

### **Phase 3: Enterprise** 📋
- [ ] White-label solutions for businesses
- [ ] API for third-party integrations
- [ ] Advanced multi-signature support
- [ ] Compliance and regulatory features
- [ ] Enterprise SLA and support

### **Phase 4: Ecosystem** 🌐
- [ ] Marketplace for payment terminal templates
- [ ] Plugin system for custom payment flows
- [ ] Integration with major e-commerce platforms
- [ ] DeFi yield optimization for merchant funds
- [ ] DAO governance for platform development

## 🤝 **Contributing**

We welcome contributions from the community!

### **How to Contribute:**

1. **Fork the Repository**
   ```bash
   git clone https://github.com/BeerSlothAgent/cube-pay-ar.git
   ```

2. **Create Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**
   - Follow the existing code style
   - Add tests if applicable
   - Update documentation

4. **Commit Your Changes**
   ```bash
   git commit -m "feat: add your feature description"
   ```

5. **Push and Create PR**
   ```bash
   git push origin feature/your-feature-name
   ```

### **Development Guidelines:**
- Follow TypeScript best practices
- Write meaningful commit messages (Conventional Commits)
- Add JSDoc comments for public APIs
- Test on multiple browsers and devices
- Ensure mobile responsiveness

## 📞 **Support & Community**

- **Issues**: [GitHub Issues](https://github.com/BeerSlothAgent/cube-pay-ar/issues)
- **Discussions**: [GitHub Discussions](https://github.com/BeerSlothAgent/cube-pay-ar/discussions)
- **Documentation**: See `/docs` folder for detailed guides

## 📄 **License**

MIT License - See [LICENSE](LICENSE) file for details.

## 🔗 **Links & Resources**

### **Live Applications:**
- **Main Platform**: [AgentSphere Platform](https://playful-cranachan-e941e5.netlify.app/)
- **AR Demo**: [AR Viewer Demo](https://admirable-hamster-b9c370.netlify.app/)
- **Presentation**: [Project Overview](https://agentsphere-0xa1tku.gamma.site/)

### **Related Repositories:**
- **Main Repository**: [cube-pay-ar](https://github.com/BeerSlothAgent/cube-pay-ar)
- **E-Shop Integration**: [eshop-sparkle-assets](https://github.com/BeerSlothAgent/eshop-sparkle-assets)
- **On/Off Ramp**: [onofframp-cube-paygate](https://github.com/BeerSlothAgent/onofframp-cube-paygate)

### **Documentation:**
- [CCIP Integration Guide](./CCIP_IMPLEMENTATION_LEADERSHIP_SUMMARY.md)
- [Revolut Integration](./REVOLUT_INTEGRATION_COMPLETE_GUIDE.md)
- [AR Viewer Setup](./MOBILE_AR_DEPLOYMENT_GUIDE.md)
- [Payment Cube System](./PAYMENT_CUBE_SYSTEM_DOCUMENTATION.md)
- [API Documentation](./API_DOCUMENTATION_POLYGON_AMOY_SOLANA_DEVNET.md)

### **Technology Partners:**
- **Chainlink CCIP**: Cross-chain interoperability
- **Revolut Business**: Fiat payment processing
- **Supabase**: Backend infrastructure
- **ThirdWeb**: Web3 development platform
- **Netlify**: Deployment and hosting

---

## 🌟 **About CubePay AR**

CubePay AR is part of the **AgentSphere** ecosystem, a comprehensive platform for spatial augmented reality and blockchain-powered applications. Our mission is to revolutionize payments by eliminating physical barriers and empowering merchants with virtual, device-free payment infrastructure.

### **Why CubePay AR?**

Traditional payment systems require:
- ❌ Expensive physical terminals
- ❌ Complex setup and maintenance
- ❌ Card data storage and tokenization
- ❌ High processing fees
- ❌ Limited payment options

**CubePay AR provides:**
- ✅ Virtual terminals deployed instantly
- ✅ Zero hardware costs
- ✅ User-controlled payment sovereignty
- ✅ Transparent, competitive fees
- ✅ Crypto + fiat + cross-chain support

---

**Built with ❤️ for the Future of Payments**

**Powered by:** Blockchain • Chainlink CCIP • Revolut • Spatial Computing

**Part of:** AgentSphere Spatial Augmented FinApp Ecosystem �
