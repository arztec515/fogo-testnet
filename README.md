# Fogo Terminal
[![IMG-20250801-181639.jpg](https://i.postimg.cc/Sx06Vg0G/IMG-20250801-181639.jpg)](https://postimg.cc/vczxZLZ1)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-node.js-lightgrey.svg)

**Fogo Terminal** is a powerful command-line interface (CLI) built to **simplify and accelerate transactions** on the Fogo Testnet. It provides a fast and user-friendly way to execute common DeFi operations, such as swaps and asset management, directly from your terminal.

---

## Key Features

* **Asset Management**: View your native FOGO token balance in real-time.
* **Cross-Token Swaps**: Execute swaps between FOGO, fUSD, USDT, and USDC.
* **Batch Execution**: Run multiple transactions sequentially with a single command.
* **Add Liquidity** (Coming Soon)
* **Transfer** (Coming Soon)

---

## Prerequisites

Before getting started, ensure you have the following software installed:
* [Node.js](https://nodejs.org/) (v18.x or newer)
* [Solana Tool Suite (CLI)](https://docs.solana.com/cli/install-solana-cli-tools)

---

## Installation & Setup

Follow these steps to get the Fogo Terminal up and running.

**1. Clone the Repository**

```bash
git clone https://github.com/arztec515/fogo-testnet.git
cd fogo-testnet
```

**2. Install Dependencies**

Run the following command to install all the necessary packages.
```bash
npm install
```

**3. Change Environment File (.env)**

Rename file `.env.example` to `.env`in the project's root directory. This file will store your wallet's private key.
```
cp env.example .env
```

After change name to .env file and add your PRIVATE_KEY.

```
nano .env
```
The program supports two formats:
 * Option 1: Base58 String (Recommended)
```
PRIVATE_KEY=57fzAscJ4bgo1QtGUhEgt6rXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
```
 * Option 2: Byte Array
```
PRIVATE_KEY=[11,22,33,44,55,66,77,88,99,101,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127,128,129,130,131,132,133,134,135,136,137,138,139,140,141,142,143,144,145,146,147,148,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165]
```

## Usage
To run the terminal, use the following command from the root directory:
```
node index.js
```

The Fogo Terminal header will appear, and you can begin using the available commands.

---

## ⚠️ Security Warning
 * This tool is designed for use in a Testnet environment.
 * It is strongly not recommended to use a private key from your mainnet wallet that holds real assets.
 * Always use a dedicated burner wallet funded by a testnet faucet for all development and testing activities. The developers are not responsible for any loss of assets due to misuse of this tool.
