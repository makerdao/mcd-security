---
description: >-
  Audit reports and economic simulations for the Liquidations 2.0 upgrade of the
  Multi-Collateral Dai (MCD) Protocol
---

# Liquidations 2.0

The Liquidations 2.0 upgrade for the MCD Protocol resolves some inefficiencies in the original liquidation system by replacing the current English style auction system, where bids start low, with a new Dutch style auction system, where auction prices generally start high and drop over time. 

The key advantage to the new liquidation system is that the entire Vault’s collateral is available at a given price. As time passes, the DAI the protocol is willing to take for the collateral falls. This allows keepers to leverage all liquidity available on-chain using single block composability. 

The design is intended to reduce the risk that auctions clear at lower-than-market prices, while removing most liquidity constraints from keepers. Liquidations 2.0 is also intended to reduce price volatility risk from keepers.

For more info, read the [Maker Improvement Proposal \(MIP\) for Liquidations 2.0](https://forum.makerdao.com/t/mip45-liquidations-2-0-liq-2-0-liquidation-system-redesign/6352)

## Audit Reports

The following security **audits on the smart contracts code** have been conducted prior to the launch of the Liquidations 2.0 upgrade:

* [Quantstamp - MakerDAO Liquidations 2.0 - Final Report](https://github.com/makerdao/mcd-security/raw/master/Audit%20Reports/Liquidations_2.0/Quantstamp_MakerDAO%20Liquidations%202.0%20-%20Final%20Report%20with%20Maker%20Comments.pdf) by [Quantstamp](https://quantstamp.com/)
* [Trail of Bits - MakerDAO Liquidations 2.0 - Final Report](https://github.com/makerdao/mcd-security/raw/master/Audit%20Reports/Liquidations_2.0/Trail%20of%20Bits_MakerDAO%20Liquidations%202.0%20Final%20Report.pdf) by [Trail of Bits](https://www.trailofbits.com/)
* [ChainSecurity - MakerDAO Liquidations 2.0 - Final Report](https://github.com/makerdao/mcd-security/raw/master/Audit%20Reports/Liquidations_2.0/ChainSecurity_MakerDAO_Liquidations2.0_Final.pdf) by [ChainSecurity](https://chainsecurity.com/audits/)

### Economic Simulations

Furthermore, [Gauntlet](https://gauntlet.network/) was engaged to perform **economic simulations of Liquidations 2.0 and 1.2** for purposes of comparison on various metrics of performance, and to simulate Liquidations 2.0 under different parameter settings to inform optimally choosing these parameters for the live system. 

The report can be found at [https://maker-report.gauntlet.network/](https://maker-report.gauntlet.network/).

