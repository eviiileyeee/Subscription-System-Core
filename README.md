# ☕ **Subscription-System-Core** Smart Contract

This repository provides a smart contract framework that enables users to support creators by "buying a coffee"—a metaphorical transaction where users send Ethereum (ETH) along with a personal message. The project leverages Solidity and Hardhat for smart contract development and testing, ensuring compatibility with Core Blockchain networks.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/eviiileyeee/Subscription-System-Core.git
cd ProjectName
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the project root:

```env
PRIVATEKEY="your_core_wallet_private_key"
CORE_TEST2_SCAN_KEY="your_testnet2_explorer_api_key"
```

> ⚠️ **Important:** Never share your private key or commit the `.env` file to version control.

---

## 🛠 Hardhat Commands

### Compile Contracts

```bash
npx hardhat compile
```

### Run Tests

```bash
npx hardhat test
```

### Deploy Contract

Use a deployment script:

```bash
npx hardhat run scripts/deploy.js --network core_testnet2
```

---

## 🔍 Contract Verification

You can verify contracts using Core block explorers:

```bash
npx hardhat verify --network core_testnet2 <deployed_contract_address> <constructor_args_if_any>
```

API keys for verification must be included in `.env` as shown above.

---
