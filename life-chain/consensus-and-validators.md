# Consensus & validators

## Consensus

The LIFE AI chain uses Avalanche's **Snowman++** consensus protocol. Snowman is a linear-chain consensus based on repeated random subsampling of validators, providing fast, probabilistic finality. Snowman++ adds a soft proposer window to reduce block contention.

The chain runs on AvalancheGo with validator infrastructure managed through AvaCloud.

## Validator model

Validators are managed by a **Proof-of-Authority (PoA) Validator Manager** contract from Ava Labs' [ICM contracts](https://github.com/ava-labs/icm-contracts). Only the Validator Manager owner can add or remove validators; there is no permissionless staking.

To join the validator set, an operator runs a compatible AvalancheGo validator node and is registered as an L1 validator on the Avalanche P-Chain through the Validator Manager, subject to the LIFE AI chain's validator admission policy.

## Current validator set (testnet)

| Node ID | Weight | Share | Operator |
|---|---|---|---|
| `NodeID-NBwvdq5tbw4KKdhXZ3RjWm5QjhnVsx4iu` | 100 | 50% | LIFE AI (AvaCloud-managed node) |
| `NodeID-MifYgtWuQCGFiEd37iwxwcz8UTWLyAa48` | 100 | 50% | LIFE AI (AvaCloud-managed node) |

- Validator Manager contract (on Avalanche Fuji C-Chain): `0x9d353f6048877f06b83cb9a839b7c65b32adbb6b`
- As a testnet, all validators are operated by a single entity. No decentralization guarantee is claimed for this phase.

The live validator set can be checked on the Avalanche P-Chain with `platform.getCurrentValidators` for subnet ID `25YEBH59JH1B1BXaQp7KRE6B5gx7NcvywDUvCne9Q3yizZHbtR`.

## Phases

| Phase | Status |
|---|---|
| Testnet | Live on Avalanche Fuji (see above) |
| Private mainnet | No private mainnet phase is planned |
| Public mainnet | No plan or timeline yet. The validator breakdown and decentralization attestation will be published before any launch |
