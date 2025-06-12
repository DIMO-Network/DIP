---
hidden: true
---

# \*\*\*DIP-10: Amendment 1

> **Headline**: Adding a native SPL $DIMO token on Solana
>
> **Author:** The DIMO Foundation
>
> **Submitter(s):** The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment adds an official $DIMO token on the Solana blockchain.

It also tweaks the DIMO Credit minting flow to incorporate USDC support.

## Motivation

Solana has emerged as a meaningful blockchain that many DIMO users already know and love to use. By allowing $DIMO to seamlessly bridge to Solana, users are able to utilize their tokens with the Solana wallets and apps they already love using.

Additionally, we can streamline DIMO Credit purchases by allowing them to be created with USDC, prior to converting USDC to $DIMO and burning it. This makes the developer experience more efficient and simple, while preserving the automated $DIMO token burn.

## Specification

_<mark style="color:green;">// If passed, this proposal would edit the following section within the DIP-10 Specification section:</mark>_&#x20;

### The DIMO token ($DIMO)

_The primary token of the DIMO ecosystem used for governance, staking, and payments_&#x20;

[**Ethereum**](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b)

Address: 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b&#x20;

Key properties: Native bridging support (can be <mark style="color:red;">locked/unlocked</mark>~~<mark style="color:red;">minted/burned</mark>~~ via [~~<mark style="color:red;">Polygon Bridge</mark>~~](https://portal.polygon.technology/bridge) ~~<mark style="color:red;">&</mark>~~ [Wormhole NTT](https://wormhole.com/products/native-token-transfers)), governance delegation, upgradeable by DIMO Foundation multi-signature contract.

[**Base**](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) **/** [**Optimism**](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c)

Address: 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c

Key properties: Native bridging support (can be minted/burned via [Wormhole NTT](https://wormhole.com/products/native-token-transfers)), governance delegation, upgradeable by DIMO Foundation multi-signature contract.

[**Polygon**](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db)

Address: 0xE261D618a959aFfFd53168Cd07D12E37B26761db

Key properties: Native bridging support (can be minted/burned via [~~<mark style="color:red;">Polygon Bridge</mark>~~](https://portal.polygon.technology/bridge) ~~<mark style="color:red;">&</mark>~~ [Wormhole NTT](https://wormhole.com/products/native-token-transfers)), governance delegation, upgradeable by DIMO Foundation multi-signature contract.

[<mark style="color:red;">**Solana**</mark>](https://solscan.io/token/ERQXNXuWfpaGMh9Cs19zxcQTtzCVNZerdKXJ7BQKXVhd)

<mark style="color:red;">Address: ERQXNXuWfpaGMh9Cs19zxcQTtzCVNZerdKXJ7BQKXVhd</mark>

<mark style="color:red;">Key properties: Native bridging support (can be minted/burned via</mark> [<mark style="color:red;">Wormhole NTT</mark>](https://wormhole.com/products/native-token-transfers)<mark style="color:red;">), upgradeable by DIMO Foundation multi-signature contract.</mark>

...

## Implementation

If passed, DIP-10 would be updated after the four day timelock. The Solana version of $DIMO will be recognized immediately once deployed. The adjustment to the DIMO Credit purchase flow will be deployed once the relevant contract updates are completed and audited. All disclaimers on every DIP and amendment will be updated to include the Solana token.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-10: Amendment 1", May 2025. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
