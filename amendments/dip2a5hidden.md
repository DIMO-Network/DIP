---
hidden: true
---

# DIP-2: Amendment 5

> **Headline**: Adding baseline rewards for integration providers
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Draft
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment adds a weekly allocation of points that goes to integrations providers (e.g., Tesla) so that they earn a share of the weekly baseline rewards pool. The initial value is 500 points per active integration.

If Digital Infrastructure Inc. maintains the integration on behalf of a third party, they shall hold the tokens in escrow for that third party and may only deduct tokens as needed to cover the cost charged directly by the third party and/or the SIM provider.&#x20;

For example, imagine Digital Infrastructure maintains a Kia integration and receives $4 USD worth of tokens per vehicle per month. If Kia charges Digital Infrastructure Inc. $5 per month, Digital Infrastructure Inc. keeps all of the $DIMO. If Kia charges $1 per month, they keep $1 worth and hold the other $3 worth of $DIMO for Kia to claim at any point.

## Motivation

Integrations providers typically bear a cellular, cloud, and/or licensing fee to connect vehicles to DIMO each month and without this rewards mechanism, subscription fees to connect to DIMO would soon be added.  By allowing integrations providers to earn a modest amount of $DIMO with baseline each week, we can avoid instituting mandatory subscriptions while further aligning all parties by allowing them a natural pathway to accumulate $DIMO tokens.

**Long-term automakers should host these integrations themselves and become major stakeholders of the DIMO ecosystem and holders of $DIMO.**

At current issuance levels, this would come out to somewhere around 2 $DIMO per week per car and would therefore dilute user earnings by about 8.5% per month. It's almost as if the network grew by 8.5% overnight.

## Specification

<mark style="color:green;">// If passed, this proposal would incorporate the following changes to the Abstract section of DIP-2:</mark>

This proposal specifies the conditions by which DIMO users <mark style="color:red;">and integrations providers</mark> will earn baseline $DIMO token rewards for connecting to the network.

Baseline Issuance rewards users <mark style="color:red;">and integrations providers</mark> with a piece of a weekly issuance pool of $DIMO tokens.

<mark style="color:green;">// and in the Specifications section:</mark>

Qualified users <mark style="color:red;">and entities</mark> will earn their share of this weekly issuance based on how many points they've earned relative to other users <mark style="color:red;">and entities</mark> in that period. In other words, if you earn 1% of the points in a given week, you also get 1% of the tokens distributed that week.

...

<mark style="color:red;">Additionally, integrations providers earn 500 points, and therefore $DIMO, for the vehicle connections that they enable alongside their users. Each integration has the same qualification requirements for earning each week as it does for a user; vehicles they provide the connection for must be paired, verified, and sending data.</mark>

<figure><img src="../.gitbook/assets/Screenshot 2024-09-30 at 9.25.31 PM.png" alt=""><figcaption></figcaption></figure>

<mark style="color:red;">If Digital Infrastructure Inc. maintains the integration on behalf of a third party, they shall hold the tokens in escrow for that third party and may only deduct tokens as needed to cover the cost charged directly by the third party and/or the SIM provider.</mark>&#x20;

<mark style="color:red;">For example, imagine Digital Infrastructure maintains a Kia integration and receives $4 USD worth of tokens per vehicle per month. If Kia charges Digital Infrastructure Inc. $5 per month, Digital Infrastructure Inc. keeps all of the $DIMO. If Kia charges $1 per month, they keep $1 worth and hold the other $3 worth of $DIMO for Kia to claim.</mark>

## Implementation

If passed, DIP-2 would be updated and these changes implemented once the software code is audited and ready, or after the four day timelock, whichever is later.  This would be expected to launch by the end of 2024.

## **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-2: Amendment 2", October 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
