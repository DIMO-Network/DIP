# DIP-3: Marketplace Issuance

> **Headline**: How protocol revenue is converted into $DIMO rewards for users
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review
>
> **Discord forum URL**: Pending
>
> **Voting URL**: Pending

## Abstract

Marketplace Issuance rewards drivers based on what third parties are paying for their data.&#x20;

It will start off very simple, but should evolve with future DIPs as the ecosystem matures and regulatory clarity improves.

The DIMO Foundation will collect proceeds from the sale of aggregate and anonymized data and, for each dollar (USD) or $DIMO token received, will burn 0.01 $DIMO and distribute the remaining 0.99 to the set of users who have opted in to data sales as a part of the vehicle pairing process.

Users may earn additional $DIMO when they use marketplace apps. The amount and terms will vary as specified by the app developer and agreed to by users so long as the reward is remitted in $DIMO and 1% is burned. The Foundation can accept cash and remit $DIMO on the apps behalf if the app developer prefers not to interact with $DIMO directly.

## Motivation

DIMO users should be rewarded primarily based on the value that they generate to create a more direct link between incentivizes and optimal behaviors. Those who create the most value for the network should have the biggest voice&#x20;

In the early stages of DIMO's development, the vast majority of rewards will come from [Baseline Issuance](dip-2-baseline-issuance.md), which is designed to simulate market demand for user data in the simplest way possible. As the network matures, this balance will likely shift the other way and the majority of rewards will come from Marketplace Issuance. This is comparable to other web3 networks like Helium, where their rewards from proof of coverage hopefully shrink in comparison to rewards from data transfer over time.

## Specification







DINC will keep 3% and remit the rest in kind

Licensed apps must pay all user referral bonuses to DIMO Foundation

Data sales = split among everyone. Add per user payment in the future. Add node subscription in the future.

Revenue split to broker









## Implementation

In order to enact the specification above, the DIMO Foundation has licensed Digital Infrastructure Inc., the publisher of [DIMO Mobile](https://onelink.to/dimo), to:

* Sell aggregate and anonymized user data to third parties in accordance with local regulations and remit proceeds to the Foundation per the specification above;
* Connect users to other applications who receive&#x20;

to confirm eligibility, calculate points, and trigger the rewards smart contract to distribute tokens. Technical documents can be found [here](https://docs.dimo.zone/docs/protocol/rewards-contract).

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-3: Marketplace Issuance", no. 3, November 2022. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

None

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
