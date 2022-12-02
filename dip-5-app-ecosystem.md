# DIP-5: App Ecosystem

> **Headline**: How Clients, Nodes, Apps, and Data Consumers get licensed to access User data.
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

The DIMO app ecosystem has five main components:&#x20;

* **Users**: connect their vehicles, generate data, use apps, and spend/earn $DIMO;&#x20;
* **Clients**: provide interfaces for Users to interact with the protocol (e.g., [DIMO Mobile](https://onelink.to/dimo));&#x20;
* **Nodes**: receive IoT device data from Users and serve it to licensed apps and data customers;&#x20;
* **Apps & Data Consumers**: build products that pay node operators for User data and connectivity; and&#x20;
* **DIMO** **App Ecosystem**: a team that issues licenses to Clients, Node operators, and Apps.

This proposal defines how Clients, Node Operators, and Apps & Data Consumers will form, remain in good standing, and interact with Users, their data, and the protocol itself.

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

## **Motivation**

The goal of this proposal is to put in place a framework that can safely and effectively grow the number of:&#x20;

* Users who will share their data, protect their privacy, spend money in the marketplace and earn rewards;&#x20;
* App developers who build applications that make use of User data and connectivity; and&#x20;
* Service Providers who use apps to help Users solve problems and save money.&#x20;

## Specifications&#x20;

### Establishing the DIMO App Ecosystem Team

If passed, this proposal would formally recognize the DIMO App Ecosystem team on interim basis and delegate certain rights and duties to it.

A larger and more detailed plan and budget will be presented as part of the [Resource Allocation DIP](templates/resource-allocation-template.md) and community presentation and Q\&A coming within the next 120 days.

#### Purpose&#x20;

The DIMO App Ecosystem team's goal is to maximize earnings, utility, and security for Users. They are tasked with:&#x20;

* Attracting, vetting, licensing, and onboarding data and connectivity Clients, Nodes, Apps, and Data Consumers;
* Monitoring and reporting on the effectiveness and compliance of licensed Clients, Nodes, Apps, and Data Consumers; and
* Generally protecting Users' privacy and security.

#### Team Composition & Operating Structure&#x20;

The initial team lead is [Yev Khessin](https://www.linkedin.com/in/yevgeny-khessin/)[ ](https://www.linkedin.com/in/brien-east-1137516b/details/experience/)(of Digital Infrastructure Inc.) who will be responsible for assembling other contributors and preparing the upcoming presentation.

#### Conflicts

In order to mitigate conflicts of interest, team members agree to reject any form of compensation from current or potential Client, Node, or App & Data Customer, or any of their close affiliates.

#### Authority & Domain&#x20;

DIMO App Ecosystem will have the authority to grant and revoke licenses to Clients, Nodes, Apps, and Data Consumers. However, they cannot lower the initial licensing requirements outlined below.

The $DIMO token holders may overrule DIMO Platform Licensing, may amend the powers and responsibilities this team possesses, and/or may extend these powers and responsibilities to other teams with any valid governance vote.&#x20;

#### Budget & Financial Projections&#x20;

DIMO Integrations is seeking an initial budget of 50,000 $DAI which may be used for any purpose and 10,000 $DIMO to use for testing. The directors of the DIMO Foundation will approve and reimburse invoices as needed.

#### Summary of Commitments&#x20;

DIMO Platform Licensing commits to:&#x20;

* Publish the analysis and outcome from every license application and revocation;&#x20;
* Alert the community, particularly affected Users, and provide a post-mortem if there is ever a major issue concerning a licensed Client, Node, App, or Data Consumer;&#x20;
* Publish metrics as defined in the [Operating Goals & Metrics](dip-5-app-ecosystem.md#operating-goals-and-metrics) section;
* Comply with the terms of the [Conflicts of Interest](dip-5-app-ecosystem.md#conflicts-of-interest) section; and
* Always act in good faith and in the best interest of the DIMO community.&#x20;

### Clients&#x20;

A client is a type of application that allows Users to interact directly with the DIMO protocol. Typically, this will mean creating and managing their account, creating and managing their vehicle identity, adding and removing credentials in their identity glovebox (e.g., insurance and registration), adding and removing telemetry devices, and viewing back their own data. Clients are to DIMO what Metamask and Rainbow Wallet are to Ethereum. [DIMO Mobile](https://onelink.to/dimo) is an example of a client.

Prior to gaining a license, Clients must stake 20,000 $DIMO tokens.

### Nodes&#x20;

A Node is an entity that receives data from Users and makes it available to Clients, Apps, and Data Consumers. These entities are responsible for forming and upholding agreements that protect User privacy and enable DIMO applications. Nodes are to DIMO what Infura or Alchemy are to Ethereum. [DIMO Explorer](https://explorer.dimo.zone/) is an example of a Node.

Node operators must stake 100,000 $DIMO tokens plus an additional 2 $DIMO per connected User. This achieves two purposes: 1) it acts as a security deposit that can be slashed if the operator misbehaves; and 2) it ensures that node operators have their incentives aligned with DIMO. The staked $DIMO will remain locked for as long as the application continues to access User data. Any application may renounce their license and receive back the staked $DIMO after six months if there are no challenges.

All stored User data must be encrypted in transit and at rest. Both nodes and the businesses that they serve must always comply with relevant privacy regulations (e.g., GDPR). Node operators may share data with licensed Clients, Apps, and Data Consumers per the opt-in of Users.

### Apps & Data Consumer&#x20;

Apps & Data Consumers are services that provide utility and rewards to Users.&#x20;

Some examples of Apps include peer-to-peer car rentals, efficient online car marketplaces, defi auto lending, smart insurance, and web3 ride hailing. Uber, Geico, eBay Motors, and Hertz could be rebuilt as leaner, cheaper, and more effective protocols on top of DIMO.&#x20;

Data Consumers may be businesses who pay for User data.

Apps & Data Consumers do not need to stake or pay $DIMO to get started and connect to up to 10,000 Users. After crossing this threshold, they must stake 10,000 $DIMO and burn an additional 1,000 $DIMO for every 20,000 users they serve per month.

### Application

Whoever seeks a license to be a Client, Node, or App & Data Consumer may fill in the application form [here](https://gkmkni9caof.typeform.com/to/Tl3rglKv).

### Payments

Certain payments made between DIMO users, Clients, Nodes, and/or Apps & Data Customers must generate Market Issuance. See [dip-3-marketplace-issuance-and-token-burn.md](dip-3-marketplace-issuance-and-token-burn.md "mention").

## Implementation

The newly formed DIMO App Ecosystem team will be responsible for the implementation of the programs and procedures introduced in this document.&#x20;

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-5: App Ecosystem", no. 5, December 2022. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

None

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
