# DIP-4: Device Integrations

> **Headline**: Expanding the ecosystem of DIMO compatible hardware devices and software connection methods
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

This proposal outlines the method by which hardware manufacturers (like [AutoPi](https://www.autopi.io/)) who produce compatible devices, as well as software developers (like Digital Infrastructure Inc.) who build digital integrations (collectively referred to as integration providers) bond $DIMO and receive a license.

The requirements for any integration providers are that they must:&#x20;

1. Pass a DLP that approves their license application;
2. Bond $DIMO tokens as a security deposit;&#x20;
3. Pay the applicable amount of DIMO Credits (DCX) for each integration they enable; and
4. Remain in good standing with the community.&#x20;

## Motivation&#x20;

As a part of the vision to establish DIMO as a decentralized universal protocol, it is important to develop a robust and diverse ecosystem of manufacturers producing DIMO compatible hardware and software companies providing digital integrations.

The goals of this proposal are to:&#x20;

* Onboard and retain hardware providers (OEMs), software integrations, retailers, distributors, and support channels that are tightly aligned with the interests of the DIMO protocol and its users;&#x20;
* Accelerate the development and integration of new device types and integration methods such as dash cameras, cheaper dongles, embedded hardware, and more; and&#x20;
* Optimize the operations and financing of device production, fulfillment, and installation.

## Specifications&#x20;

### Integration Providers & Device Licenses

In order to connect to DIMO users, their vehicles, and their data, integration providers must agree to various obligations, receive a license by passing a DLP, bond the required amount, and pay DCX for each device they sell.

#### Obligations

Integration providers commit to maintaining strict quality and security standards, provide support for their services, always act in good faith, and agree not to engage in unlawful activities. The following is illustrative but not exhaustive.

Connection methods must not:&#x20;

* Interfere with the users safe operation of their vehicle;&#x20;
* Damage the vehicle it is installed in;&#x20;
* Deliberately or negligently generate false data.&#x20;

Connection methods must:&#x20;

* Comply with all local regulations;&#x20;
* Receive adequate support from the provider for a reasonable duration of time;&#x20;
* Perform as expected; and
* Only share data with recipients that the user has opted into sharing with per the parameters of the DIMO protocol.

#### Application&#x20;

Prospective integration providers may receive a license by passing a DLP using the [License Approval Template](../templates/license-approval-template.md). The application must provide details about their business, their operating history, as well as specifications for the initial devices they intend to manufacture and/or software services they intend to provide.&#x20;

The DLP must contain specifications for at least one device design, test units, and data samples and/or a code repository and a functioning demo. Licensed providers are able to submit additional and simplified applications for new devices and software methods at any time.

#### Connection Specifications&#x20;

The following are minimum device specifications.

Both Hardware & Software

<table><thead><tr><th width="171.16385091122186">Certification</th><th>Description</th></tr></thead><tbody><tr><td>Power management</td><td>DIMO compatible devices must implement power management to prevent phantom drain of the vehicles it connects to, and efficiently manage being in “sleep” mode.</td></tr><tr><td>Secure runtime</td><td>Security is of highest importance to DIMO for both safety and security of the users. To provide an additional layer of safety to the car and the user, DIMO devices must run signed and verified code. Hardware must use secure boot mechanisms.</td></tr><tr><td>Streaming interface</td><td>DIMO Integrations will provide a specification for how the data should be formatted (schema) and sent to the protocol (delivery). Initially, the data will be sent in compressed json, moving to more efficient binary methods of encoding such as protobuf or avro.</td></tr><tr><td>Approved geography</td><td>Currently, devices may only operate within the United States of America, Canada, and Europe. Support for new regions may be added by the DIMO community in future DIPs.</td></tr></tbody></table>

Hardware Only&#x20;

<table><thead><tr><th width="168.58734683468623">Certification</th><th>Description</th></tr></thead><tbody><tr><td>Hardware secure element &#x26; EVM wallet</td><td>The identity of the device and the vehicle it is connected to is of high importance. In web3, this is known as a “wallet”, but is essentially a private key to identify the device. To limit spoofing, DIMO requires the private keys to be stored inside a hardware secure element. This key is also used for encrypted, secure transmission of vehicle data. Each device should contain its own EVM compatible wallet.</td></tr><tr><td>DBC logger configuration</td><td>Each vehicle is different and provides different signals on the canbus. To handle this variety of messages, DIMO maintains an open repository [OPENDBC]. To be compatible with DIMO, the device must accept dynamic configuration of signals for filtering, parsing, and delivery to the protocol.</td></tr><tr><td>OTA process</td><td>To be accepted into the program, the device manufacturer must routinely support and update their devices as new vulnerabilities are found. This must be able to be done via cellular connection.</td></tr><tr><td>3rd party certifications</td><td><p>CE Certifications EN 301 489-1 v2.2.0 EN55025:2008 EN 50498 and Directive 2004/104/EC ISO 7637-2:2011 EN 301 489-3 V2.1.1 <img src="https://lh4.googleusercontent.com/E_LfSnGkea7mAmpWINsnajyDt8F4sbSyGW3AYIMMidRF92y6GiV_nJ8tgZMILXp3A4V4IQbAcg3d_6DEhFTHYbb3Aggjnv2STFXto4MhDgPs9SnVVK0n1d1vkJD8mJCkZ5SrLzSYLGR1TSw_XbHjJg" alt="AutoPi.io - CE Certified" data-size="line"></p><p>FCC Certifications Devices certified under the following standards: FCC 47 CFR Part 15, Class A:10–1–17 Edition <img src="https://lh6.googleusercontent.com/OX11obGi-bwDcoF0vgnN1-imk7w_9o6-G9c624gYqDSeOj29p4oxy-8ByicOyEgLGfnP9sXxuOXGEg2HsjE_jwNUt7IEc317ai13cr0bllaOr80iMGfYJHVjuizNQDzx3GcLeX5GfshLYYL5SHnuXg" alt="AutoPi.io - FCC Certified" data-size="line"></p></td></tr></tbody></table>

#### Licenses & Bonding&#x20;

Licenses are NFTs that can only be minted or transferred by DIMO Integrations. These certify the integration provider meets all required qualifications required and has been whitelisted for the production of compatible devices. After receiving a license, the integration provider is required to submit a deposit of $DIMO tokens (the “bond”). For more on how this works, see [License](https://app.gitbook.com/s/fmY0p4toAb7e89toAV2R/identity-protocol/nodes-and-nfts/license "mention").

Periodically, or with a significant change in price of $DIMO, the amount required to bond will rebase automatically. Every year on January 1st, the bond amount automatically adjusts to whatever the amount of $DIMO is that is equivalent to $10,000 USD. Rebasing can also happen within the year, whenever the 7 day token weighted average price (TWAP) of $DIMO changes by 50% or more relative to the price last used to calculate the deposit amount. For example, if $DIMO is worth $2.00 on January 1st, the bond requirement is 5,000 $DIMO. If the price of $DIMO increases to $2.80, there is no change in the deposit amount. Once the token weighted average price over 7 days increases to $3.00, then the bond requirement is rebased to 3,333 $DIMO.

If the bond amount is ever decreased, existing license holders have the option to withdraw the excess amount by notifying the DIMO Foundation of their desire to do so. If the bond amount ever increases, the license holder is grandfathered in and not obligated to add additional $DIMO.

This DIP may be updated without passing an amendment to update the bond amount below per the rules described herein.

**As of the last rebasing on July 5, 2024, the bond amount is 77,101 $DIMO.**

Past bond amounts were:

* December 12, 2022: 100,000 $DIMO

![](<../.gitbook/assets/image (6).png>)

While it is preferred that the integration provider is the party putting up the bond, it is also possible for a financing partner, such as a distributor, to put up the bond on behalf of the manufacturer.&#x20;

Should applicants not have $DIMO or not want to interact with tokens, they may purchase $DIMO from the Foundation and/or have the Foundation put up the bond on their behalf.

#### Slashing & License Revocation&#x20;

Through a governance vote, DIMO token holders have the ability alter the manufacturer’s bonding requirements. Manufacturers must be given thirty days to adjust their bond to the new level.

Token holders are also able to ban devices from the network (e.g., if they’re not secure and provide false data) and/or suspend or revoke a manufacturer’s license through a valid governance vote if they violate the obligations specified above or there is demonstrable and material negligence or malice perpetrated by the manufacturer that harms users or the DIMO protocol generally.

Any manufacturer may renounce their license and receive back their bonded $DIMO after six months.

### Connecting a Device to DIMO&#x20;

#### Device Payment Requirements&#x20;

For physical hardware, licensed manufacturers pay 4,000 DIMO Credits (DCX) to mint a device and enable it to connect to the DIMO network.

<figure><img src="../.gitbook/assets/image (1) (1) (2).png" alt=""><figcaption></figcaption></figure>

## Implementation&#x20;

If passed, the DIMO Foundation will issue licenses per valid governance votes.

## Copyright&#x20;

Copyright and related rights waived via CC0

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-4: Device Integration", no. 4, December 2022. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Dec 7, 2022: added discussion forum and voting type to the DIP header.

Dec 7, 2022: adjusted review date to give people more time to claim the Airdrop prior to voting going live.

Dec 26, 2023: adjusted review date again to allow for fixes to delegation strategy prior to voting.

Dec 30: combined Micro and Standard Dongle to one category ("Dongle") and decreased minting price on all device categories.

Jan 6, 2023: final adjustment to review date — proposals go to vote on Tuesday Jan 10.

Jan 6, 2023: simplified the language on buying tokens from the DIMO Foundation and removed the preset exchange rate. Refer to [dip6.md](dip6.md "mention") for more on exchanging tokens with the Foundation.

Jan 6, 2023: updated the language surrounding revoking a hardware manufacturer's license to include cause.

Jan 9, 2023: made device minting cost 25 $DIMO for all device types for now

Mar 29, 2023: passed [DIP-4 & 5: Amendment 1](../amendments/dip4-and-5a1.md)

July 6, 2024: disclaimer adjusted, updated for DLPs, and updated per [DIP-4 & 5: Amendment 2](../amendments/dip4-5a2.md)

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
