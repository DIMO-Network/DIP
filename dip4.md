# DIP-4: Device Integrations

> **Headline**: Expanding the ecosystem of DIMO compatible hardware devices and software connection methods
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review (until January 5th, 2022 at 5:00 UTC)
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: Level 3

## Abstract

This proposal outlines the method by which hardware manufacturers (like [AutoPi](https://www.autopi.io/)) who produce compatible devices, as well as software developers (like [SmartCar](https://smartcar.com/)) who build digital integrations (collectively referred to as integration providers) stake $DIMO and receive a license.

The requirements for any integration providers are that they must:&#x20;

1. Pass a DIP that approves their license application;
2. Stake 100,000 $DIMO tokens as a security deposit;&#x20;
3. Transfer the applicable amount of $DIMO for each integrations they enable; and
4. Remain in good standing with the community.&#x20;

## Motivation&#x20;

As a part of the vision to establish DIMO as a decentralized universal protocol, it is important to develop a robust and diverse ecosystem of manufacturers producing DIMO compatible hardware and software companies providing digital integrations.

The goals of this proposal are to:&#x20;

* Onboard and retain hardware providers (OEMs), software integrations, retailers, distributors, and support channels that are tightly aligned with the interests of the DIMO protocol and its users;&#x20;
* Accelerate the development and integration of new device types and integration methods such as dash cameras, cheaper dongles, embedded hardware, and more; and&#x20;
* Optimize the operations and financing of device production, fulfillment, and installation.

## Specifications&#x20;

### Integration Providers & Device Licenses

In order to connect to DIMO users, their vehicles, and their data, integration providers must agree to various obligations, receive a license by passing a DIP, stake 100,000 $DIMO, and deposit $DIMO for each device they sell.

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

Prospective integration providers may receive a license by passing a DIP using the [License Approval Template](templates/license-approval-template.md). The application must provide details about their business, their operating history, as well as specifications for the initial devices they intend to manufacture and/or software services they intend to provide.&#x20;

The DIP must contain specifications for at least one device design, test units, and data samples and/or a code repository and a functioning demo. Licensed providers are able to submit additional and simplified applications for new devices and software methods at any time.

_Integration Types_&#x20;

All integrations methods must be categorized as one of the following device types. New device types may be added by token holders with a valid governance vote.

| Device Type   | Concept Image                                                                                                                                                                                                                | Description                                                                                             | Typical Price Point                                                                    |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Software Only | N/A                                                                                                                                                                                                                          | Leverages existing vehicle subscription programs and their APIs to establish a baseline of connectivity | No added charge. Vehicle manufacturer (e.g., Ford, BMW) may charge a subscription fee. |
| Dongle        | <img src="https://lh4.googleusercontent.com/GRTqY_WLRyeZOLP1pVBYfSYdGVUWt1PkoETQV6RMpp9dv9J6eBachCMRinU0xTLmllv5FqrXc8HwsaIHoxTS3Iu6sz7MmxaB9SELzz2A5lGaXZ7vTFR0DIGKLzBK31NezvVeTh506XH9k-kG6dP8eg" alt="" data-size="line"> | Records vehicle data from the CAN bus.                                                                  | $350                                                                                   |
| Hub           | <img src="https://lh6.googleusercontent.com/cW34tdb4DmfURDEFbWxoxj5ERDEnqZHH2dsUASFow2t-xKnmK1hxqO3rW6PCSvZ6mR5BsoYcbaQk-rJqlDaouSZsjcpehE2iIDjkt0s5syt9VMT1XL0XRlT0qh00mwwVSA-h9io-mOh4EX9Al6Ldpg" alt="" data-size="line"> | IoT hub that enables long term local storage and backup of data.                                        | $500                                                                                   |
| Dash Camera   | <img src="https://lh6.googleusercontent.com/iHX9U2U_0JmIAT9N6wWHBLrbaeBgSmAe0BOQl-AidpMPL6sYyUN0-L4glSSDJpbtae7zMV4lDKNqsE1Sno6nt5kvvr1Vq-8Q_XDzT9C-HIh_ySkiKT7ZFjpLnMMohFqSotMraAwn1VgRehEiAHRpYQ" alt="" data-size="line"> | Device that records camera footage and possibly other telemetry                                         | $500                                                                                   |
| Fleet Device  | <img src="https://lh4.googleusercontent.com/5GZ6wu9JU1rmER4U0qvBEsCdZ4EyCfSwlHNuy7ap1eN807pdaKGttS2RSnNF2Ic0mr73AMnbxgKYiq124gEkfOCQUqwRGDBx66_CajHhfXEXjfBBb9hsb5Leg4OZ5ewSK2uKH_gzjt-RGhyPXECMpg" alt="" data-size="line"> | Telemetry devices designed for commercial use                                                           | $1,000                                                                                 |
| AI Device     | <img src="https://lh6.googleusercontent.com/wKACXQZGzx-nPAWv3ks_rD0yr36c4W9k470JyfYbijs6RbY6crv0XLXKJ9jET5Eg0nvS_wzsRYtSnQKFpbiLI0c6w8jnl9YUmbVEISXcn3E0nP6LIEwWY1lEUZMVztYiHiCxvpQqY6IUx_kLtu1ECw" alt="" data-size="line"> | Device that supplements enhanced driving features (e.g., Comma AI)                                      | $2,000                                                                                 |

#### Connection Specifications&#x20;

The following are minimum device specifications.

Both Hardware & Software

| Certification       | Description                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Power management    | DIMO compatible devices must implement power management to prevent phantom drain of the vehicles it connects to, and efficiently manage being in “sleep” mode.                                                                                                       |
| Secure runtime      | Security is of highest importance to DIMO for both safety and security of the users. To provide an additional layer of safety to the car and the user, DIMO devices must run signed and verified code. Hardware must use secure boot mechanisms.                     |
| Streaming interface | DIMO Integrations will provide a specification for how the data should be formatted (schema) and sent to the protocol (delivery). Initially, the data will be sent in compressed json, moving to more efficient binary methods of encoding such as protobuf or avro. |
| Approved geography  | Currently, devices may only operate within the United States of America, Canada, and Europe. Support for new regions may be added by the DIMO community in future DIPs.                                                                                              |

Hardware Only&#x20;

| Certification                        | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Hardware secure element & EVM wallet | The identity of the device and the vehicle it is connected to is of high importance. In web3, this is known as a “wallet”, but is essentially a private key to identify the device. To limit spoofing, DIMO requires the private keys to be stored inside a hardware secure element. This key is also used for encrypted, secure transmission of vehicle data. Each device should contain its own EVM compatible wallet.                                                                                                                                                                                                                                                                                                                                          |
| DBC logger configuration             | Each vehicle is different and provides different signals on the canbus. To handle this variety of messages, DIMO maintains an open repository \[OPENDBC]. To be compatible with DIMO, the device must accept dynamic configuration of signals for filtering, parsing, and delivery to the protocol.                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| OTA process                          | To be accepted into the program, the device manufacturer must routinely support and update their devices as new vulnerabilities are found. This must be able to be done via cellular connection.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 3rd party certifications             | <p>CE Certifications EN 301 489-1 v2.2.0 EN55025:2008 EN 50498 and Directive 2004/104/EC ISO 7637-2:2011 EN 301 489-3 V2.1.1 <img src="https://lh4.googleusercontent.com/E_LfSnGkea7mAmpWINsnajyDt8F4sbSyGW3AYIMMidRF92y6GiV_nJ8tgZMILXp3A4V4IQbAcg3d_6DEhFTHYbb3Aggjnv2STFXto4MhDgPs9SnVVK0n1d1vkJD8mJCkZ5SrLzSYLGR1TSw_XbHjJg" alt="AutoPi.io - CE Certified" data-size="line"></p><p>FCC Certifications Devices certified under the following standards: FCC 47 CFR Part 15, Class A:10–1–17 Edition <img src="https://lh6.googleusercontent.com/OX11obGi-bwDcoF0vgnN1-imk7w_9o6-G9c624gYqDSeOj29p4oxy-8ByicOyEgLGfnP9sXxuOXGEg2HsjE_jwNUt7IEc317ai13cr0bllaOr80iMGfYJHVjuizNQDzx3GcLeX5GfshLYYL5SHnuXg" alt="AutoPi.io - FCC Certified" data-size="line"></p> |

#### Licenses & Staking&#x20;

Licenses are NFTs that can only be minted or transferred by DIMO Integrations. These certify the integration provider meets all required qualifications required and has been whitelisted for the production of compatible devices. After receiving a license, the integration provider is required to submit a deposit of 100,000 $DIMO tokens (the “stake”). For more on how this works, see [License NFT](https://app.gitbook.com/s/fmY0p4toAb7e89toAV2R/protocol/license-nft "mention").

![](<.gitbook/assets/image (6).png>)

While it is preferred that the integration provider is the party putting up the stake, it is also possible for a financing partner, such as a distributor, to put up the stake on behalf of the manufacturer.&#x20;

Should applicants not have $DIMO or not want to interact with tokens, they may purchase $DIMO from the Foundation and/or have the Foundation put up the stake on their behalf. The price of $DIMO should be 1 USD equivalent paid in a popular fiat currency (e.g., USD, EUR, GBP), ETH, BTC, or DAI.

The staking amount, as well as the exchange rate for $DIMO offered by the Foundation, may be altered by any future governance vote.

#### Slashing & License Revocation&#x20;

If an integration provider violates their obligations as specified above, their license may be suspended or revoked. Any manufacturer may renounce their license and receive back their staked $DIMO after six months.

Through a governance vote, DIMO token holders have the ability to ban devices from the network (e.g., if they’re not secure and provide false data), suspend or revoke a manufacturer’s license at any time, or increase the manufacturer’s staking requirement above the minimum 100,000 $DIMO.

### Connecting a Device to DIMO&#x20;

#### Device Payment Requirements&#x20;

For physical hardware, licensed manufacturers pay a set amount of $DIMO to mint a device and enable it to connect to the $DIMO network.

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

The $DIMO payment is set aside. Each month that the connection persists, the integration provider receives some of that $DIMO back as rebate for twenty four months until they earn back 70%.&#x20;

Why add this complexity? It's to align incentives.

This rebate mechanism ensures that both integration providers and DIMO Integrations are long-term holders of $DIMO and that they have an incentive to produce resilient devices and services that users will love and want to keep connected.

The DIMO Treasury keeps any $DIMO that isn't returned to the manufacturer.

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

#### Cost of Device Minting

The amount of DIMO required for device minting varies by device type.

| Type          | Description                                                                                             | Cost (in $DIMO) |
| ------------- | ------------------------------------------------------------------------------------------------------- | --------------- |
| Software Only | Leverages existing vehicle subscription programs and their APIs to establish a baseline of connectivity | 0               |
| Dongle        | Records vehicle data from the CAN bus, stand-alone connectivity                                         | 25              |
| Hub           | IoT hub that enables long term local storage and backup of data.                                        | 50              |
| Dash Camera   | Device that records camera footage and possibly other telemetry                                         | 50              |
| Fleet Device  | Telemetry devices designed for commercial use                                                           | 75              |
| AI Device     | Device that supplements enhanced driving features (e.g., Comma AI)                                      | 75              |

Similar to the stake required for licensing, device minting costs may be covered by financing partners, such as a distributor.&#x20;

### Temporary Licenses

For six months after the passage of this DIP, the following companies are have a temporary license. Following six months, they will need to apply for a permanent license per the process defined above.

* [AutoPi Aps](https://www.autopi.io/) is licensed to produce it's [DIMO x AutoPi Data Miner](https://shop.dimo.zone/products/dimo-data-device?title=default%2520title)
* [Smartcar](https://smartcar.com/) is licensed to offer a software connection
* Digital Infrastructure Inc is licensed to offer a software connection.

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

Dec 26: adjusted review data again to allow for fixes to delegation strategy prior to voting.

Dec 30: combined Micro and Standard Dongle to one category ("Dongle") and decreased minting price on all device categories.

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
