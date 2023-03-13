# DIP-7: Referrals Round 1

> **Headline**: Allocating a pool of $DIMO to launch a formal referral program&#x20;
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review (until March 22, 2023 at 12:00 UTC)
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: Level 1

## Abstract

This proposal re-establishes a formal referral program for DIMO users.

When one user refers another user who connects their first car to DIMO, both parties will receive 50 $DIMO at the end of the that week as a one-time bonus at roughly the same time as their baseline rewards. Referral bonuses will be available until the $DIMO token allocation runs out or the program is amended by a future governance vote.

## Motivation

This referral program is designed to accelerate new user onboarding, while also rewarding existing users for their continued support.

## Specification

#### Establishing a $DIMO pool for referral bonuses

This proposal sets aside a pool of 2,500,000 $DIMO to fund this referral program, meaning that only the first 25,000 referrals will earn this reward (2,500,000 $DIMO / 50 $DIMO \* 2 users per referral). This proposal may be amended by a future governance vote to top off this pool or otherwise alter referrals.&#x20;

#### Referring another user

Any user, whether they've connected a car or not, is eligible to generate a unique six digit referral code within the DIMO Mobile app. This code can be shared intimately (text it directly to a friend) or broadly (Tweeted out to the world). The referrer's personal information is not ascertainable from the referral code itself, although it's possible that in certain circumstances another user would be able to guess the blockchain address of the referrer by auditing the on-chain payout.

_Any user can refer multiple new users and earn the bonus for each new user._

#### Being referred

New users can enter a referral code as a part of onboarding as a one-time bonus. In order to be eligible, the new user must:&#x20;

1. Enter a referral code prior to connecting their first car;
2. Must be minting that specific car for the first time; and
3. Must fully connect their vehicle and qualify for one week of baseline rewards (see [dip2.md](dip2.md "mention")).

In other words, if you've already added any car to your account, you can no longer be referred (but you can still refer others). Also, if your specific vehicle was previously connected by you or another user, it will not be eligible for a referral, even if you reconnect it from scratch.

_A user can only be referred one time._

#### Payout

A one-time referral bonus of 50 $DIMO is paid out to at approximately 5:00 UTC the following Monday to both parties when a referred user meets all eligibility requirements (as specified in [#being-referred](dip7.md#being-referred "mention")) and while token supplies last (as specified in [#establishing-a-usddimo-pool-for-referral-bonuses](dip7.md#establishing-a-usddimo-pool-for-referral-bonuses "mention")).

The DIMO Foundation may delay the payout to investigate suspicious activity if there are signs of a malicious or dishonest attack. The DIMO Foundation may withhold referral bonuses from a user indefinitely at its discretion if has good reason to believe the bonus was not earned in good faith.

## Implementation

If passed, this proposal will only be enacted when a licensed DIMO client adds functionality, compliant with this specification, to enable referrals. Digital Infrastructure Inc. is currently developing new functionality into the DIMO Mobile app allowing users to generate and input referral codes. Successful referrals would be tracked and shared with the DIMO Foundation, who will conduct the weekly issuance.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-7: Referral Bonus", no. 7, February 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Mar 3, 2023: adjusted the date that the proposal is in review from March 3 to March 15. This is to create more time discussion and hopefully the introduction of a fourth proposal related to marketplace issuance that can be voted alongside the three that are currently in review.

Mar 13, 2023: extended the review period from March 15 to March 22. This is to continue to provide more time for discussion and hopefully the introduction of a fourth proposal related to marketplace issuance that can be voted alongside the three that are currently in review.

Mar 13, 2023: altered name from "Referral Bonus" to "Referral Round 1" to clarify that future referral programs need not be amendments to this proposal.

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
