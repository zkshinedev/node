# zkShine Node Infrastructure

![Solana](https://img.shields.io/badge/Built_for-Solana-14F195?logo=solana&logoColor=white)
![DePIN](https://img.shields.io/badge/DePIN-Network-blueviolet)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Version-0.2.0--alpha-yellow)

> **zkShine Node** powers the decentralized privacy infrastructure — combining ZK compute, anonymous relaying, and VPN gateway services to deliver full-stack privacy for the Solana ecosystem.

---

## 🧩 Components

| Component | Description |
|------------|--------------|
| ⚙️ **ZK Compute Node** | Executes zkSNARK/zkSTARK proofs for confidential computations. |
| 🛰️ **Privacy Relayer** | Submits user transactions without exposing wallet or IP metadata. |
| 🌐 **Web3 VPN Gateway** | Provides encrypted RPC routing and decentralized proxy services. |
| 🧱 **Confidential Vault Daemon** | Manages encrypted storage for zkVault access and identity proofs. |

---

## ⚙️  Architecture Overview

```console
User → Wallet → Privacy Relayer → zkCompute Node → Solana Network → Vault Storage
- Generate and verify zero-knowledge proofs.
- Relay Solana transactions privately on behalf of users.
- Encrypt and route traffic through zkShine VPN Gateways.
- Host small encrypted data blobs for zkVault (identity proofs, documents).
Node.js >= 18
Docker & Docker Compose
Solana CLI
Yarn or npm
git clone https://github.com/zkshinedev/node.git
cd node
yarn install
