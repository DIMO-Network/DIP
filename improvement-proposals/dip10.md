# DIP-10: Network Tokens

> **Headline**: Clarifying the role of various fungible DIMO protocol tokens&#x20;
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Deployed
>
> **Voting URL**: [Snapshot](https://snapshot.box/#/s:dimo.eth/proposal/0x2b5d8aee4a334c3537702df3a4cfdb93b889b122ad3e373f6452edc7f148d27b)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](dip1.md#voting-protocol)

## Abstract

This proposal lists out core DIMO protocol fungible tokens on each chain and describes their properties.

## Motivation

As the number of chains and tokens in the DIMO ecosystem expands, it's important to clarify the authenticity and role of each token on each chain.

## Specification

The following tokens are officially recognized fungible DIMO network tokens.

### The DIMO token ($DIMO)

_The primary token of the DIMO ecosystem used for governance, staking, and payments_&#x20;

[**Ethereum**](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b)

Address: 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b&#x20;

Key properties: Native bridging support (can be minted/burned via [Polygon Bridge](https://portal.polygon.technology/bridge) & [Wormhole NTT](https://wormhole.com/products/native-token-transfers)), governance delegation, upgradeable by DIMO Foundation multi-signature contract.

[**Base**](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) **/** [**Optimism**](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c)

Address: 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c

Key properties: Native bridging support (can be minted/burned via [Wormhole NTT](https://wormhole.com/products/native-token-transfers)), governance delegation, upgradeable by DIMO Foundation multi-signature contract.

[**Polygon**](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db)

Address: 0xE261D618a959aFfFd53168Cd07D12E37B26761db

Key properties: Native bridging support (can be minted/burned via [Polygon Bridge](https://portal.polygon.technology/bridge) & [Wormhole NTT](https://wormhole.com/products/native-token-transfers)), governance delegation, upgradeable by DIMO Foundation multi-signature contract.

### DIMO Credit (DCX)

_A stable credit pegged to $0.0001 USD that can only be created and purchased with $DIMO. Once DCX is spent, it is burned and cannot be reused._

[**Polygon**](https://polygonscan.com/address/0x7186F9aC35d24c9a4cf1E58a797c04DF1b334322)

Address: 0x7186F9aC35d24c9a4cf1E58a797c04DF1b334322

Key properties: Non-transferrable, upgradeable by DIMO Foundation multi-signature contract.

### Suggested Bridges

DIMO recommends use of the [Wormhole Native Token Transfer](https://wormhole.com/products/native-token-transfers) bridging system to move $DIMO between Ethereum and Polygon. While Wormhole is a popular product used by many other blockchain tokens and trusted to do an excellent job, they are third party and DIMO is not responsible for their performance.

### Unofficial Wrapped or Derivative Tokens

An important feature of blockchain is that anyone can permissionlessly create wrapped or derivative versions of any token to expand their capabilities.

Unofficial wrapped assets: typically this entails locking up tokens on one chain and minting a corresponding token on another chain so that the asset can "bridge" to the new chain. The asset can move around the new chain freely and the only way to unlock the token on the original chain is to either lock or burn the token on the new chain.

Unofficial derivative assets: these are assets that derive their value in someway from another underlying token, typically as futures, options, or yield-bearing tokens.

Exercise caution when interacting with such products as they are created by unaffiliated third parties who may not guarantee security, performance, and legality.

### Related Audits

{% file src="../.gitbook/assets/Sigma Prime Audit 1.pdf" %}

{% file src="../.gitbook/assets/Sayfer Audit 1.pdf" %}

{% file src="../.gitbook/assets/Sayfer Audit 2.pdf" %}

## Implementation

$DIMO on the aforementioned chains has already been deployed and is immediately functional, but will not achieve "official status" until this DIP Is passed and the four day timelock concludes.&#x20;

Updates will be made to every disclaimer in this repository to include the contract addresses of the tokens described herein.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP - 10: The $DIMO Token", no. 10, November 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Dec 9, 2024: Added Base and Optimism $DIMO contract addresses

Feb 7, 2025: Corrected a typo. 1 DCX has always equalled $0.0001 USD, not $0.001 USD

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
