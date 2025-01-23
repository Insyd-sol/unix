# UNIX TypeScript SDK 🖥️

The TypeScript implementation of my UNIX framework for blockchain-enabled AI agents.

## Features
- Full TypeScript/JavaScript support
- Type-safe API
- Built-in wallet adapters
- Extensive plugin system
- Framework agnostic

## Quick Setup

```bash
# Install the core package
npm install @Insyd-sol/core

# Install wallet adapter (e.g., for EVM chains)
npm install @Insyd-sol/wallet-viem

# Optional: Install plugins you need
npm install @Insyd-sol/plugin-erc20
```

## Development

1. Clone the repo
2. Install dependencies: `pnpm install`
3. Build packages: `pnpm build`

## Package Structure
- `core/`: Core framework functionality
- `wallets/`: Wallet adapters for different chains
- `plugins/`: Protocol-specific plugins
- `adapters/`: AI framework adapters
- `examples/`: Example implementations

## Testing
Run `pnpm test` to execute the test suite.

## Documentation
Visit [unix.dev](https://unix.dev) for full documentation.
