# Hey, I'm Anton 👋

Smart Contract Engineer with 5+ years in software engineering, specialising in production DeFi for the last 3 years. Before going deep on Solidity, I built automated testing infrastructure and data pipelines at scale (Barclays, PyTest, 
PySpark). Now I focus on protocol architecture, cross-chain messaging, and security - and I'm exploring where AI agents intersect with the DeFi ecosystem.

Currently finishing a Uniswap V4 hook focused on impermanent loss minimisation.

---

## What I build

- **DeFi protocols and integrations** - vaults (ERC-4626, Morpho Vaults V1/V2), lending markets (Aave V3, Morpho Market), and DEX integrations (Uniswap V2 / V3 / V4 + hooks).

- **Cross-chain infrastructure** - production deployments using LayerZero OFT / OApp standards and Chainlink CCIP for multi-chain asset and message routing.

- **Protocol security** - fuzz testing with Echidna, static analysis with Slither, internal audits, and detailed test suites using Foundry.

- **Bots for HFT** - arbitrage bots for HFT between DEX - DEX and CEX - DEX.

---

## Technical depth

```
Languages       Solidity (primary) · Yul · Python · TypeScript
EVM             Memory / Storage / Calldata layout · Gas optimization · Inline assembly
Standards       ERC-20 / 721 / 1155 / 1153 / 2612 / 4626
Proxy patterns  Transparent Proxy · UUPS
Cross-chain     LayerZero OFT / OApp · Chainlink CCIP
Security        DeFi vulnerabilities prevention · Secure Solidity coding patterns · Auditing · Fuzzing
Tooling         Foundry (preferred) · Hardhat · Echidna · Slither · Tenderly
Backend         FastAPI · PostgreSQL · Docker · Redis 
```

---

## Deployed on mainnet

| Project | Chain | Description |
|---|---|---|
| [$HAI OFT](https://basescan.org/address/0x7002987e5F63716273E77b51E12A578143C222aa#code) Migration | Ethereum · BSC · Base | Redesigned and migrated ~$6M market cap token to LayerZero OFT standard via UUPS upgradeable proxy. Preserved user balances using Merkle proof-based distribution. |
| [Hacken Launchpool](https://basescan.org/address/0x03a6859d85e4f4b8c380ef7cc73f86ee7a9f3b76#code) | Base | Staking and reward distribution protocol integrated with the Hacken ecosystem. Built from scratch to mainnet. |
| Vault-based Prediction Market | Ethereum | Prediction market protocol for Hacken Proof bug bounty platform. Chainlink price feeds + Uniswap for fair payout calculation. |
---

## Selected projects

### [eigen-auction](https://github.com/ohMySol/eigen-auction)
EigenAuction is a system built on top of Uniswap v4 hooks and EigenLayer AVS that introduces an app-specific sequencing mechanism to reduce Loss-Versus-Rebalancing (LVR) for liquidity providers (LPs).

Instead of allowing arbitrageurs to capture value through traditional blockspace competition and tips to block builders/proposers, EigenAuction redirects this flow into an off-chain arbitrage auction secured by EigenLayer. Arbitrageurs bid for the right to execute arbitrage, with proceeds partially redistributed to LPs.

The auction winner receives top-of-block execution rights for the arbitrage opportunity.

### [erc4626-strategy-vault](https://github.com/ohMySol/erc4626-strategy-vault)
ERC-4626 vault with a permissionless strategy marketplace. Morpho-style timelocks for risk-sensitive actions, role-based access (owner / curator / guardian / allocator), gasless deposits via ERC-2612 permit, and a performance fee model that splits yield between the protocol and strategy creators. Fuzz tested with Echidna.

### [uni-v4-limit-order-hook](https://github.com/ohMySol/uni-v4-limit-order-hook)
Uniswap V4 hook implementing on-chain limit orders. Uses `beforeSwap` and `afterSwap` callbacks to match pending orders against pool price movements. *(Impermanent loss minimisation hook in progress.)*

### [panorama](https://github.com/ohMySol/panorama)
A smart contract dependency analyzer that visualizes the entire dependency graph in a way that you can clearly see what your vault or pool or strategy depends on. It takes the Solidity contract address for the input and via the BFS (breadth-first search) algorithm builds a dependency graph where each node - is a separate external contract your requested address relies on.
Useful in improving risk management, auditing and large codebases research.

---

## Beyond code

- Running a [Telegram channel](https://t.me/call_data) on DeFi and smart contract development - protocol breakdowns, my DeFi projects and experience, and yield strategy analysis. 100+ subscribers.

- Actively managing my own DeFi yield positions across Morpho and Uniswap. Continiously searching for new opportunities / strategies in yield generation with security first mindset.

---

## Connect

[Telegram](https://t.me/ohmysol) · [LinkedIn](https://www.linkedin.com/in/anton-holovchenko-3221321a5/) · [X](https://x.com/ohMySolboy/)

*Currently open to new roles - smart contract engineering, DeFi protocol development, yield strategies development.*
