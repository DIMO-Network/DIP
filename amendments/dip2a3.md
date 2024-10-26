# DIP-2: Amendment 3

> **Headline**: Adjusting points by integration type
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Deployed
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0x6169051cbf2aa31226a6c15a2634fbf8907a459cc362cba9e3991a604031cbec)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment reframes the points categories by integration type.

## Motivation

The new [DIMO LTE R1 by Ruptela](../license-proposals/dlp5.md), along with anticipated improvements to software connections, have exposed shortcomings in the current classifications around points for integration types. This proposal would reorient the language more clearly around data potential.&#x20;

It also increases the rewards for more limited OBD devices by 1,000 points, due to the Macaron having outperformed expectations on coverage and data throughput.

You might ask, "why do device connections continue earn more points than software connections?" This is because software connections cost more to maintain, require no upfront cost by the user, and, at least for now, require dependencies on third parties that could easily lead to disruptions. The OBD port, on the other hand, is protected by right to repair and privacy regulations and will remain accessible always.&#x20;

Nearly all cars that can connect via software can also add a hardware connection whereby rewards for both stack on top of each other, as shown in the example.

## Specification

<mark style="color:green;">// If passed, this proposal would incorporate the following changes to the Specifications section of DIP-2:</mark>

In year one, DIMO will issue 1,105,000 $DIMO per week to all qualified DIMO users at 5 AM UTC each Monday. This issuance amount will automatically decrease by 15% every <mark style="color:red;">52 weeks following the anniversary of the December 12, 2024 mainnet launch</mark>~~<mark style="color:red;">year</mark>~~, with Baseline Issuance ending in 40 years, unless modified by a future DIP.

...

Points <mark style="color:red;">for users</mark> are calculated as follows:

<figure><img src="../.gitbook/assets/Screenshot 2024-09-30 at 5.57.00 PM.png" alt=""><figcaption></figcaption></figure>

<mark style="color:red;">**Connection types**</mark><mark style="color:red;">: to be considered "Comprehensive", an integration must send extensive telemetry data in near real-time. As of the last update of this proposal, the AutoPi, LTE R1 and native Tesla connection qualify as comprehensive.</mark>

Users who fail to connect for three consecutive weeks will fall back one level.

In the example shown in the table above, Alice earns 2,000 points for having been connected between 2<mark style="color:red;">1</mark>~~<mark style="color:red;">0</mark>~~ to 3<mark style="color:red;">5</mark>~~<mark style="color:red;">6</mark>~~ weeks, 1,000 points for her Limited software connection, and 6,000 points for having <mark style="color:red;">comprehensive device</mark>~~<mark style="color:red;">a Full-Size OBD Dongle</mark>~~ installed in her vehicle.

Here there are <mark style="color:red;">4</mark>~~<mark style="color:red;">1</mark>~~0,000 cars connected to DIMO and each car generates an average of 6,000 points that week, for a total of <mark style="color:red;">24</mark>~~<mark style="color:red;">6</mark>~~0,000,000 points. Alice's 9,000 points represent 0.0<mark style="color:red;">04</mark>~~<mark style="color:red;">15</mark>~~% of the points for that week (9,000 ÷ <mark style="color:red;">24</mark>~~<mark style="color:red;">6</mark>~~0,000,000). Therefore, she earns <mark style="color:red;">41.44</mark>~~<mark style="color:red;">165.75</mark>~~ out of the 1,105,000 tokens from this pool (1,105,000 \* 0.0<mark style="color:red;">04</mark>~~<mark style="color:red;">15</mark>~~%).

...

<figure><img src="../.gitbook/assets/Screenshot 2024-09-30 at 5.55.05 PM.png" alt=""><figcaption></figcaption></figure>

## Implementation

If passed, DIP-2 would be updated and these changes implemented once the software code is ready, or after the four day timelock, whichever is later.

## **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-2: Amendment 3", October 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
