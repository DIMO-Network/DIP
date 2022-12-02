# DIP-4: Device Integrations

> **Headline**: Expanding the ecosystem of DIMO compatible hardware devices and software connection methods
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

This proposal outlines the method by which a new committee, called DIMO Integrations, will issue licenses to hardware manufacturers (like [AutoPi](https://www.autopi.io/)) who can produce compatible devices, as well as software developers (like [SmartCar](https://smartcar.com/)) who build digital integrations (collectively referred to as integration providers).

The requirements for any integration providers are that they must:&#x20;

1. Submit an application providing background on their business and receive approval from DIMO Integrations;
2. Stake 100,000 $DIMO tokens as a security deposit;&#x20;
3. Submit specifications and other details for each device or software integration service for approval from DIMO Integrations;
4. Pair the applicable “device minting” NFT with each vehicle they connect to; and
5. Remain in good standing with the community.&#x20;

## Motivation&#x20;

As a part of the vision to establish DIMO as a decentralized universal protocol, it is important to develop a robust and diverse ecosystem of manufacturers producing DIMO compatible hardware and software companies providing digital integrations.

The goals of this proposal are to:&#x20;

* Onboard and retain hardware providers (OEMs), software integrations, retailers, distributors, and support channels that are tightly aligned with the interests of the DIMO protocol and its users;&#x20;
* Accelerate the development and integration of new device types and integration methods such as dash cameras, micro dongles, embedded hardware, and more;&#x20;
* Establish standard device management software and APIs; and&#x20;
* Optimize the operations and financing of device production, fulfillment, and installation.

## Specifications&#x20;

### Establishing the DIMO Integrations Team&#x20;

If passed, this proposal would formally recognize the DIMO Integrations team and delegate certain rights and duties to it.

#### Purpose

DIMO Integrations is a delegate of the greater DIMO community responsible for ensuring the realization of the goals listed in the previous section. Primarily, this team is tasked with:&#x20;

* Recruiting, evaluating, and accepting new hardware manufacturers and software integration providers;&#x20;
* Monitoring existing connectivity enablers and, when necessary, challenging their stake and/or license (although this is not an exclusive right as any community member may also raise a challenge);&#x20;
* Researching, developing, and implementing new device types and specifications; and&#x20;
* Developing and publishing open source device management software.&#x20;

#### Team Composition & Operating Structure&#x20;

The initial team lead is [Brien East ](https://www.linkedin.com/in/brien-east-1137516b/details/experience/)(Digital Infrastructure Inc.) who will be responsible for assembling other contributors and prepare a [Resource Allocation DIP](templates/resource-allocation-template.md) and community presentation within 90 days. This team should be composed of trusted mechanical engineers, software developers, supply chain experts, game theorists, finance professionals, and attorneys.

#### Conflicts

In order to mitigate conflicts of interest, team members agree to reject any form of compensation from current or potential device manufacturers, except as otherwise defined in this proposal.&#x20;

#### Operating Goals & Metrics&#x20;

DIMO Integrations is explicitly targeting and tracking the following minimum operating goals and metrics.

Goals (target completion by the end of 2023):&#x20;

* Publish an open source firmware and software for device management;&#x20;
* Onboard five distinct device manufacturers;&#x20;
* Facilitate staking and the long-term alignment of all integration providers; and&#x20;
* Approve the production of at least five devices spanning at least two different device types.

Metrics:&#x20;

* Track and publish a current list of licensed integration providers in good standing; and
* Track and publish devices connected and disconnected by manufacturer and by device type per month, every month.

#### Authority & Domain&#x20;

As a part of the plan to progressively decentralize the project, DIMO Integrations will start with concentrated responsibilities and authorities, which will be decentralized over time.

DIMO Integrations will have the authority to grant and revoke licenses to integration providers and their devices/software services. However, they cannot lower the requirements that all manufacturers must stake a minimum 100,000 $DIMO as a security deposit and must use a “device minting” NFT for each device sold.

DIMO Integrations will serve as administrators in a device management software open source repository on Github. However, manufacturers are not required to use this software, and it will be published with an MIT open source license so that it may be forked.

The $DIMO token holders may overrule DIMO Integrations, may amend the powers and responsibilities this team possesses, and/or may extend these powers and responsibilities to other teams with any valid governance vote.&#x20;

#### Budget & Financial Projections&#x20;

DIMO Integrations is seeking an initial infusion of 150,000 $DAI and 50,000 $DIMO. These resources would go to a Gnosis Safe multi-signature wallet on the Polygon PoS chain requiring the signatures of \_\_ out of the \_\_ voting members. The address for that wallet is: \[0x… insert address here].

A larger and more detailed budget will be requested as part of the upcoming [Resource Allocation DIP](templates/resource-allocation-template.md) and community presentation that will&#x20;

Additionally, DIMO Integrations will earn $DIMO per connected vehicle which will be split among various members (see [Device Minting NFTs](dip-4-device-integrations.md#device-minting-nfts)).

#### Summary of Commitments&#x20;

DIMO Integrations commits to:&#x20;

* Publish the analysis and outcome from every license application and revocation;&#x20;
* Alert the community, particularly affected users, and provide a post-mortem if there is ever a major issue concerning a licensed integration provider and/or any of their devices;&#x20;
* Publish metrics as defined in the [Operating Goals & Metrics](dip-4-device-integrations.md#operating-goals-and-metrics) section;&#x20;
* Refuse any form of compensation from current or potential integration provider as to avoid any conflict of interest, except as otherwise defined above; and&#x20;
* Always act in good faith and in the best interest of the DIMO community.

### Integration Providers & Device Licenses

In order to connect to DIMO users, their vehicles, and their data, integration providers must agree to various obligations, apply for a license, submit specifications or code for a specific connection method, receive acceptance from DIMO Integrations, stake 100,000 $DIMO, and attach a “device minting” NFT to each device they sell or user they connect.

#### Obligations

Integration providers commit to maintaining strict quality and security standards, provide support for their services, abide to always act in good faith, and agree not to engage in unlawful activities. The following is illustrative but not exhaustive.

Connection methods must not:&#x20;

* Interfere with the users safe operation of their vehicle;&#x20;
* Damage the vehicle it is installed in;&#x20;
* Deliberately or negligently generate false data.&#x20;

Connection methods must:&#x20;

* Comply with all local regulations;&#x20;
* Receive adequate support from the provider for a reasonable duration of time;&#x20;
* Perform as expected;&#x20;
* Only share data with recipients that the user has opted into sharing with per the parameters of the DIMO protocol; and&#x20;
* If a physical device, be delivered to customers in a reasonable timeframe and fashion.&#x20;

#### Application&#x20;

Prospective integration providers must submit an application providing details about their business, their operating history, as well as specifications for the initial devices they intend to manufacture and/or software services they intend to provide. The initial application must contain specifications for at least one device design, test units, and data samples and/or a code repository and a functioning demo.

Licensed providers are able to submit additional and simplified applications for new devices and software methods at any time.

DIMO Integrations will design and launch the application materials and publish documentation outlining the application process within 60 days following the passing of the DIP #3.&#x20;

Integration Types&#x20;

New device types may be added at any time by DIMO Integrations. The initial device categories include.

| Device Type     | Concept Image                                                                                                                                                                                                                | Description                                                                                               | Typical Price Point                                                                    |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Software Only   | N/A                                                                                                                                                                                                                          | Leverages existing vehicle subscription programs and their APIs to establish a baseline of connectivity   | No added charge. Vehicle manufacturer (e.g., Ford, BMW) may charge a subscription fee. |
| Standard Dongle | <img src="https://lh4.googleusercontent.com/GRTqY_WLRyeZOLP1pVBYfSYdGVUWt1PkoETQV6RMpp9dv9J6eBachCMRinU0xTLmllv5FqrXc8HwsaIHoxTS3Iu6sz7MmxaB9SELzz2A5lGaXZ7vTFR0DIGKLzBK31NezvVeTh506XH9k-kG6dP8eg" alt="" data-size="line"> | Records vehicle data from the CAN bus, stand-alone connectivity                                           | $350                                                                                   |
| Hub             | <img src="https://lh6.googleusercontent.com/cW34tdb4DmfURDEFbWxoxj5ERDEnqZHH2dsUASFow2t-xKnmK1hxqO3rW6PCSvZ6mR5BsoYcbaQk-rJqlDaouSZsjcpehE2iIDjkt0s5syt9VMT1XL0XRlT0qh00mwwVSA-h9io-mOh4EX9Al6Ldpg" alt="" data-size="line"> | IoT hub that enables long term local storage and backup of data, as well as cheaper dongle and dash cams. | $500                                                                                   |
| Dash Camera     | <img src="https://lh6.googleusercontent.com/iHX9U2U_0JmIAT9N6wWHBLrbaeBgSmAe0BOQl-AidpMPL6sYyUN0-L4glSSDJpbtae7zMV4lDKNqsE1Sno6nt5kvvr1Vq-8Q_XDzT9C-HIh_ySkiKT7ZFjpLnMMohFqSotMraAwn1VgRehEiAHRpYQ" alt="" data-size="line"> | Device that records camera footage and possibly other telemetry                                           | $500                                                                                   |
| Fleet Device    | <img src="https://lh4.googleusercontent.com/5GZ6wu9JU1rmER4U0qvBEsCdZ4EyCfSwlHNuy7ap1eN807pdaKGttS2RSnNF2Ic0mr73AMnbxgKYiq124gEkfOCQUqwRGDBx66_CajHhfXEXjfBBb9hsb5Leg4OZ5ewSK2uKH_gzjt-RGhyPXECMpg" alt="" data-size="line"> | Telemetry devices designed for commercial use                                                             | $1,000                                                                                 |
| AI Device       | <img src="https://lh6.googleusercontent.com/wKACXQZGzx-nPAWv3ks_rD0yr36c4W9k470JyfYbijs6RbY6crv0XLXKJ9jET5Eg0nvS_wzsRYtSnQKFpbiLI0c6w8jnl9YUmbVEISXcn3E0nP6LIEwWY1lEUZMVztYiHiCxvpQqY6IUx_kLtu1ECw" alt="" data-size="line"> | Device that supplements enhanced driving features (e.g., Comma AI)                                        | $2,000                                                                                 |

#### Connection Specifications&#x20;

The following are minimum device specifications as set by the DIMO Community in this DIP, which may only be amended by a future DIP. Except for the ways specified in the table below, DIMO Integrations may not alter these requirements, but it may add additional specifications that go above and beyond, particularly for certain device types (e.g., dash cams may have additional specifications related to privacy and compression).

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

Licenses are NFTs that can only be minted or transferred by DIMO Integrations. These certify the integration provider meets all required qualifications required and has been whitelisted for the production of compatible devices. After receiving a license, the integration provider is required to submit a deposit of 100,000 $DIMO tokens (the “stake”). **The DIMO protocol will check both the NFT license and the on-chain stake balance to determine if a provider is licensed or not.**

![](<.gitbook/assets/image (6).png>)

While it is preferred that the integration provider is the party putting up the stake, it is also possible for a financing partner, such as a distributor, to put up the stake on behalf of the manufacturer.&#x20;

#### Slashing & License Revocation&#x20;

If an integration provider violates their obligations as specified above, some or all of their stake may be forfeit (“slashed”) and their license may be suspended or revoked. Any $DIMO holder may issue a challenge per the DIMO arbitration procedure (see DIP-2 \[insert link]). If the DIMO Court, the name for DIMO’s arbitration council, sides in the favor of the challenger, all or some of the stake may be burned and/or given to affected users.

While DIMO Integrations, is both able to and expected to act as the challenger most of the time, they do not have the authority to unilaterally slash the manufacturers stake. That power lies with the DIMO Court.

They do, however, have unilateral ability to ban devices from the network (e.g., if they’re not secure and provide false data), suspend or revoke a manufacturer’s license at any time, or increase the manufacturer’s staking requirement above the minimum 100,000 $DIMO.

Any manufacturer may renounce their license and receive back their staked $DIMO after six months if there are no successful challenges during that time frame.



### Connecting a Device to DIMO&#x20;

#### Device Minting NFTs&#x20;

For physical devices, in addition to proper licensing as defined in the previous section, the EVM wallet contained within the secure element must hold a “device minting” NFT. These are special NFTs that require $DIMO to acquire initially, but which may then be sold and transferred (e.g., on OpenSea) until the moment they are bonded to a licensed device.

![](<.gitbook/assets/image (11).png>)

All device sales must include a device minting NFT; end users should not be required to source one themselves. For those familiar, these are similar in concept to mint vials (e.g., [CloneX Mintvial](https://opensea.io/collection/clonex-mintvial?utm\_governance=OPNS9ci96jyifptpsdwen90e\&utm\_source=google\&utm\_medium=paid\&utm\_account=6961136327\&utm\_term=clonex%20mint%20vial\&utm\_matchtype=e\&utm\_campaignid=17563298525\&utm\_adgroupid=140912765951\&utm\_keywordid=kwd-1657036550808\&wpsrc=Google%20AdWords\&wpcid=17563298525\&wpsnetn=g\&wpkwn=clonex%20mint%20vial\&wpkmatch=e\&wpcrid=605564529802\&wpscid=140912765951\&wpkwid=kwd-1657036550808\&gclid=CjwKCAjw5s6WBhA4EiwACGncZRqKQE2ZTbSRYCiwnk9kzrUy4emwMiAbry2KeLOAnYSIMoYNq0pXxRoCekYQAvD\_BwE)).

![](<.gitbook/assets/image (10).png>)

Similarly, for software connection methods that don’t yet make use of an EVM wallet to sign data, a device minting NFT must be sent to the vehicle NFT address as a part of the pairing process. Therefore, unlike a hardware device that may be moved from vehicle to vehicle without needing a second device minting NFT, every new software connection will require another device minting NFT.

![](<.gitbook/assets/image (1).png>)

Why add this complexity? To align the incentives of various stakeholders, the $DIMO that is used to acquire the NFT is set aside. Each month that the connection persists, the integration provider receives some of that $DIMO back as rebate for twenty four months until they earn back 70% of the deposit. Additionally, DIMO Integrations receives $DIMO over the same period until they earn 0.1% - 15% of the deposit. See [Rewards Calculation for DIMO Integrations Team](dip-4-device-integrations.md#rewards-calculation-for-dimo-integrations-team) for more information on this calculation.

This rebate mechanism ensures that integration providers and DIMO Integrations are long-term holders of $DIMO and that they have an incentive to produce resilient devices and services that users will love and want to keep connected.

The remaining $DIMO will go directly to the DIMO Treasury, as will royalties from the secondary trading of the device minting NFTs. Secondary trading will also generate valuable price discovery information.

![](<.gitbook/assets/image (7).png>)

Device NFTs provide a fair way for the DIMO community to control the supply of each type of connected device so as not to overwhelm the protocol too early. While it is fair to say that users who have already established a connection may have an incentive to artificially constrain the number of device minting NFTs so there is less competition on the network for baseline rewards, they have a more powerful long-term incentive to grow the network and its adoption.

#### Quantity and Cost of Device Minting NFTs&#x20;

The availability and amount of DIMO required for a device minting NFT varies by device type. Quantities may (and will) be increased by a future vote of $DIMO holders. It’s likely that constraints will be lifted altogether and any licensed integrations provider will be able to mint as many as needed, when needed.

| Type            | Description                                                                                               | Initial Quantity | Cost (in $DIMO) |
| --------------- | --------------------------------------------------------------------------------------------------------- | ---------------- | --------------- |
| Software Only   | Leverages existing vehicle subscription programs and their APIs to establish a baseline of connectivity   | 1,000,000        | 10              |
| Standard Dongle | Records vehicle data from the CAN bus, stand-alone connectivity                                           | 100,000          | 50              |
| Hub             | IoT hub that enables long term local storage and backup of data, as well as cheaper dongle and dash cams. | 30,000           | 70              |
| Dash Camera     | Device that records camera footage and possibly other telemetry                                           | 30,000           | 80              |
| Fleet Device    | Telemetry devices designed for commercial use                                                             | 100,000          | 120             |
| AI Device       | Device that supplements enhanced driving features (e.g., Comma AI)                                        | 30,000           | 150             |

Similar to the stake required for licensing, device minting NFTs may be provided by financing partners, such as a distributor.&#x20;

#### Rewards Calculation for DIMO Integrations Team

The reward to DIMO Integrations is calculated using a reverse bonding curve that decreases the proportional reward over time. The curve is established for each device type. This is done in order to incentivize the team to do the difficult work of establishing new device categories and getting them to critical mass.

![](<.gitbook/assets/image (4).png>)

The formula to determine the % reward of the staked $DIMO from Device Minting NFTs that DIMO Integrations is eligible to receive as a reward is calculated as:

> _<mark style="color:blue;">Reward for a single NFT if connected for two years = Price of NFT \* maximum of ( 0.1% OR 15% \* (99.9999% ^ (# of that NFT type sold - 1)))</mark>_

![](https://lh3.googleusercontent.com/eH4Vxl2ckdKGTP03fJRNVf-X4tdfggL9MjQbUhL9Rdq3zNafL-02G\_Kyn0oxHxaDsIWhTSl8HQAm3CbfqPjw3EAs9T9NRzV73GYdC\_T6gWHixBLxo-pxoAxBN5dU5rkp9Eo-1ektI2AVIsqwNRS8rY4)

#### Pairing & Connectivity

As described in [Connection Specifications](dip-4-device-integrations.md#connection-specifications), DIMO Integrations will provide a specification for formatting and sending data to the protocol and establishing a data stream.

Additionally, Digital Infrastructure Inc will open-source the pairing code for the Gen 1 DIMO Data Miner and mobile application, which can be used as a spec for any future pairing process using a standard bluetooth interface.

Digital Infrastructure Inc. has also been approved to negotiate global rates for cellular connectivity, and have selected Twilio as the initial connectivity provider, an ISO27001 Certified and GDPR-compliant MVNO. Approved OEMs will be given access to acquire SIMs and bind connectivity agreements at the bulk purchase price and can pass costs along to their customers through purchase and subscription agreements.

Rates will be consistent throughout 2022, and connectivity will be re-auctioned in 2023.

These rates can be applied to any approved device, and manufacturers can choose to go with their own connectivity provider if they choose, although additional integration work may be required to achieve Proof of Movement Certification.&#x20;

## Implementation&#x20;

If passed, this DIP-3 will be in effect immediately after the four day time lock concludes. The newly formed DIMO Integration Committee will be responsible for the implementation of the programs and procedures introduced in this document.

## Copyright&#x20;

Copyright and related rights waived via CC0

## Citation&#x20;

Please cite this document as:

Andy Chatham, Rob Solomon, Diego Moro, "DIP-3: Device Integrations", no. 3, May 2022. \[Online serial]. Available: \[https://github.com/DIMO-Network/DIP]
