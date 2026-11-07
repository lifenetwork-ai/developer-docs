# Build on the LIFE AI chain

The LIFE AI chain is EVM-compatible, so standard Ethereum tooling works unchanged. Point your tool at the RPC URL and chain ID from [Network information](network-information.md). You need testnet `ALIFE` for gas.

## Foundry

```sh
# Check connectivity
cast chain-id --rpc-url https://subnets.avax.network/lifev1/testnet/rpc

# Deploy a contract
forge create src/Counter.sol:Counter \
  --rpc-url https://subnets.avax.network/lifev1/testnet/rpc \
  --account <your-keystore-account> \
  --broadcast
```

## Hardhat

```js
// hardhat.config.js
module.exports = {
  solidity: "0.8.30",
  networks: {
    lifeTestnet: {
      url: "https://subnets.avax.network/lifev1/testnet/rpc",
      chainId: 99991,
      accounts: [process.env.PRIVATE_KEY],
    },
  },
};
```

## Fee parameters (testnet)

| Parameter | Value |
|---|---|
| Block gas limit | 12,000,000 |
| Target block rate | 2 s |
| Minimum base fee | 25 gwei |
| Target gas | 25,000,000 |
