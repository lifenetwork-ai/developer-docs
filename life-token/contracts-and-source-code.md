# Contracts & source code

## Source repository

- Repository: https://github.com/lifenetwork-ai/life-token-contracts (release `v1.0.0`)
- Commit: `00d4be00bd0b6b1bbfaa0a30d82f0668d5adf542`
- Token source: https://github.com/lifenetwork-ai/life-token-contracts/blob/00d4be00bd0b6b1bbfaa0a30d82f0668d5adf542/src/LIFEToken.sol
- Flattened source (zip): https://github.com/lifenetwork-ai/life-token-contracts/releases/download/v1.0.0/LIFEToken-source.zip
- Compiler: solc `0.8.30`, optimizer enabled with 200 runs, EVM version `cancun`

## Contracts

| Contract | Purpose |
|---|---|
| `LIFEToken.sol` | Fixed-supply ERC20 token, no admin functions |
| `LIFEVestingVault.sol` | UUPS-upgradeable shared vesting vault for Investor, Advisor, Foundation and Ecosystem grants |
| `LIFEUpgradeTimelock.sol` | Timelock (minimum 48-hour delay) controlling vesting vault upgrades |
| `TGERegistry.sol` | Records the common TGE timestamp |
| `TGEDistributionVault.sol` | Fixed TGE distribution allocations |
| `LIFEEmissionVault.sol` | Scheduled emission release |

## Build and verify

```sh
git clone --recurse-submodules https://github.com/lifenetwork-ai/life-token-contracts
cd life-token-contracts
forge build
forge test
```
