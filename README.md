# 🚀 Solana Hello World Smart Contract

This project demonstrates how to deploy a simple **Rust-based smart contract** (Hello World) on the **Solana Devnet**, using the **Solana CLI** and Rust toolchain.

📚 _Note: This Hello World guide has moved to the [official Solana documentation](https://docs.solana.com/)._

---

## ✅ Highlights

- 🔧 Built in Rust and compiled to BPF bytecode  
- 🌐 Deployed to **Devnet** using `solana program deploy`  
- 🖼️ Includes screenshots for each step  
- 🧪 Verified to work with **Solana CLI v1.17+**

---

## 🛠️ Setup & Deployment Steps

### 1. Install Solana CLI

```bash
solana --version
```

### 2. Configure Devnet & Generate Wallet

```bash
solana config set --url https://api.devnet.solana.com
solana-keygen new
solana airdrop 2
```

### 3. Clone Hello World Example

```bash
git clone https://github.com/solana-labs/example-helloworld.git
cd example-helloworld
```

### 4. Install Rust & BPF Toolchain

```bash
rustup install stable
rustup component add rust-src
```

### 5. Install Node.js dependencies

```bash
npm install
```

### 6. Build the Smart Contract

```bash
npm run build:program-rust
```

Or (if `cargo build-bpf` is deprecated):

```bash
docker run --rm -v "%cd%":/project -w /project solanalabs/solana:v1.17.15 \
  cargo build-sbf --manifest-path=src/program-rust/Cargo.toml --sbf-out-dir=dist/program
```

### 7. Deploy to Devnet

```bash
solana program deploy dist/program/helloworld.so
```

---

## 💡 Deployment Info

- **Wallet Address:**  
  `38QZx3nJPp8bERyVge8ya3wmbtHzsvgD6tjffoT3DuQX`

- **Program ID:**  
  `BMG1DEhdfd5148A5tiN3ZVuaBTTmro7U6UiN1rmsFBuG`

- **Explorer (Devnet):**  
  [View on Solana Explorer](https://explorer.solana.com/address/BMG1DEhdfd5148A5tiN3ZVuaBTTmro7U6UiN1rmsFBuG?cluster=devnet)

---

## 🖼️ Screenshots

📷 [Click to view screenshots in Google Docs](https://docs.google.com/document/d/1qB4l2D_W6euuG6qus7e7PFXIiZT-BG2pnrpQlI3lN5g/edit?tab=t.0)

---

## 📄 License

This project uses the [MIT License](https://github.com/solana-labs/example-helloworld/blob/master/LICENSE), inherited from Solana Labs.

---

💬 _Created as part of a Blockchain Technologies 2 course assignment._
