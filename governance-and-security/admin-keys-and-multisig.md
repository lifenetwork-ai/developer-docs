# Admin keys & multisig

The LIFE ERC20 token contract has no owner or admin role (no mint, pause, blacklist or upgrade), so no multisig can control the token itself. Multisigs only control the distribution contracts and the LIFE AI chain administration.

## Planned production setup

| Role | Signature parameters | Signers |
|---|---|---|
| Governance/Treasury Safe | 3-of-5 | Five designated representatives, each representing one of the five highest-impact LIFE AI network subnets (application-level service groups within the LIFE AI network, not Avalanche subnets/L1s); each holds one independent signer key |
| Emergency Safe | 3-of-5 | LIFE AI core team |
| LIFE AI chain administration (Validator Manager owner, FeeManager/RewardManager precompile admin) | To be transferred to the Governance Safe | — |

The identities and wallet addresses of all production signers will be disclosed once finalized and before mainnet/TGE.

## Current testnet setup (Avalanche Fuji)

| Role | Address | Signature parameters |
|---|---|---|
| Governance/Treasury Safe | `0x015eaebf18986D4F65655B07b15e863F65b5913b` | 2-of-3, test keys held by the LIFE AI engineering team |
| Emergency Safe | `0x60E0f8D92CF27898D5D1F1Cb64dA906ea05A70EE` | 2-of-3, test keys held by the LIFE AI engineering team |
| LIFE AI chain administration (Validator Manager owner, FeeManager/RewardManager precompile admin) | `0xeedC556a6935c4B9532754e6fc97cD20DDd59544` | Single LIFE AI-controlled key |

The NativeMinter and allow-list precompiles are not enabled on the LIFE AI chain.
