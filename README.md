# Token2022 to SPL Wrapper

## Overview
This program allows wrapping of **Token2022** Solana tokens into **SPL tokens**. Each token created using **Token2022** can be wrapped into its unique SPL token, which can then be used across various applications on the **Solana blockchain**.

This is an **early release** and currently supports only the **transfer fee extension**.

## Features
- Wrap **Token2022** tokens into **SPL tokens**.
- Support for **transfer fee extension**.
- Enables cross-application usage of wrapped tokens.

## Installation
Ensure you have the following installed:
- [Rust](https://www.rust-lang.org/)
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli)

### Clone the Repository
```sh
git clone https://github.com/your-repo/token2022-spl-wrapper.git
cd token2022-spl-wrapper
```

### Build the Program
```sh
cargo build --release
```

## Usage

### Deploy the Program
Ensure your Solana CLI is configured with the correct network:
```sh
solana config set --url https://api.mainnet-beta.solana.com
```

Deploy the program using:
```sh
solana program deploy target/release/token2022_spl_wrapper.so
```

### Wrapping a Token2022 Token
To wrap a **Token2022** token into an SPL token, call the program with the appropriate parameters:
```sh
solana program invoke \
  --account <token2022-mint-address> \
  --account <destination-spl-mint-address> \
  --signer <your-wallet-keypair.json>
```

## Roadmap
- Support for additional **Token2022 extensions**.
- Improved user experience with **CLI commands**.
- Integration with **Solana wallets** for seamless wrapping.

## Contributing
We welcome contributions! Please open an issue or submit a pull request if you find a bug or have an improvement idea.

## License
This project is licensed under the **MIT License**.

## Contact
For questions and discussions, join our **Solana developer community** or open an issue on this repository.

Telegram: [Dogewhiz](https://t.me/dogewhiz)

