<p align="center">
  <a href="https://solana.com">
    <img alt="Solana" src="https://i.imgur.com/uBVzyX3.png" width="250" />
  </a>
</p>

# Hello world on Solana

This hello world guide has moved to the [main Solana documentation](https://docs.solana.com/getstarted/rust).

This project showcases the deployment of a simple Rust-based smart contract (Hello World) on the **Solana Devnet**, using the Solana CLI and Rust toolchain.

## ✅ Highlights
- Built in **Rust** and compiled to BPF bytecode
- Deployed to **Devnet** using `solana program deploy`
- Includes relevant screenshots for each step
- Verified to work with **Solana CLI v1.17+**

## 🛠️ Setup & Deployment Steps

### 1. Install Solana CLI
```bash
solana --version

2.Configure Devnet & Generate Wallet
solana config set --url https://api.devnet.solana.com
solana-keygen new
solana airdrop 2

3. Clone Hello World Example
git clone https://github.com/solana-labs/example-helloworld.git
cd example-helloworld

4. Install Rust & BPF Toolchain
rustup install stable
rustup component add rust-src

5. Install Node dependencies
npm install

6. Build the Smart Contract
npm run build:program-rust

7. Deploy to Devnet
solana program deploy dist/program/helloworld.so
---


💡 Deployment Info
Wallet Address:
38QZx3nJPp8bERyVge8ya3wmbtHzsvgD6tjffoT3DuQX

Program ID:
BMG1DEhdfd5148A5tiN3ZVuaBTTmro7U6UiN1rmsFBuG

Explorer Link:
View on Solana Explorer (Devnet)


Screenshots : https://docs.google.com/document/d/1qB4l2D_W6euuG6qus7e7PFXIiZT-BG2pnrpQlI3lN5g/edit?tab=t.0




📄 License
This project uses the MIT license, inherited from Solana Labs:https://github.com/solana-labs/example-helloworld/blob/master/LICENSE


