# DIP-3: Marketplace Issuance & Token Burn

> **Headline**: How transactions are converted into $DIMO rewards for users
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

Transactions enabled by DIMO Apps generate additional $DIMO rewards for users, known as Marketplace Issuance. This is in addition to [Baseline Issuance](../dip-2-baseline-issuance.md). These transactions will also generate a $DIMO token burn.&#x20;

It will start off very simple, but can evolve with future DIPs as the ecosystem matures and regulatory clarity improves.

## Motivation

DIMO users and apps should be rewarded based on the value that they generate to create a more direct link between incentives and optimal behaviors. Those who create the most value for the network should have the largest $DIMO rewards and the biggest voice in its future direction.

In the early stages of DIMO's development, the vast majority of rewards will come from [Baseline Issuance](dip2.md), which is designed to simulate market demand for user data in the simplest way possible. As the network matures, this balance will shift so the majority of rewards come from Marketplace Issuance. This is comparable to other web3 networks like Helium, where the rewards from proof of coverage ideally shrink in comparison to rewards from data transfer as adoption increases.

## Specification

### Market Issuance

Users are able to opt-in to sharing data with licensed DIMO Apps. These apps must specify what data they are collecting, what they may do with it, and what portion of any data sales revenue that they will keep, if applicable.

For all transactions involving the sale of user data or access, the amount will be translated to $DIMO tokens and the portion owed to the user will be distributed in $DIMO and 1% of the transaction will be burned.

If the the transaction is denominated in $DIMO, the calculation is obvious. If denominated or paid in fiat (USD, EUR, GBP) or other assets (DAI, BTC, ETH), amounts are converted to $DIMO at the current market price at the time of the transaction. The node operator may choose between CoinMarketCap and CoinGecko for the price oracle.

The easiest way to understand this mechanism is through examples of various transaction types, all listed below.&#x20;

For simplicity, these examples assume a market price of $10 USD per $DIMO token and round to two decimal points.

#### Example 1: The sale of aggregate and anonymized user data

Marketplace Issuance generated by the sale of aggregate and anonymized data is split evenly among all users who are currently opted into and contributing data to that data pool at the time the reward is distributed.

_Hypothetical Example:_ You grant DIMO Explorer, a licensed DIMO App, the right to sell your aggregate and anonymized data when you opt-in to Baseline Rewards. As a part of the opt-in, users agree that Explorer keeps a 5% cut for their efforts, leaving users with 95%. In 2023, Explorer generates $1,000,000 in USD by selling reports on overall traffic patterns, battery performance, self-driving system usage, road quality, and other driving behaviors.

* **Burn**: 1,000 $DIMO ($1,000,000 / 10 $perDIMO x 1%)
* **Settlement**:&#x20;
  * Explorer receives $49,500 USD ($1,000,000 x 99% x 5%)
  * Users receive 94,050 $DIMO ($1,000,000 / 10 $perDIMO x 99% x 95%)

<img src="../.gitbook/assets/file.drawing (1).svg" alt="" class="gitbook-drawing">

#### Example 2: The sale of disaggregated user data

Marketplace Issuance generated by the direct sale of user data will go to the respective user. 99% of net proceeds are issued to the user and 1% is burned.

_Hypothetical Example:_ You grant DataWiz, a DIMO App, the right to sell your anonymized but disaggregated (vehicle specific data). You share trip telemetry data and vehicle status, but not location or glovebox (license, title, insurance) data. You agree to DataWiz's license agreement that gives them a 5% cut of your data sales.

Verizon subscribes to your cell coverage data so they can map their signal strength. Panasonic subscribes to your battery data, which they use to improve their designs. Other businesses subscribe to similar streams. DataWiz receives an aggregate $60/month in USD from brokering your data.

* **Burn**: 0.06 $DIMO each month ($60 / 10 $perDIMO x 1%)
* **Settlement**:&#x20;
  * DataWiz receives $2.97/month USD ($60 x 99% x 5%)
  * You receive 5.64 $DIMO per month ($60 / 10 $perDIMO x 99% x 95%)

<img src="../.gitbook/assets/file.drawing (3).svg" alt="" class="gitbook-drawing">

#### Example 3: Direct incentives

Marketplace Issuance may also be earned directly from apps. Incentives must be in $DIMO. 99% of the incentive is issued to the user and 1% is burned.&#x20;

_Hypothetical Example:_ All Farm Insurance is a DIMO App that gives new customers 50 $DIMO when they switch to All Farm and share their vehicle health, location, and mileage data for better insurance rates.

* **Burn**: 0.51 $DIMO (50.5 x 1%)
* **Settlement**:&#x20;
  * You receive 500 $DIMO (50.50 x 99%)

<img src="../.gitbook/assets/file.drawing (1) (2).svg" alt="" class="gitbook-drawing">

### Market Issuance from transactions involving goods & services

In the future, transactions on top of DIMO rails that involve payment for goods and services can also generate rewards and token burn.&#x20;

For example, you drive for, _RID3SHAR3_, a better DIMO-fied version of Uber. A passenger pays $40 USD for you to drive them to the airport. 1% is translated to $DIMO and burned. Some or all of the payment you receive is translated into $DIMO.

Loan payments, insurance payments, car sales, and other transactions can generate $DIMO token burn and rewards.

This mechanism should be implemented at a time in the future when DIMO adoption and regulatory clarity are suitably far along.

## Implementation

In order to enact the specification above, the DIMO Foundation will issue licenses to DIMO Applications, per [DIP-5](dip5.md), that specify the terms by which those applications handle user data and remit cash or $DIMO.&#x20;

DIMO apps may burn and distribute $DIMO directly. In cases where DIMO apps do not have or wish to use $DIMO, or do not wish to handle the distribution directly, the DIMO Foundation will assist in conversions and distributions. The DIMO Foundation reserves the right limit or deny the service of assisting third parties in exchanging fiat or other crypto for $DIMO, or to use a higher price for $DIMO if, for example, it determines there isn't sufficient actual volume or genuine price discovery to give legitimacy to the market price, or if the asset being exchanged is difficult or unwise to accept.

To assist in this matter, the DIMO Foundation has engaged Digital Infrastructure Inc. to process data and calculate distributions. As is the case with Baseline Issuance, user<mark style="color:red;">s</mark> are not eligible for rewards if their wallets are flagged by Chainalysis' [AML tools](https://www.chainalysis.com/free-cryptocurrency-sanctions-screening-tools/) as risky or fraudulent.

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

July 6, 2024: disclaimer adjusted

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
