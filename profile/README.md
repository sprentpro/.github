<p align="center">
  <a href="https://sprent.pro/"><img src="assets/sprent.png" alt="SPRENT — on-chain market-making vault for Solana order books" width="100%"></a>
</p>

# SPRENT

**Put capital on the other side of the order book.**

SPRENT builds market-making desks on Solana. A desk holds depositor capital in a vault, quotes the Manifest order book through a restricted operator key, and settles each depositor's share of the result at epoch close.

<p>
  <a href="https://sprent.pro/"><img src="https://img.shields.io/badge/Website-sprent.pro-C2F143?style=flat-square&amp;labelColor=101113" alt="Website: sprent.pro"></a>
  <a href="https://x.com/sprent_pro"><img src="https://img.shields.io/badge/X-%40sprent__pro-101113?style=flat-square" alt="X: @sprent_pro"></a>
  <a href="https://github.com/sprent-pro/sprent"><img src="https://img.shields.io/badge/Source-sprent-101113?style=flat-square" alt="Source: sprent"></a>
  <a href="https://github.com/sprent-pro/sprent/blob/main/VERIFY.md"><img src="https://img.shields.io/badge/Read-verification-F5F4EE?style=flat-square&amp;labelColor=101113" alt="Verification record"></a>
  <a href="https://github.com/sprent-pro/sprent/actions/workflows/ci.yml"><img src="https://github.com/sprent-pro/sprent/actions/workflows/ci.yml/badge.svg" alt="Build and tests"></a>
  <a href="https://github.com/sprent-pro/sprent/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-101113?style=flat-square" alt="MIT license"></a>
</p>

## The desk

**Capital stays in the vault.** The operator can quote and cancel within the program's risk limits. It cannot pay depositor funds to an arbitrary wallet.

**Orders have limits.** Post-only execution, oracle price bands, inventory caps and an epoch loss limit constrain quoting. A halted desk can only reduce inventory.

**Settlement has a record.** Epoch close reconciles the venue and vault balances before pricing shares. Performance fees use each depositor's own high-water mark; withdrawals follow the queue and cooldown.

## Open source

| Repository | What's inside |
| :--- | :--- |
| **[sprent-pro/sprent](https://github.com/sprent-pro/sprent)** | Anchor vault program, Manifest integration, TypeScript accounting library, interface definition and tests. |

Start with the [architecture and build guide](https://github.com/sprent-pro/sprent#architecture), or inspect the [verification record](https://github.com/sprent-pro/sprent/blob/main/VERIFY.md). The repository is a source snapshot; it does not claim byte-for-byte parity with a live deployment.

## Follow the work

[Visit SPRENT](https://sprent.pro/) · [Updates on X](https://x.com/sprent_pro) · [Report a bug](https://github.com/sprent-pro/sprent/issues) · [Security policy](https://github.com/sprent-pro/sprent/blob/main/SECURITY.md)
