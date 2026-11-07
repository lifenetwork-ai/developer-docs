# Overview

The LIFE AI network has two on-chain components:

| Component | What it is | Where it runs |
|---|---|---|
| **LIFE AI chain** | An Avalanche L1 (EVM, Subnet-EVM) operated with a Proof-of-Authority validator manager and hosted on AvaCloud | Avalanche Fuji testnet (chainId `99991`) |
| **LIFE token** | A fixed-supply ERC20 token (`LIFE`, 10,000,000,000 supply) plus vesting and distribution contracts | Avalanche C-Chain (testnet: Fuji, chainId `43113`) |

The two components are independent: the LIFE ERC20 token lives on Avalanche C-Chain and does not depend on the LIFE AI chain. The LIFE AI chain uses its own native gas token, `ALIFE` (testnet).

## Where to go next

- Connect to the chain: [Network information](../life-chain/network-information.md)
- Understand how the chain is secured: [Consensus & validators](../life-chain/consensus-and-validators.md)
- Review the token source: [Contracts & source code](../life-token/contracts-and-source-code.md)
- See who controls administrative keys: [Admin keys & multisig](../governance-and-security/admin-keys-and-multisig.md)
