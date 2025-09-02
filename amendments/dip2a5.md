# DIP-2: Amendment 5

> **Headline**: Simplifying the connection level system and increasing Tesla rewards
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Deployed
>
> **Voting URL**: [Snapshot](https://snapshot.box/#/s:dimo.eth/proposal/0x64f8a9a250a4519cbe6563f23d64640e21dd109c18e3c1c295bcf9d85ca18015)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 1](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment replaces the current "Limited" and "Comprehensive" connection categories with a 3-6 level system that raises the bar for qualified connections. Levels range from Level 3 (moderate data updated every minute) to Level 6 (comprehensive real-time data), with progressively higher weekly point rewards incentivizing higher-quality connections.

All reward boosts are consolidated into the level system, simplifying how boosts stack. A connection registry clarifies which integrations qualify for each level and their designated hosts.

Tesla's native connection from Digital Infrastructure Inc. is upgraded to Level 6 due to improved polling, achieving parity with R1 and AutoPi. The classic Smartcar integration becomes ineligible due to limited data liveness, though a future enhanced Smartcar product could qualify for Level 6 when available.

## Motivation

The current binary system inadequately reflects data quality spectrum and fails to establish minimum network participation standards. By raising the qualification floor to Level 3, this amendment addresses a key product-market fit challenge: app developers and users struggle to derive meaningful value from limited connections, so these have been eliminated from earning eligibility.

The 3-6 level system ensures only valuable data contributors receive rewards while properly compensating based on actual network contribution. Consolidating all boosts into the level system eliminates reward calculation complexity.

The connection registry brings transparency to qualification criteria. Tesla's technical improvements warrant Level 6 recognition alongside premium hardware solutions, while legacy integrations failing to meet modern standards are excluded to maintain network quality.

This framework strengthens incentive alignment between data value and rewards while establishing quality thresholds that improve overall network utility for developers and end users.

## Specification

<mark style="color:green;">// If passed, this proposal would incorporate the following changes to the Specifications section of DIP-2:</mark>

<figure><img src="../.gitbook/assets/Screenshot 2025-06-11 at 10.34.28 PM.png" alt="" width="563"><figcaption></figcaption></figure>

...

**Connection types**: <mark style="color:red;">Currently licensed connections are categorized as follows:</mark>

<mark style="color:red;">Level 6: R1 by Ruptela, AutoPi x DIMO by AutoPi, Tesla in collaboration with Digital Infrastructure Inc., Enhanced Wireless by Smartcar in collaboration with Digital Infrastructure Inc.</mark>

<mark style="color:red;">Level 3: Macaron by Hashdog</mark>

~~<mark style="color:red;">to be considered "comprehensive", an integration must send extensive telemetry data in near real-time. As of the last update of this proposal, the AutoPi, LTE R1 and native Tesla connections qualify as "comprehensive" integrations.</mark>~~

Every box depicting points can stack on one another. This means that a car can have a streak level, a boost level, <mark style="color:red;">on top of their data connection for a maximum level of 12</mark>  <mark style="color:red;"></mark>~~<mark style="color:red;">a software connection, and hardware connection for a maximum 16,000 weekly points</mark>~~. A car must send valid data to qualify for rewards in a given week. If a car isn't driven, it will receive zero $DIMO regardless of any streak or boost.

In the example shown in the table above, Alice earns <mark style="color:red;">1 levels</mark>~~<mark style="color:red;">2,000 points</mark>~~ for having been connected between 21 to 35 weeks, <mark style="color:red;">2 levels</mark>~~<mark style="color:red;">1,000 points</mark>~~ for locking <mark style="color:red;">1</mark>500 $DIMO for <mark style="color:red;">12</mark>~~<mark style="color:red;">6</mark>~~ months~~<mark style="color:red;">, 1,000 points for her Limited software connection,</mark>~~ and <mark style="color:red;">6 levels</mark>~~<mark style="color:red;">,000 points</mark>~~ for having a <mark style="color:red;">premium connection</mark> for ~~<mark style="color:red;">comprehensive device installed in</mark>~~ her vehicle.

Here there are 40,000 cars connected to DIMO and each car generates an average of <mark style="color:red;">6 levels</mark>~~<mark style="color:red;">,000 points</mark>~~ that week, for a total of 240,000 <mark style="color:red;">levels</mark>~~<mark style="color:red;">,000 points</mark>~~. Alice's <mark style="color:red;">9 levels</mark>~~<mark style="color:red;">10,000 points</mark>~~ represent 0.00<mark style="color:red;">375</mark>~~<mark style="color:red;">4</mark>~~% of the <mark style="color:red;">levels</mark>~~<mark style="color:red;">points</mark>~~ for that week (<mark style="color:red;">9</mark>~~<mark style="color:red;">10,000</mark>~~ ÷ 240,000~~<mark style="color:red;">,000</mark>~~). Therefore, she earns <mark style="color:red;">41.4375</mark>~~<mark style="color:red;">46.04</mark>~~ out of the 1,105,000 tokens from this pool (1,105,000 \* 0.00<mark style="color:red;">375</mark>~~<mark style="color:red;">4</mark>~~%).

Curious how this would play out for people besides Alice? The table below shows earnings for a small sample of hypothetical drivers in the same hypothetical week. This is meant to be illustrative using a small handful of made up users, not an exhaustive list of every combination of attributes.

<figure><img src="../.gitbook/assets/Screenshot 2025-06-11 at 10.32.40 PM.png" alt=""><figcaption></figcaption></figure>

## Implementation

If passed, DIP-2 would be updated and these changes implemented after the four day timelock.

## **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-2: Amendment 5", June 2025. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
