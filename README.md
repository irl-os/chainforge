# ChainForge 🔗🔥

**ChainForge** is an open-source command-line tool to generate blockchain addresses with customizable prefixes or suffixes. Perfect for those who want personalized wallet addresses for different blockchains! Currently, **Solana** is supported, with placeholders for **Bitcoin SV (BSV)**, **Fractal Bitcoin (fBTC)**, and **Bitcoin Cash (BCH)**.

## Features

- 🎉 Generate blockchain wallet addresses with custom prefixes or suffixes
- 🌐 Currently supports Solana; extensible for more chains!
- 🚀 Built with TypeScript and runs on Bun for high performance

## Getting Started

### Prerequisites

- **[Bun](https://bun.sh/)** installed on your system

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/ChainForge.git
   cd ChainForge
   ```

2. Install the required dependencies:

   ```bash
   bun install
   ```

### Usage

Run ChainForge with the following syntax:

```bash
bun run address_generator.ts <blockchain> <prefix|suffix> <phrase>
```

- **`blockchain`**: Choose from `sol`, `bsv`, `fbtc`, or `bch`
- **`prefix|suffix`**: Specify whether the phrase should appear as a prefix or suffix
- **`phrase`**: Define the text pattern you want (e.g., `abcd`, `w4v3`)

#### Example

Generate a Solana address that ends with "w4v3":

```bash
bun run address_generator.ts sol suffix w4v3
```

**Note**: Since this uses brute-force key generation, it may take some time to find an address matching your criteria.

## Supported Blockchains

| Blockchain      | Status      | Notes                                      |
|-----------------|-------------|--------------------------------------------|
| Solana (`sol`)  | ✅ Supported | Uses `@solana/web3.js` for key generation |
| Bitcoin SV (`bsv`) | 🚧 Coming Soon | Placeholder logic for now               |
| Fractal Bitcoin (`fbtc`) | 🚧 Coming Soon | Placeholder logic for now         |
| Bitcoin Cash (`bch`) | 🚧 Coming Soon | Placeholder logic for now            |

## Contributing

We welcome contributions to add support for additional blockchains, improve the generation speed, or optimize existing logic!

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a Pull Request.

## Roadmap

- [ ] Add support for Bitcoin SV (BSV) address generation
- [ ] Add support for Fractal Bitcoin (fBTC) address generation
- [ ] Add support for Bitcoin Cash (BCH) address generation
- [ ] Performance improvements for address matching
- [ ] Integrate a UI for more interactive use

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Inspired by the fun of personalizing blockchain addresses and contributing to open-source blockchain tools!

---

Happy forging with **ChainForge**! 🛠🔗
