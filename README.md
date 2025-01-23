<div align="center">

# UNIX 🖥️
A powerful AI agent framework for blockchain interactions

[Documentation](https://unixsol.xyz/) | [Examples](https://github.com/Insyd-sol/unix/tree/main/typescript/examples)

</div>

## What is UNIX?
UNIX (Universal Network Interface eXtension) is a framework I created to bridge the gap between AI agents and blockchain technology. It provides a unified interface for AI agents to interact with various blockchain networks, making it easy to perform operations like sending tokens, interacting with smart contracts, and managing wallets.

### The Problem I Solved
Building AI agents that can interact with blockchains is complex. You have to deal with:
- Multiple blockchain networks (Ethereum, Solana, etc.)
- Different wallet providers
- Various smart contract protocols
- Multiple AI agent frameworks

Each combination requires its own implementation, making it time-consuming and error-prone to build blockchain-capable AI agents.

### The Solution
UNIX provides a single, unified interface that works with:
- **Any AI Framework**: Works seamlessly with Langchain, Vercel AI SDK, Eliza, and more
- **Any Blockchain**: Supports Ethereum, Solana, and other EVM chains
- **Any Wallet**: Use your own keys, Crossmint Smart Wallets, or any other provider
- **Any Protocol**: Easy integration with DeFi protocols, NFT marketplaces, and more

## Quick Start

```typescript
// Connect your wallet
const wallet = ...  // Your wallet connection

// Get the tools you need
const tools = getOnChainTools({
  wallet: viem(wallet),
  plugins: [
    sendETH(),
    erc20({ tokens: [USDC] }),
    // Add more plugins as needed
  ],
})

// Use with your AI agent
const result = await generateText({
    model: openai("gpt-4"),
    tools: tools,
    prompt: "Send 1 USDC to 0x..."
});
```

## Features
- 🔌 **Plug & Play**: Works with all major AI frameworks
- 🔒 **Secure**: Built with security best practices
- 🌐 **Multi-Chain**: Support for major blockchain networks
- 🛠️ **Extensible**: Easy to add new protocols and features
- 📚 **Well Documented**: Comprehensive guides and examples

## Installation

```bash
# Using npm
npm install @Insyd-sol/core

# Using pnpm
pnpm add @Insyd-sol/core

# Using yarn
yarn add @Insyd-sol/core
```

## Examples
Check out the [examples directory](https://github.com/Insyd-sol/unix/tree/main/typescript/examples) for complete working examples, including:
- Basic token transfers
- DeFi interactions
- NFT operations
- Custom protocol integrations

## Contributing
Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) to get started.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support
- 📚 [Documentation](https://unix.dev)
- 💬 [Telegram Community](https://t.me/unixonsol)
- 🐦 [Twitter](https://x.com/unix_solana)
