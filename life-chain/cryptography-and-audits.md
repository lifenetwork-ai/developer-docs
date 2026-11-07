# Cryptography & audits

At the protocol level the LIFE AI chain uses standard Avalanche cryptographic implementations. It does not use custom cryptographic algorithms or zero-knowledge protocols.

| Purpose | Primitive |
|---|---|
| Node-to-node communication and node identity | TLS (staking certificates) |
| Transaction signatures | secp256k1 ECDSA |
| Avalanche Warp Messaging / ICM and L1 validator registration | BLS12-381 signatures |
| Hashing | Keccak-256 (EVM), SHA-256 |

## References

- Avalanche cryptographic primitives: https://build.avax.network/docs/rpcs/other/standards/cryptographic-primitives
- AvalancheGo source code: https://github.com/ava-labs/avalanchego
- Avalanche security audits: https://github.com/ava-labs/audits
- Subnet-EVM third-party audit (Least Authority): https://leastauthority.com/blog/least-authority-announces-the-publication-of-the-ava-labs-subnet-evm-audit/
- ICM contracts (Validator Manager) audits: https://github.com/ava-labs/icm-contracts/tree/main/audits

## LIFE-specific contracts

- The LIFE ERC20 token is a standard OpenZeppelin Contracts v5.4.0 ERC20 with no custom cryptography.
- The LIFE vesting and distribution contracts are developed in-house and contain no custom cryptography. They have been reviewed internally and have not yet received a third-party audit.
