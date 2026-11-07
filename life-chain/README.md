# Chain overview

The LIFE AI chain is an [Avalanche L1](https://build.avax.network/docs/avalanche-l1s) deployed and managed through [AvaCloud](https://avacloud.io). It runs Avalanche's standard open-source software:

- **AvalancheGo** as the node and consensus client
- **Subnet-EVM** as the virtual machine, so the chain is fully EVM-compatible (Solidity contracts, MetaMask, Foundry, Hardhat)

Key properties:

| Property | Value |
|---|---|
| Consensus | Avalanche Snowman++ |
| Validator model | Proof-of-Authority (PoA) Validator Manager |
| Execution | EVM (Subnet-EVM) |
| Native gas token | `ALIFE` (testnet), 18 decimals |
| Target block rate | 2 seconds |
| Block gas limit | 12,000,000 |

Pages in this section:

- [Network information](network-information.md)
- [Consensus & validators](consensus-and-validators.md)
- [Node software](node-software.md)
- [Cryptography & audits](cryptography-and-audits.md)
- [Build on the LIFE AI chain](build-on-life-chain.md)
