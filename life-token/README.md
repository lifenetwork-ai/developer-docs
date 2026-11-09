# Token overview

`LIFE` is the LIFE AI network token, issued as an ERC20 on **Avalanche C-Chain**.

| Property | Value |
|---|---|
| Name / symbol | LIFE AI / `LIFE` |
| Standard | ERC20 (OpenZeppelin Contracts v5.4.0) |
| Decimals | 18 |
| Total supply | 10,000,000,000 LIFE, fixed, minted once at deployment |
| Admin functions | None: no owner, mint, burn, pause, blacklist, transfer fee or upgrade |

## Allocation and vesting

Months are 30 days, measured from TGE (Month 0).

| Allocation | Share | LIFE | Release |
|---|---:|---:|---|
| Subnet distribution | 19% | 1,900,000,000 | Unlocked at TGE to subnet treasuries |
| Subnet emission and rewards | 31% | 3,100,000,000 | 80 quarterly batches, each locked 48 months; releases Months 48–285 |
| Investors | 20% | 2,000,000,000 | 0% at TGE; 25% at Month 12; remaining 75% in 36 monthly installments, Months 13–48 |
| Advisors | 5% | 500,000,000 | Same as Investors |
| Ecosystem | 10% | 1,000,000,000 | 3-month cliff, then linear over 120 months, Months 4–123 |
| Foundation | 8% | 800,000,000 | 3-month cliff, then linear over 120 months, Months 4–123 |
| Team | 7% | 700,000,000 | 12-month cliff, then linear over 48 months, Months 13–60 |

These schedules are enforced on-chain by the vesting, emission and distribution contracts (see [Contracts & source code](contracts-and-source-code.md)).

## Deployments

| Network | Address |
|---|---|
| Avalanche Fuji testnet (43113) | [`0xb4099e22daff6f8aea114ad89194c9e9538df08e`](https://testnet.snowtrace.io/address/0xb4099e22daff6f8aea114ad89194c9e9538df08e#code) (source verified, exact match on Sourcify & Snowtrace) |
| Avalanche C-Chain mainnet (43114) | Not yet deployed |

The mainnet token will be deployed from the same source file and compiler settings, source-verified on Snowtrace and Sourcify, and its address published here.

See [Contracts & source code](contracts-and-source-code.md) for the source repository and distribution contracts.
