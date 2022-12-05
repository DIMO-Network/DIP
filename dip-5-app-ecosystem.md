# DIP-5: App Ecosystem

> **Headline**: How Clients, Nodes, Apps, and Data Consumers get licensed to access User data.
>
> **Author**: The DIMO Foundation
>
> **Submitter**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review
>
> **Voting URL**: Pending

## Abstract

The DIMO app ecosystem has five main components:&#x20;

* **Users**: connect their vehicles, generate data, use apps, and spend/earn $DIMO;&#x20;
* **Clients**: provide interfaces for Users to interact with the protocol (e.g., [DIMO Mobile](https://onelink.to/dimo));&#x20;
* **Nodes**: receive IoT device data from Users and serve it to licensed apps and data customers; and
* **Apps & Data Consumers**: build products that pay node operators for User data and connectivity.

This proposal defines how Clients, Node Operators, and Apps & Data Consumers will form, remain in good standing, and interact with Users, their data, and the protocol itself.

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

## **Motivation**

The goal of this proposal is to put in place a framework that can safely and effectively grow the number of:&#x20;

* Users who will share their data, protect their privacy, spend money in the marketplace and earn rewards;&#x20;
* App developers who build applications that make use of User data and connectivity; and&#x20;
* Service Providers who use apps to help Users solve problems and save money.&#x20;

## Specifications&#x20;

### Clients&#x20;

A client is a type of application that allows Users to interact directly with the DIMO protocol. Typically, this will mean creating and managing their account, creating and managing their vehicle identity, adding and removing credentials in their identity glovebox (e.g., insurance and registration), adding and removing telemetry devices, and viewing back their own data. Clients are to DIMO what Metamask and Rainbow Wallet are to Ethereum. [DIMO Mobile](https://onelink.to/dimo) is an example of a client.

### Nodes&#x20;

A Node is an entity that receives data from Users and makes it available to Clients, Apps, and Data Consumers. These entities are responsible for forming and upholding agreements that protect User privacy and enable DIMO applications. Nodes are to DIMO what Infura or Alchemy are to Ethereum. [DIMO Explorer](https://explorer.dimo.zone/) is an example of a Node.

All stored User data must be encrypted in transit and at rest. Both nodes and the businesses that they serve must always comply with relevant privacy regulations (e.g., GDPR). **Node operators may only share data with licensed Clients, Apps, and Data Consumers per the explicit terms of a User's opt-in**.

### Apps & Data Consumer&#x20;

Apps & Data Consumers are services that provide utility and rewards to Users.&#x20;

Some examples of Apps include peer-to-peer car rentals, efficient online car marketplaces, defi auto lending, smart insurance, and web3 ride hailing. Uber, Geico, eBay Motors, and Hertz could be rebuilt as leaner, cheaper, and more effective protocols on top of DIMO.&#x20;

Data Consumers may be businesses who pay for User data.

### Licensing

Prospective Clients and Nodes may receive a license by passing a DIP using the [License Approval Template](templates/license-approval-template.md).

Apps and Data Consumers do not require a governance vote to receive a license, but must comply with all terms in the Obligations and Staking sections in order to interact with DIMO Users and their data.&#x20;

### Staking

Clients, Nodes, Apps, and Data Consumers must stake $DIMO, or must have someone do it on their behalf. If a staker violates their obligations as specified below, their license may be suspended or revoked. They may renounce their license and receive back their staked deposit six months later.

**Clients**: Must stake 20,000 $DIMO as a one-time deposit.

**Nodes**: Must stake 500,000 $DIMO as a one-time deposit.

**Apps**: There is no stake required if the app has fewer than 40,000 Users. After exceeding this threshold, Apps must stake 10,000 $DIMO per 40,000 Users.

**Data Consumers**: No stake required.

Should applicants not have $DIMO or not want to interact with tokens, they may purchase $DIMO from the Foundation and/or have the Foundation put up the stake on their behalf. The price of $DIMO should be 1 USD equivalent paid in a popular fiat currency (e.g., USD, EUR, GBP), ETH, BTC, or DAI.

The amounts for staking, as well as the exchange rate for $DIMO offered by the Foundation, may be altered by any future governance vote.

### Obligations

Clients, Nodes, Apps, and Data Consumers commit to maintaining strict quality and security standards, provide support for their services, always act in good faith, and agree not to engage in unlawful activities. The following is illustrative but not exhaustive.

They must not:&#x20;

* Interfere with the users safe operation of their vehicle;&#x20;
* Deliberately or negligently generate false data.&#x20;

They must:&#x20;

* Comply with all local regulations;&#x20;
* Only share data with recipients that the user has opted into sharing with per the parameters of the DIMO protocol;
* Use best practices to protect User's and their data; and
* Comply with [dip-3-marketplace-issuance-and-token-burn.md](dip-3-marketplace-issuance-and-token-burn.md "mention") wherever applicable.

### Temporary Licenses

For six months after the passage of this DIP, the following companies are have a temporary license. Following six months, they will need to apply for a permanent license per the process defined above.

* Digital Infrastructure Inc is licensed to operate the Client: [DIMO Mobile](https://onelink.to/dimo) Client and the Node: [DIMO Explorer](https://explorer.dimo.zone/).

## Implementation

If passed, the DIMO Foundation will issue licenses per valid governance votes, and will collect and hold staking deposits.

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-5: App Ecosystem", no. 5, December 2022. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

None

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
