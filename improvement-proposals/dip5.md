# DIP-5: Ecosystem

> **Headline**: How Clients, Nodes, Apps, and Data Consumers get licensed to access User data
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

Nodes store data on behalf of users and make it available to the developers with authorization from the user.

This proposal defines how these two entity types form, remain in good standing, and interact with users, their data, and the protocol itself.

## **Motivation**

The goal of this proposal is to put in place a framework that can safely and effectively grow the number of:&#x20;

* Users who will share their data, protect their privacy, spend money in the marketplace and earn rewards;&#x20;
* Number of node runners that make the data easily accessible and provably valid;
* App developers who build applications that make use of the data and connectivity;

## Specifications&#x20;

### Nodes&#x20;

A Node is an entity that stores data on behalf of users and makes it available to developers only as authorized by their users. These entities are responsible for forming and upholding agreements that protect user privacy and enable DIMO applications.&#x20;

Nodes may receive data from several protocols, such as UDP, MQTT, or Streamr Network. They provide API's and interfaces that can be used to access data, and the on-chain indexer.

All data they receive must be encrypted in transit and at rest. Both Nodes and the businesses that they serve must always comply with relevant privacy regulations (e.g., GDPR). **Node operators may only share data with licensed developers per the explicit terms of a user's active opt-in**. In other words, any Data Subscriber must receive an explicit signature from a user's wallet in order to receive their data.

Prospective Nodes may receive a license by passing a DLP that follows the [License Approval Template](../templates/license-approval-template.md) and by depositing the required $DIMO bond.

Periodically, or with a significant change in price of $DIMO, the amount required to bond will rebase automatically. Every year on January 1st, the bond amount automatically adjusts to whatever the amount of $DIMO is that is equivalent to $30,000 USD. Rebasing can also happen within the year, whenever the 7 day token weighted average price (TWAP) of $DIMO changes by 50% or more relative to the price last used to calculate the deposit amount. For example, if $DIMO is worth $2.00 on January 1st, the bond requirement is 15,000 $DIMO. If the price of $DIMO increases to $2.80, there is no change in the deposit amount. Once the token weighted average price over 7 days increases to $3.00, then the bond requirement is rebased to 10,000 $DIMO.

If the bond amount is ever decreased, existing license holders have the option to withdraw the excess amount by notifying the DIMO Foundation of their desire to do so. If the bond amount ever increases, the license holder has six months to deposit additional $DIMO to reach the new minimum.

This DIP may be updated without passing an amendment to update the bond amount below per the rules described herein.

**As of the last rebasing on July 5, 2024, the bond amount is 231,303 $DIMO.**

Past bond amounts were:

* December 12, 2022: 500,000 $DIMO

### Developers&#x20;

Developers are entities that offer services to users (e.g., a refinancing app) and/or pay users for data (e.g., an electric vehicle R\&D company). Developers must pay 100,000 DIMO Credits (DCX), which is equivalent to $100 USD, to acquire a developer license.

### Obligations

Nodes and Developers commit to maintaining strict quality and security standards, provide support for their services, always act in good faith, and agree not to engage in unlawful activities. The following is illustrative but not exhaustive.

They must not:&#x20;

* Interfere with the users safe operation of their vehicle;&#x20;
* Deliberately or negligently generate false data.&#x20;

They must:&#x20;

* Comply with all local regulations;&#x20;
* Only share data with recipients that the user has opted into sharing with per the parameters of the DIMO protocol;
* Use best practices to protect User's and their data; and
* Comply with other DIPs, particularly those that cover marketplace issuance and token burn, wherever applicable. As of the time this is written, that pertains to [dip3.md](dip3.md "mention").

### Slashing & License Revocation&#x20;

Through a governance vote, DIMO token holders have the ability alter the bonding requirements. Licensees must be given thirty days to adjust their bond to the new level.

Token holders are also able to suspend or revoke licenses through a valid governance vote if the licensee violates the obligations specified above or there is demonstrable and material negligence or malice perpetrated that harms users or the DIMO protocol generally.

## Implementation

If passed, the DIMO Foundation will issue licenses per valid governance votes, and will collect and hold bonding deposits.

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-5: App Ecosystem", no. 5, December 2022. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Dec 7, 2022: added discussion forum and voting type to the DIP header.

Dec 7, 2022: adjusted review date to give people more time to claim the Airdrop prior to voting going live.

Dec 26, 2023: adjusted review date again to allow for fixes to delegation strategy prior to voting.

Jan 6, 2023: final adjustment to review date — proposals go to vote on Tuesday Jan 10.

Jan 6, 2023: adding clarifying language on the revocation of the licenses that matches DIP-4

Jan 6, 2023: simplified the language on buying tokens from the DIMO Foundation and removed the preset exchange rate. Refer to [dip6.md](dip6.md "mention") for more on exchanging tokens with the Foundation.

Jan 9, 2023: altered labels and language to increase clarity. Simplified requirements for Applications and Data consumers. Extended the duration of Digital Infrastructure Inc's licenses.

Mar 29, 2023: passed [DIP-4 & 5: Amendment 1](../amendments/dip4-and-5a1.md)

July 6, 2024: disclaimer adjusted, updated for DLPs, and updated per [DIP-4 & 5: Amendment 2](../amendments/dip4-5a2.md)

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
