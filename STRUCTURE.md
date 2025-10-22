# Monorepo Structure

```
cube-pay-ar/
│
├── apps/                           # Applications
│   ├── ar-viewer/                  # Main AR Viewer & AgentSphere App
│   │   ├── components/             # React components
│   │   │   ├── marketplace/        # AgentSphere marketplace
│   │   │   ├── ui/                 # Radix UI components
│   │   │   ├── ARViewer.jsx        # AR viewer
│   │   │   ├── PaymentQRModal.jsx  # Payment modals
│   │   │   └── ...
│   │   ├── services/               # Business logic
│   │   │   ├── qrCodeService.js
│   │   │   ├── evmPaymentService.js
│   │   │   ├── solanaPaymentService.js
│   │   │   └── ...
│   │   ├── config/                 # Chain configs
│   │   ├── hooks/                  # React hooks
│   │   ├── providers/              # Context providers
│   │   ├── utils/                  # Utilities
│   │   └── package.json
│   │
│   ├── eshop/                      # E-commerce Shop (submodule)
│   │   └── [E-shop codebase]
│   │
│   └── on-off-ramp/                # Payment Gateway (submodule)
│       └── [On/Off ramp codebase]
│
├── packages/                       # Shared packages
│   ├── shared/                     # Shared utilities & types
│   │   └── [To be populated]
│   │
│   └── payment-engine/             # Core payment engine
│       └── [To be extracted from ar-viewer]
│
├── docs/                           # Documentation
│   ├── API_Documentation.md
│   ├── Schemas.md
│   └── ...
│
├── sql/                            # Database schemas
│   └── ...
│
├── package.json                    # Root workspace config
├── README.md                       # Main documentation
└── .gitmodules                     # Submodule configuration
```

## Key Components

### AR Viewer App (`apps/ar-viewer`)
- **AR/3D Rendering**: Three.js based 3D agent visualization
- **AgentSphere Marketplace**: Browse and interact with AI agents
- **Payment Integration**: Multi-chain wallet support
- **QR Code System**: Generate and scan payment QR codes

### Shared Packages (`packages/`)
- **shared**: Common utilities, types, constants
- **payment-engine**: Core payment processing logic (to be extracted)

### External Apps (Submodules)
- **eshop**: E-commerce frontend
- **on-off-ramp**: Fiat gateway

## Development Workflow

1. Work on any app independently in `apps/`
2. Extract shared code to `packages/`
3. Import shared packages across apps
4. Commit everything together in one branch
