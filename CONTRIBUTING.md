# Contributing to UNIX

Thanks for your interest in contributing to UNIX! This document will guide you through the contribution process.

## Getting Started

1. Fork the repository
2. Clone your fork: `git clone https://github.com/YOUR_USERNAME/unix.git`
3. Install dependencies: `pnpm install`
4. Create a new branch: `git checkout -b feature/your-feature-name`

## Development Workflow

### Project Structure
```
unix/
├── typescript/          # TypeScript implementation
│   ├── packages/       # Core packages
│   ├── examples/       # Example projects
│   └── scripts/        # Development scripts
├── python/             # Python implementation
│   ├── src/           # Source code
│   └── examples/      # Example projects
└── docs/              # Documentation
```

### Building the Project
```bash
# Build all packages
pnpm build

# Build specific package
cd typescript/packages/core
pnpm build
```

### Running Tests
```bash
# Run all tests
pnpm test

# Run specific package tests
cd typescript/packages/core
pnpm test
```

## Creating a Plugin

1. Use the plugin creation script:
```bash
cd typescript
pnpm create-plugin -n your-plugin-name -t evm
```

2. Implement your plugin functionality in `src/your-plugin-name.service.ts`

3. Add tests in `src/__tests__/`

## Pull Request Process

1. Update documentation for any new features
2. Add tests for new functionality
3. Ensure all tests pass: `pnpm test`
4. Update the changelog
5. Submit your PR with a clear description

## Code Style

- Use TypeScript for type safety
- Follow existing code formatting (enforced by Biome)
- Write clear commit messages
- Document public APIs
- Add tests for new features

## Need Help?

- Check the [documentation](https://unix.dev)
- Join our [Discord](https://discord.gg/Insyd-sol)
- Open an issue

## License
By contributing, you agree that your contributions will be licensed under the MIT License.
