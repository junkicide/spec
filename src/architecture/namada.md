# M1 Overview

M1 is a sovereign proof-of-stake blockchain, using Tendermint BFT consensus,
that enables multi-asset private transfers for any native or non-native asset
using a multi-asset shielded pool derived from the Sapling circuit. M1 features
full IBC protocol support, a natively integrated Ethereum bridge, and simple governance.
A multi-asset shielded transfer wallet is provided in order to facilitate
safe and private user interaction with the protocol.

Over time the set of supported features may be extended to include
features such as fully programmable validity predicates, distributed
key generation & threshold decryption for Ferveo, and more advanced
ZKP circuits. See [M2](./m2.md).

## Raison d'être

Safe and user-friendly multi-asset privacy doesn't yet exist in the blockchain ecosystem. Up until now you
had the choice to build a sovereign chain that reissues assets (e.g. Zcash) or to
build a privacy preserving solution on existing chains (e.g. Tornado Cash on
Ethereum). Both have large trade-offs: in the former case users don't have
assets that they actually want to use and in the latter case the restrictions
of existing platforms mean that users leak a ton of metadata
and the protocols are expensive and clunky to use.

M1 can support any asset on an IBC-compatible blockchain,
and assets sent over a custom Ethereum bridge that will
reduce transfer costs and streamline UX as much as possible.
Once assets are on M1, shielded transfers will be cheap
and all assets contribute to the same anonymity set.

M1 is also a helpful stepping stone to finalise, test,
and launch a protocol version that is simpler than the full
Anoma protocol but still encapsulates a unified and useful
set of features. There are reasons to expect that it may
make sense for a fractal instance focused exclusively on
shielded transfers to exist in the long-term, as it can
provide throughput and user-friendliness guarantees which
are more difficult to provide with a more general platform.
M1 is designed so that it could evolve into such an instance.

# Features

## Base Ledger

- [Consensus](m1/consensus.md)
- [P2P layer](m1/p2p-layer.md)
- [Execution system](m1/execution-system.md)
- [Governance](m1/governance.md)
- [Proof-of-stake](m1/proof-of-stake.md)

## Cryptography

- [Multi-asset shielded pool circuit](m1/masp.md)

## Interoperability

- [IBC integration](m1/ibc.md)
- [Bidirectional Ethereum bridge](m1/ethereum-bridge.md)

## Economics

- [Shielded pool incentives](m1/masp/shielded-pool-incentives.md)
- [Proof-of-stake reward distribution](m1/proof-of-stake/reward-distribution.md)
- [Cubic slashing](m1/proof-of-stake/cubic-slashing.md)
- [Inflation system](m1/inflation-system.md)
- [Fee system](m1/fee-system.md)

## User interfaces

- [Web-based wallet](m1/web-wallet-interface.md)
- [Web-based block explorer](m1/web-explorer-interface.md)
