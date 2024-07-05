# DIP-2: Amendment 1

> **Headline:** Adding baseline issuance calculations for new Mini OBD device
>
> **Author:** The DIMO Foundation
>
> **Submitter(s):** The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status:** Approved
>
> **Voting URL:**[ ](https://snapshot.org/#/dimo.eth/proposal/0x74f67d2da46e74e190063932f7b6a27fdafc7fa368ee5a275335db3a9e666499)[Snapshot](https://snapshot.org/#/dimo.eth/proposal/0xbd4a05c2afa054d12b0f9255ed6c0776ee888f533ca9e0812d33f8435a8ba089)
>
> **Discussion Forum:**[ Discord](https://chat.dimo.zone/) #🗳️governance forum
>
> **Vote Type:**[ Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)​

## Abstract

This amendment to [DIP-2 ](../improvement-proposals/dip2.md)adds baseline rewards eligibility for a new category of DIMO compatible hardware, the Mini OBD Dongle. This device will earn 2,000 points per car week, plus a streak bonus. It also renames the DIMO Data Miner to the Full-size OBD Dongle to distinguish the two categories.

It also corrects a few old typos… oops!

## Motivation

The goal of Baseline Issuance is to prime the network by incentivizing drivers to connect vehicles and stream data. As demand for connected vehicle data matures, Baseline Rewards can taper off and be replaced by rewards from Marketplace Issuance.&#x20;

In DIP-2, the software and hardware connection options were given their point calculations based on how much data they stream to the network and how direct the connection is. To maintain the integrity of baseline rewards, the new Mini OBD Dongle needs to be allocated weekly points commensurate with the type and amount of data it streams to the network.&#x20;

The rationale behind the Mini OBD dongle earning 2,000 points per car per week is that it will provide the same basic data functions (GPS, Vehicle ID, etc) and simple vehicle data (hard braking, error code scanning, battery health) as a Full-size OBD dongle, but will lack more advanced data types and overall capabilities.

## Specification

<mark style="color:green;">// If passed, this proposal would incorporate the following changes to the Specification section of DIP-2:</mark>

Points are calculated as follows:

<figure><img src="https://lh4.googleusercontent.com/gohYbIl2G09qH3FVmJR4_2m6RGSjIA266meMN0P9mrwuez73Rbr6yVxcLxlF794BKpA7EbrXjeFQ1xpH5EpxqQLXxWyJS8iG5nkZzqOZIEWuSk4Pk1EZYxiHIkV1AYn3QROBAo2uALQCQ4uFB6i4_w" alt=""><figcaption></figcaption></figure>

Users who fail to connect for three consecutive weeks will fall back one level.

In the example shown in the table above, Alice earns 2,000 points for having been connected between 20 to 36 weeks, 1,000 points for her Smart<mark style="color:red;">c</mark>~~<mark style="color:red;">C</mark>~~ar software connection, and 6,000 points for having a <mark style="color:red;">Full-Size OBD Dongle</mark>[ ~~<mark style="color:red;">DIMO Data Miner</mark>~~](https://shop.dimo.zone) installed in her vehicle.

Here there are 10,000 cars connected to DIMO and each car generates an average of 6,000 points that week, for a total of 60,000,000 points. Alice's 9,000 points represent 0.015% of the points for that week (9,000 ÷ 60,000,000). Therefore, she earns 165.75 out of the 1,105,000 tokens from this pool (1,105,000 \* 0.015%).

Curious how this would play out for people besides Alice? The table below shows earnings for a small sample of hypothetical drivers in the same hypothetical week. This is meant to be illustrative using a small handful of made up users, not an exhaustive list of every combination of attributes.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

## Implementation

In accordance with DIP-6, the DIMO Foundation has engaged Digital Infrastructure Inc., to confirm eligibility and calculate points. Digital Infrastructure Inc. will update the rewards formula after the four day timelock and prior to the official launch of the first Mini OBD Dongle. Technical documents on baseline rewards can be found[ here](https://docs.dimo.zone/docs/protocol/rewards-contract).

## **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-2: Amendment 1", August 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
