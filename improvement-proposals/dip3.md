# DIP-3: Vehicle Data Access Fees

> **Headline**: How developers pay per car per month to access vehicle data
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Deployed
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0x74f67d2da46e74e190063932f7b6a27fdafc7fa368ee5a275335db3a9e666499)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](dip1.md#voting-protocol)

## Abstract

Developers accessing vehicle data pay a simple fee per vehicle per month. Proceeds are partially distributed to the nodes that store the offchain vehicle data and partially kept by the DIMO protocol treasury as profit. This treasury can be reinvested or burned per future governance votes.

## Motivation

This proposal is designed to fairly compensate the DIMO protocol, as well as the node that stores the offchain data that is being accessed by the developer, in the simplest and fairest terms possible.

## Specification

### Fees

Developers accessing vehicle data pay a simple fee of 1,250 DCX ($1.25 USD) per vehicle per month of data. If they are performing a "look back" and are pulling data for previous months they did not already pay for, they pay 1,250 DCX per each previous month capped at 12,500 DCX (e.g., pulling 10, 12, or 24 months of historical data costs 12,500 DCX). The cap is inclusive of the current month.

For example, when a user first signs up in [DIMO Mobile](https://apps.apple.com/us/app/dimo-mobile/id1589486727) and the app retrieves their vehicle data, the app publisher, Digital Infrastructure Inc., must pay 1,250 DCX. If that user had already onboarded their car to DIMO a year prior using another separate DIMO app and are connecting to DIMO Mobile for the first time, the publisher pays 1,250 DCX for the current month of data plus an additional 1,250 DCX for each prior month, capped at 12,500 DCX only if they are ingesting that historical data (e.g., to show historical trips taken).

[DCX is a stable credit](dip10.md#dimo-credit-dcx) that is always worth $0.0001 USD and it can only be purchased using the $DIMO token. Websites like [console.dimo.org](https://console.dimo.org) abstract this process for the developer, allowing them to use a credit card to buy DCX in a simple flow. Once DCX is spent by a developer it is burned and cannot be reused.

Modifications and new fees can be added with future amendments. Some likely examples include:

* An increased monthly charge for video streaming from embedded cameras and dash cams;
* Fine-grained a la cart options that allow developers to pay a lower base rate per vehicle plus add-on fees for accessing telemetry, location, documents, and/or commands; and
* Per action fees such as updating vehicle permissions, pairing and unpairing a device, etc.

While fees are the same, whether a developer is just getting started or a large enterprise, the [Ignite Grants team](dip8.md) is equipped to offer grants to hobbyists and startups.

### Compensating nodes

The nodes that store vehicle data (more on what a node is [here](dip5.md#nodes)) charge developers to access vehicles using DCX, but this is not how they are compensated. DCX is non-transferrable and is burned when spent by developers.

Rather, the $DIMO that is spent to acquire DCX goes into a pool. Each month, 60% of that pool is kept by the protocol as profit. This builds up the treasury, which can be reinvested and/or burned per future governance votes. The remaining 40% is distributed to entities based on how much DCX was spent on their behalf proportional to every other node.

As an examples, let's imagine there are two nodes, Node A and Node B. In a given month, 1,125,000 DCX is burned by developers paying to access data from Node A, and 125,000 DCX is burned by developers who access data from Node B. Node A receives 36% of the pool (40% \* 90%) and Node B receives 4% (40% \* 10%).

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

## Implementation

If passed, DIP-3 would be updated as specified above after the four day timelock concludes and access fees would go into effect starting January 1, 2025.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-3: Marketplace Issuance", no. 3, November 2022. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Dec 7, 2022: added discussion forum and voting type to the DIP header.

Dec 7, 2022: adjusted review date to give people more time to claim the Airdrop prior to voting going live.

Jan 6, 2023: final adjustment to review date — proposals go to vote on Tuesday Jan 10.

Dec 26, 2023: adjusted review date again to allow for fixes to delegation strategy prior to voting.

Mar 29, 2023: passed [DIP-3: Amendment 1](../amendments/dip3a1.md)

Jul 6, 2024: disclaimer adjusted

Dec 26, 2024: passed [DIP-3: Amendment 2](../amendments/dip3a2.md)

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
