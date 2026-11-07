# Node software

The LIFE AI chain runs entirely on Avalanche's standard open-source node software. No custom or proprietary node software is used.

| Component | Role | License | Source |
|---|---|---|---|
| AvalancheGo | Node and consensus client | BSD-3-Clause | https://github.com/ava-labs/avalanchego |
| Subnet-EVM | EVM virtual machine (now maintained inside the AvalancheGo repository) | LGPL-3.0 | https://github.com/ava-labs/avalanchego/tree/master/graft/subnet-evm |

## Updates

Validator nodes are AvaCloud-managed. AvaCloud provides automated node software updates for managed validators; updates are not enforced at the consensus protocol level. Network upgrades follow the AvalancheGo release process: https://github.com/ava-labs/avalanchego/releases
