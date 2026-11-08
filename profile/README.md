<p align="center">
  <a href="https://sprent.pro/"><img src="assets/sprent.png" alt="SPRENT — on-chain market-making vault for Solana order books" width="100%"></a>
</p>

<p align="center">
  <strong>CA:</strong> <a href="https://solscan.io/token/K8gETh1jTeAtMPKYyid5vFY5LrNLSNW6Yd1QZ1wpump"><code>K8gETh1jTeAtMPKYyid5vFY5LrNLSNW6Yd1QZ1wpump</code></a>
</p>

# SPRENT

**Put capital on the other side of the order book.**

SPRENT builds market-making desks on Solana. A desk holds depositor capital in a vault, quotes the Manifest order book through a restricted operator key, and settles each depositor's share of the result at epoch close.

<p>
  <a href="https://sprent.pro/"><img src="https://img.shields.io/badge/Website-sprent.pro-C2F143?style=flat-square&amp;labelColor=101113" alt="Website: sprent.pro"></a>
  <a href="https://x.com/sprent_pro"><img src="https://img.shields.io/badge/X-%40sprent__pro-101113?style=flat-square" alt="X: @sprent_pro"></a>
  <a href="https://solscan.io/account/GnfjrTU3LuytJm1BSLVWvBM721Jvs1dTQBa4aWAMUw3g"><img src="https://img.shields.io/badge/Network-mainnet-C2F143?style=flat-square&amp;labelColor=101113" alt="Live on Solana mainnet"></a>
  <a href="https://github.com/sprentpro/sprent-vault"><img src="https://img.shields.io/badge/Source-sprent--vault-101113?style=flat-square" alt="Source: sprent-vault"></a>
  <a href="https://github.com/sprentpro/sprent-vault/blob/main/VERIFY.md"><img src="https://img.shields.io/badge/Read-verification-F5F4EE?style=flat-square&amp;labelColor=101113" alt="Verification record"></a>
  <a href="https://github.com/sprentpro/sprent-vault/actions/workflows/ci.yml"><img src="https://github.com/sprentpro/sprent-vault/actions/workflows/ci.yml/badge.svg" alt="Build and tests"></a>
  <a href="https://github.com/sprentpro/sprent-vault/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-101113?style=flat-square" alt="MIT license"></a>
</p>

## The desk

**Capital stays in the vault.** The operator can quote and cancel within the program's risk limits. It cannot pay depositor funds to an arbitrary wallet.

**Orders have limits.** Post-only execution, oracle price bands, inventory caps and an epoch loss limit constrain quoting. A halted desk can only reduce inventory.

**Settlement has a record.** Epoch close reconciles the venue and vault balances before pricing shares. Performance fees use each depositor's own high-water mark; withdrawals follow the queue and cooldown.

## Live on mainnet

The [SPRENT site](https://sprent.pro/) and workers are connected to the mainnet program.

`GnfjrTU3LuytJm1BSLVWvBM721Jvs1dTQBa4aWAMUw3g`

[View the mainnet program on Solscan](https://solscan.io/account/GnfjrTU3LuytJm1BSLVWvBM721Jvs1dTQBa4aWAMUw3g) · [Deployment notes](https://github.com/sprentpro/sprent-vault#deployment-status)

## Open source

| Repository | What's inside |
| :--- | :--- |
| **[sprentpro/sprent-vault](https://github.com/sprentpro/sprent-vault)** | Anchor vault program, Manifest integration, TypeScript accounting library, interface definition and tests. |

Start with the [architecture and build guide](https://github.com/sprentpro/sprent-vault#architecture), or inspect the [verification record](https://github.com/sprentpro/sprent-vault/blob/main/VERIFY.md). The verification record includes the deployed executable hash, its comparison with the release artifact and instructions for rebuilding from public source.

## Follow the work

[Visit SPRENT](https://sprent.pro/) · [Updates on X](https://x.com/sprent_pro) · [Report a bug](https://github.com/sprentpro/sprent-vault/issues) · [Security policy](https://github.com/sprentpro/sprent-vault/blob/main/SECURITY.md)
