# DIP-2: Amendment 4

> **Headline**: Adding a new type of boost to weekly rewards
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review (until October 15, 2024 at 16:00 UTC)
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This amendment gives users the ability to lock up $DIMO tokens to increase their weekly baseline earnings. A user who locks $DIMO in a specified quantity for a specified duration will receive a rewards boost similar to the Streak Level bonus.

The "Lock" boost is similar to the Streak boost, whereby there are four levels that offer 0, 1,000, 2,000, and 3,000 extra weekly points respectively. The Lock Level is determined by the quantity and duration that user locks their $DIMO. This boost is created on a per vehicle basis.

## Motivation

Baseline rewards exist to incentivize the development of a large and incentive-aligned network. A DIMO user who accumulates and retains large quantities of $DIMO will inevitably be a more aligned network participant than someone who is not.&#x20;

## Specification

<mark style="color:green;">// If passed, this proposal would incorporate the following changes to the Specifications section of DIP-2. These changes build off of DIP-2 amendment 3, assuming this passes. If it fails, the related changes to integration methods would be rolled back and only those new changes shown below will be incorporated:</mark>

<figure><img src="../.gitbook/assets/Screenshot 2024-10-11 at 11.11.44 PM.png" alt=""><figcaption></figcaption></figure>

<mark style="color:red;">Note that:</mark>

<mark style="color:red;">**Streak Levels**</mark><mark style="color:red;">: are tied to the vehicle, which means that swapping out an OBD device or transferring a vehicle to another user will preserve the level for that car; a streak cannot be transferred from one car to another; and vehicles that fail to connect for three consecutive weeks will fall back one streak level.</mark>

<mark style="color:red;">**Lock Levels**</mark><mark style="color:red;">: are per vehicle (e.g., it would take 8,000 $DIMO to boost two separate vehicles to level 4); may be assigned and unassigned to any car in your account; and can be upgraded at any time, but cannot be downgraded prematurely (e.g., you can roll 500 $DIMO from a level 1 contract that is still locked, add 1,000 more $DIMO, and upgrade it to a new level 2 contract that restarts the lock period).</mark>

<mark style="color:red;">**Connection types**</mark><mark style="color:red;">: to be considered "comprehensive", an integration must send extensive telemetry data in near real-time. As of the last update of this proposal, the AutoPi, LTE R1 and native Tesla connections qualify as "comprehensive" integrations.</mark>

<mark style="color:red;">Every box depicting points can stack on one another. This means that a car can have a streak level, a boost level, a software connection, and hardware connection for a maximum 16,000 weekly points. A car must send valid data to qualify for rewards in a given week. If a car isn't driven, it will receive zero $DIMO regardless of any streak or boost.</mark>

~~<mark style="color:red;">To be considered "Comprehensive", an integration must send extensive telemetry data in near real-time.</mark>~~

~~<mark style="color:red;">Users who fail to connect for three consecutive weeks will fall back one level.</mark>~~

In the example shown in the table above, Alice earns 2,000 points for having been connected between 21 to 35 weeks, <mark style="color:red;">1,000 points for locking 500 $DIMO for 6 months,</mark> 1,000 points for her Limited software connection, and 6,000 points for having comprehensive installed in her vehicle.

Here there are 40,000 cars connected to DIMO and each car generates an average of 6,000 points that week, for a total of 240,000,000 points. Alice's <mark style="color:red;">10</mark>~~<mark style="color:red;">9</mark>~~,000 points represent 0.004% of the points for that week (<mark style="color:red;">10</mark>~~<mark style="color:red;">9</mark>~~,000 ÷ 240,000,000). Therefore, she earns <mark style="color:red;">46.04</mark>~~<mark style="color:red;">41.44</mark>~~ out of the 1,105,000 tokens from this pool (1,105,000 \* 0.004%).

...

<figure><img src="../.gitbook/assets/Screenshot 2024-09-30 at 5.58.38 PM.png" alt=""><figcaption></figcaption></figure>

## Implementation

If passed, DIP-2 would be updated and these changes implemented once the code is ready, or after the four day timelock, whichever is later. This would be expected to launch by the end of 2024 or early 2025.

## **Copyright**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-2: Amendment 4", October 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Oct 11, 2024: Updated lock level requirements (decreased the amounts).

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
