# DIP-5: App Ecosystem

> **Headline**: How app developers get licensed to access user data.
>
> **Author**: The DIMO Foundation
>
> **Submitter**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Draft
>
> **Discord forum URL**: Pending
>
> **Voting URL**: Pending

## Abstract

This proposal defines how clients, nodes, and applications will form, remain in good standing, and interact with DIMO users, their data, and the protocol itself.

The DIMO app ecosystem has five main components:&#x20;

* **Users**: connect their vehicles, generate data, use apps, and spend/earn $DIMO;&#x20;
* **Clients**: provide interfaces for DIMO users to interact with the protocol (e.g., DIMO Mobile on iOS and Android);&#x20;
* **Node** **operators**: receive IoT device data from users and serve it to licensed apps and data customers (node operators are to DIMO what Infura or Alchemy are to Ethereum);&#x20;
* **Apps**: build products that pay node operators for DIMO user data and connectivity; and&#x20;
* **DIMO** **Platform** **Licensing**: issues licenses to clients, node operators, and apps. It also operates DIMO Pay, a payment processing and currency conversion service that apps and node operators and apps are required to use.

![](https://lh6.googleusercontent.com/K46ZpsUjd-RwMxBsR8ajNlB76HxJKPI169z5z0HcuZt09GOW-SqRnIsUHwcGK1MldM4Td0mlZI5rlVj2Ye-K4OkgVRaF1rAP0maWNjGyJEswfIOB\_Q94pet2kt-hpNhpnRUDOb8DTA3YX0spUIM)

## **Motivation**

DIMO applications are a link between data consumers and data providers. It is imperative to define how they will be created, how they will function, and the incentives that will guide their actions.

The goal of this proposal is to put in place a framework that can safely and effectively grow the number of:&#x20;

* DIMO users who will share their data, protect their privacy, and earn rewards;&#x20;
* App developers who build applications that make use of user data and connectivity; and&#x20;
* Service Providers who use apps to help users solve problems.&#x20;

## Specifications&#x20;

### Establishing the DIMO Platform Licensing Team

DIMO Platform Licensing is a group of contributors, appointed by $DIMO token holders, whose goal is to maximize earnings, utility, and security for users.&#x20;

#### Purpose&#x20;

This team is tasked with:&#x20;

* Attracting, vetting, licensing, and onboarding data and connectivity clients, nodes, and applications;
* Monitoring and reporting on the effectiveness and compliance of licensed clients, nodes and applications;&#x20;
* Generally protecting DIMO Users privacy and security; and&#x20;
* Operating the DIMO Pay subscription engine and fee converter.&#x20;

#### Team Composition & Operating Structure&#x20;

Leadership:&#x20;

* TBD

Core Contributors&#x20;

* TBD

#### Conflicts of Interest

Other than specified in this proposal, the DIMO Platform Licensing team will refuse any form of compensation from any client, node operator, or application, or any of their close affiliates.

#### Operating Goals & Metrics

2023 Goals:&#x20;

* Onboard DIMO Mobile as the first licensed client;&#x20;
* Onboard DIMO Web Services as the first licensed node operator;&#x20;
* Onboard three distinct DIMO applications which collectively serve at least 100,000 users; and&#x20;
* Detect and remedy any misuse of data by clients, node operators, and applications.

Metrics:&#x20;

* Track and maintain a current list of licensed clients, nodes, and applications with pertinent information (e.g., business name, website, support email, etc.);&#x20;
* Track and publish the number of users of each DIMO client, every month; and&#x20;
* Track and publish the number of users opted-in to each node per month, every month.&#x20;

#### Authority & Domain&#x20;

DIMO Platform Licensing will have the authority to grant and revoke licenses to clients, nodes, and applications. However, they cannot lower the initial licensing requirements outlined. They also cannot grant a license to any node, or affiliate of such node, who is presently banned as a result of an arbitration proceeding (see the applicable Licensing & Revocation section for each group).

While it is expected that this team will be the first to pursue action against a node that breaches its responsibilities, any community member may initiate a challenge to slash their stake (see the applicable Licensing & Revocation section for each group).

The $DIMO token holders may overrule DIMO Platform Licensing, may amend the powers and responsibilities this team possesses, and/or may extend these powers and responsibilities to other teams with any valid governance vote.&#x20;

#### Budget & Financial Projections

DIMO Platform Licensing is seeking an initial infusion of \_\_ $DIMO tokens (when available) and \_\_ $USDC to fulfill its purpose and achieve its 2023 goals as specified above. These resources would go to a Gnosis Safe crypto wallet on the Polygon PoS chain requiring the signatures of \_\_ out of the \_\_ voting members. The address for that wallet is: 0x\_\_



| Description                                 | $DIMO Per Month | USDC Per Month |
| ------------------------------------------- | --------------- | -------------- |
| Allocations to various contributors         | TBD             | TBD            |
| Grants to clients, node operators, and apps | TBD             | TBD            |
| Travel & other misc                         | TBD             | TBD            |
| **Total**                                   | **TBD**         | **TBD**        |

Members of Digital Infrastructure Inc. and the DIMO Foundation will not receive any compensation for their contribution to the DIMO Platform Licensing team.&#x20;

#### Summary of Commitments&#x20;

DIMO Platform Licensing commits to:&#x20;

* Publish the analysis and outcome from every license application and revocation;&#x20;
* Alert the community, particularly affected users, and provide a post-mortem if there is ever a major issue concerning a licensed client, node, or application;&#x20;
* Publish metrics as defined in the [Operating Goals & Metrics](dip-5-app-ecosystem.md#operating-goals-and-metrics) section;
* Comply with the terms of the [Conflicts of Interest](dip-5-app-ecosystem.md#conflicts-of-interest) section; and
* Always act in good faith and in the best interest of the DIMO community.&#x20;



### Clients&#x20;

A client is a type of application that allows users to interact directly with the DIMO protocol. Typically, this will mean creating and managing their account, creating and managing their vehicle identity, adding and removing credentials in their identity glovebox (e.g., insurance and registration, adding and removing telemetry devices, and viewing back their own data. These are to DIMO what Apple Mail, Outlook, and Superhuman are to email. DIMO Mobile is an example of a client ([iOS](https://apps.apple.com/us/app/dimo-mobile/id1589486727) and [Android](https://play.google.com/store/apps/details?id=com.dimo.driver\&hl=en\_US\&gl=US) links).&#x20;

To operate a licensed client, administrators must:&#x20;

* Submit an application, and receive approval from, DIMO Platform Licensing; and
* Maintain compliance with the [Rights & Obligations](dip-5-app-ecosystem.md#rights-and-obligations).

#### Application

Any entity can apply to operate a client. The DIMO Platform Licensing team will provide resources to guide the applicant through the review process and will publish a summary of the application outcome to the DIMO community quarterly.

Applicants may find and submit the application form [here](https://gkmkni9caof.typeform.com/to/Tl3rglKv).&#x20;

#### Staking

Clients must stake 10,000 $DIMO tokens. This acts as a security deposit that can be slashed if the client publisher misbehaves.

#### Rights & Obligations

To the extent that a client stores user data off device, it must be encrypted in transit and at rest. Clients may not pass user data to any third party entity, other than licensed nodes and applications in a manner that is transparent to the user and necessary to function as a client.

When collecting opt-ins from users for sharing data with nodes and apps, clients must provide users with the following.

| Information           | Description                                                                                                                                  |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Name                  | The name (entity & DBA) of the node or app (e.g., Digital Infrastructure Inc. dba DIMO Explorer)                                             |
| User's identity data  | The user’s personal data being shared and the frequency it will be streamed (e.g., insurance, registration, achievements).                   |
| Vehicle telemetry     | The streams of data being shared and the frequency it will be streamed (e.g., tire pressure, speed, location, camara data, telemetry).       |
| Staking & Trust Ratio | <p>Amount staked by node or app and the trust ratio, which is calculated as: </p><p><em>Trust Ratio = $DIMO Staked / $DIMO Required</em></p> |

Clients must always comply with relevant privacy regulations (e.g., GDPR) and all core services must be open source.

#### Licensing & Revocation

Licenses are issued on-chain as NFTs.

The DIMO Platform Licensing team may ban clients from the network (e.g., if they misuse user data) or suspend or revoke their license at any time.&#x20;

#### Payments

All payments made between DIMO users, clients, nodes, and/or apps must be routed through DIMO Pay ([see DIP-5](broken-reference)).



### Nodes&#x20;

A node is an entity that receives data from DIMO users and makes it available to applications. These entities are responsible for forming and upholding agreements that protect user privacy and enable DIMO applications. Node operators are to DIMO what Infura or Alchemy are to Ethereum.

To operate a licensed node, administrators must:&#x20;

* Submit an application, and receive approval from, DIMO Platform Licensing;&#x20;
* Stake $DIMO tokens; and
* Maintain compliance with the [Rights & Obligations](dip-5-app-ecosystem.md#rights-and-obligations-1).&#x20;

#### Application&#x20;

Any entity can apply to be a node. The DIMO Platform Licensing team will provide resources to guide the applicant through the review process and will publish a summary of the application outcome to the DIMO community quarterly.

Applicants may find and submit the application form [here](https://gkmkni9caof.typeform.com/to/Tl3rglKv).&#x20;

#### Staking&#x20;

Node operators must stake 100,000 $DIMO tokens plus an additional 2 $DIMO per connected user. This achieves two purposes: 1) it acts as a security deposit that can be slashed if the operator misbehaves; and 2) it ensures that node operators have their incentives aligned with DIMO.

Nodes should stake additional tokens as a buffer to prevent DIMO smart contracts from blocking the onboarding of new users, and to increase alignment with their existing users.&#x20;

#### Rights & Obligations

All stored user data must be encrypted in transit and at rest, and nodes must never knowingly or negligently transmit false data. Both nodes and the businesses that they serve must always comply with relevant privacy regulations (e.g., GDPR).

Node operators may share anonymized data with third parties who have received an application license from the DIMO Platform team (e.g., battery analytics app combines 1,000’s of users’ data with other data like battery supply chain data and serves it to car manufacturers), without requiring an additional opt-in from the user. For data to be considered aggregated and anonymized, it must be compiled in such a way that the recipient cannot determine any personally identifiable and sensitive information. For example, anonymized location data cannot be shared for an isolated region where only 10 people live as the sample size is too low.

Non-anonymized and personally identifiable information may be shared with licensed apps (e.g., battery analytics app that provides a user better information and recommendations for EV battery health) only when a user opts-in to sharing their data with that third party. Opt-in requests must specify the data that will be shared and the purpose for sharing it. This can be ongoing or one-time data transfer, or require the user to go off platform to transact.

Node operators must always strive to maximize revenue to themselves and DIMO users. This does not mean they cannot offer a freemium type model to apps that utilize the node service, but it does mean that a node should not give away user data in exchange for personal favor or some other form of payment or incentive on the side that doesn’t ultimately benefit DIMO users.&#x20;

#### Licensing & Revocation&#x20;

Licenses are issued on-chain as NFTs. Data will only be shared to those who have an active license and only DIMO Platform Licensing may transfer these licenses. If a license lapses, or if a node fails to maintain the required stake, data will not continue to be shared and the license to use past data for commercial purposes will expire.

If a node neglects their obligations as specified above, some or all of their stake may be forfeit (“slashed”) and their license may be suspended or revoked. Any $DIMO holder may issue a challenge per the DIMO arbitration procedure (see [DIP-2](dip-6-dispute-resolution.md)). If the DIMO Court sides in the favor of the challenger, all or some of the stake may be burned and/or given to affected users.

The staked $DIMO will remain locked for as long as the application continues to function.

While the DIMO Platform Licensing team is both able to and expected to act as the challenger most often, they do not have the authority to unilaterally slash the node’s stake.

Additionally, the DIMO Platform Licensing team may ban nodes from the network (e.g., if they misuse user data), suspend or revoke their license at any time, or increase their staking requirement above the minimum 200,000 $DIMO.

Any application may renounce their license and receive back the staked $DIMO after six months if there are no challenges.

#### Payments

All payments made between DIMO users, clients, nodes, and/or apps must be routed through DIMO Pay ([see DIP-5](broken-reference)).



### Apps&#x20;

An app is an application or service that utilizes DIMO user data to provide functionality. Examples of applications that can be built with DIMO data and identity primitives include online car marketplaces, auto lending, smart insurance, ride hailing, car sharing, and more. Uber, Geico, eBay Motors, and Hertz could be rebuilt as leaner, cheaper, and more effective protocols on top of DIMO.&#x20;

To operate a licensed app, administrators must:&#x20;

* Submit an application, and receive approval from, DIMO Platform Licensing; and
* Maintain compliance with the [Rights & Obligations](dip-5-app-ecosystem.md#rights-and-obligations).

#### Application&#x20;

Any entity can apply to license an application. The DIMO Platform Licensing team will provide resources to guide the applicant through the review process and will publish a summary of the application outcome to the DIMO community quarterly.

Applicants may find and submit the application form [here](https://gkmkni9caof.typeform.com/to/Tl3rglKv).

#### Staking

Apps must stake 10,000 $DIMO tokens. This acts as a security deposit that can be slashed if the app publisher misbehaves.

#### Rights & Obligations

To the extent that an application stores user data, it must be encrypted in transit and at rest. Apps may not pass user data to any third party entity, other than licensed clients, nodes, and apps in a manner that is transparent to the user and necessary to its function as an application.

Apps must always comply with relevant privacy regulations (e.g., GDPR) and may not resell their data feed.

Key app categories have grants available through the DIMO foundation, and developers or enterprises can submit a proposal to the committee [here](https://docs.dimo.zone/dimo-overview/development-roadmap/seeding-applications).

#### Licensing & Revocation&#x20;

Licenses are issued on-chain as NFTs.

The DIMO Platform Licensing team may ban apps from the network (e.g., if they misuse user data) or suspend or revoke their license at any time.

#### Payments

All payments made between DIMO users, clients, nodes, and/or apps must be routed through DIMO Pay ([see DIP-5](broken-reference)).

## Implementation

If passed, this DIP-4 will be in effect immediately after the four day timelock concludes. The newly formed DIMO Platform Licensing team will be responsible for the implementation of the programs and procedures introduced in this document.&#x20;

## Copyright&#x20;

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation&#x20;

Please cite this document as:

Andy Chatham, Rob Solomon, Diego Moro, "DIP-4: DIMO Clients, Nodes & Apps", no. 4, June 2022. \[Online serial]. Available: \[https://github.com/DIMO-Network/DIP]
