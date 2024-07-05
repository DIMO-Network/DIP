# DIP-2: Amendment 2

> **Headline**: Adding baseline rewards for integration providers
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review (until July 15th, 2024 at 16:00:00 UTC)
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment adds a weekly allocation of points that goes to integrations providers so that they earn a share of the weekly baseline rewards pool. The initial values are 1,000 points per week per LTE device and 500 points per week per LoRa device or software connection.&#x20;

## Motivation

Integrations providers typically bear a cellular, cloud, and/or licensing fee to connect vehicles to DIMO each month and without this rewards mechanism, subscription fees to connect to DIMO would soon be added.  By allowing integrations providers to earn a modest amount of $DIMO with baseline each week, we can avoid instituting mandatory subscriptions while further aligning all parties.

At current issuance levels, this would come out to somewhere between 2 to 5 $DIMO per week per car and would therefore dilute user earnings by about 12% per month. It's almost as if the network grew by 12% overnight.

## Specification

<mark style="color:green;">// If passed, this proposal would incorporate the following changes to the Abstract section of DIP-2:</mark>

This proposal specifies the conditions by which DIMO users <mark style="color:red;">and integrations providers</mark> will earn baseline $DIMO token rewards for connecting to the network.

Baseline Issuance rewards users <mark style="color:red;">and integrations providers</mark> with a piece of a weekly issuance pool of $DIMO tokens. Users earn varying amounts based on how they're connected and how long they've been connected, even if there is no end customer using their data. The amount that is distributed each week will start at 1,105,000 $DIMO and will decrease 15% each year.



<mark style="color:green;">// and in the Specifications section:</mark>

Qualified users <mark style="color:red;">and entities</mark> will earn their share of this weekly issuance based on how many points they've earned relative to other users <mark style="color:red;">and entities</mark> in that period. In other words, if you earn 1% of the points in a given week, you also get 1% of the tokens distributed that week.

To be qualified for rewards, users must: ~~<mark style="color:red;">download an authorized DIMO client;</mark>~~ add their vehicle and establish an integration; complete vehicle minting and device pairing on-chain as applicable; <mark style="color:red;">maintain a verifiable credential attesting to the authenticity and uniqueness of a VIN;</mark> and transmit data each week. ~~<mark style="color:red;">As of the time of this writing,</mark>~~ [~~<mark style="color:red;">DIMO Mobile</mark>~~](http://onelink.to/dimo) ~~<mark style="color:red;">is the only authorized client.</mark>~~

...

Points <mark style="color:red;">for users</mark> are calculated as follows:

<figure><img src="../.gitbook/assets/Screenshot 2024-06-12 at 7.12.11 AM.png" alt=""><figcaption></figcaption></figure>

Users who fail to connect for three consecutive weeks will fall back one level.

In the example shown in the table above, Alice earns 2,000 points for having been connected between 2<mark style="color:red;">1</mark>~~<mark style="color:red;">0</mark>~~ to 3<mark style="color:red;">5</mark>~~<mark style="color:red;">6</mark>~~ weeks, 1,000 points for her Smartcar software connection, and 6,000 points for having <mark style="color:red;">an LTE device</mark>~~<mark style="color:red;">a Full-Size OBD Dongle</mark>~~ installed in her vehicle.

...

Curious how this would play out for people besides Alice? The table below shows earnings for a small sample of hypothetical drivers in the same hypothetical week. This is meant to be illustrative using a small handful of made up users, not an exhaustive list of every combination of attributes.

<figure><img src="../.gitbook/assets/Screenshot 2024-06-12 at 7.11.11 AM (1).png" alt=""><figcaption></figcaption></figure>

<mark style="color:red;">Additionally, integrations providers earn points, and therefore $DIMO, for the vehicle connections that they enable alongside their users. LoRa devices and software connections earn 500 points for the integrations provider. LTE devices earn 1,000 points due to the increased monthly cellular costs. Each integration has the same qualification requirements for earning each week as it does for a user; vehicles they provide the connection for must be paired, verified, and sending data.</mark>

<figure><img src="../.gitbook/assets/Screenshot 2024-06-12 at 8.16.27 AM.png" alt=""><figcaption></figcaption></figure>

## Implementation

If passed, DIP-2 would be updated and these changes implemented once the software code is audited and ready, or after the four day timelock, whichever is later.

## **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-2: Amendment 2", June 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
