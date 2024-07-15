# DIP-7: Amendment 1

> **Headline**: Extending the referrals qualification period
>
> **Author:** The DIMO Foundation
>
> **Submitter(s):** The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Voting (until July 22nd, 2024 at 18:00:00 UTC)
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0x9d93ab79916c69c1cbb3356877fb08b8d12f216511115a0572767bc4eba6c32e)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 1](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment grants additional privileges to the DIMO Foundation to use its discretion to adjust the amounts, criterion, and apps that makeup the referral program.

## Motivation

The DIMO referral program is intended to onboard legitimate new users who will embrace DIMO and remain connected. While the referrals have been a great success so far, anomalous behavior has been observed whereby vehicles will connect for a very short period to earn a week of baseline rewards and the referral bonus. Also, the price of $DIMO can often fluctuate, causing the referral bonus to be overly generous or not generous enough. This proposal addresses these issues by giving the DIMO Foundation the power to act quickly without passing a governance vote each time.

## Specification

_<mark style="color:green;">// If passed, this proposal would edit the following section within the DIP-7 Specification section:</mark>_&#x20;

#### Referring another user

Any user, whether they've connected a car or not, is eligible to generate a unique six digit referral code <mark style="color:red;">or referral link</mark> within the DIMO Mobile app <mark style="color:red;">or any other app approved by the DIMO Foundation</mark>. This code <mark style="color:red;">or link</mark> can be shared intimately (text it directly to a friend) or broadly (Tweeted out to the world). The referrer's personal information is not ascertainable from the referral code itself, although it's possible that in certain circumstances another user would be able to guess the blockchain address of the referrer by auditing the on-chain payout.

_Any user can refer multiple new users and earn the bonus for each new user._

#### Being referred

New users can <mark style="color:red;">use a referral link or</mark> enter a referral code as a part of onboarding as a one-time bonus. In order to be eligible, the new user must:&#x20;

1. <mark style="color:red;">Use a referral link or e</mark>~~<mark style="color:red;">E</mark>~~nter a referral code prior to connecting their first car;
2. Must be minting that specific car for the first time; and
3. Must fully connect their vehicle and qualify for one week of baseline rewards (see [dip2.md](../improvement-proposals/dip2.md "mention")).

#### Payout

A one-time referral bonus of 50 $DIMO is paid out to at approximately 5:00 UTC the following Monday to both parties when a referred user meets all eligibility requirements (as specified in [#being-referred](dip7a1.md#being-referred "mention")) and while token supplies last (as specified in [#establishing-a-usddimo-pool-for-referral-bonuses](dip7a1.md#establishing-a-usddimo-pool-for-referral-bonuses "mention")).

#### <mark style="color:red;">Adjustments</mark>

The DIMO Foundation may <mark style="color:red;">adjust the referral amount, criteria for earning a referral, and which apps in addition to DIMO Mobile may participate in the referral program. Also, it may</mark> delay the payout to investigate suspicious activity if there are signs of a malicious or dishonest attack. The DIMO Foundation may withhold referral bonuses from a user indefinitely at its discretion if has good reason to believe the bonus was not earned in good faith.



## Implementation

If passed, DIP-7 would be updated and these changes implemented once the software code is audited and ready, or after the four day timelock, whichever is later.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-7: Amendment 1", June 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
