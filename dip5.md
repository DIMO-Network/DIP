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

The DIMO app ecosystem has several main parties:&#x20;

* **Data Publishers**: Users connect their devices via hardware and software connections;&#x20;
* **Nodes**: receive data from users, validate it, issue proofs of data validity, and serve it to licensed apps and data customers; and
* **Data Subscribers**: Products that make use of user data and connectivity.

This proposal defines how Nodes, and Data Subscribers will form, remain in good standing, and interact with users, their data, and the protocol itself. Data publishers are addressed in [dip4.md](dip4.md "mention").

<img src=".gitbook/assets/file.drawing (8).svg" alt="" class="gitbook-drawing">

## **Motivation**

The goal of this proposal is to put in place a framework that can safely and effectively grow the number of:&#x20;

* Users who will share their data, protect their privacy, spend money in the marketplace and earn rewards;&#x20;
* Number of node runners that make the data easily accessible and provably valid;
* App developers who build applications that make use of the data and connectivity;

## Specifications&#x20;

### Nodes&#x20;

A Node is an entity that receives data from devices and, after validating it against proof of movement, makes it available to Data Subscribers. These entities are responsible for forming and upholding agreements that protect user privacy and enable DIMO applications.&#x20;

Nodes may receive data from several protocols, such as UDP, MQTT, or Streamr Network. They provide API's and interfaces that can be used to access data, and the on-chain indexer.

All data they receive must be encrypted in transit and at rest. Both Nodes and the businesses that they serve must always comply with relevant privacy regulations (e.g., GDPR). **Node operators may only share data with licensed Data Subscribers per the explicit terms of a user's active opt-in**. In other words, any Data Subscriber must receive an explicit signature from a user's wallet in order to receive their data.

Nodes are to DIMO what Infura or Alchemy are to Ethereum.&#x20;

### Data Subscribers&#x20;

Data Subscribers are entities that offer services to users (e.g., a refinancing app) and/or pay users for data (e.g., an electric vehicle R\&D company).

#### Clients&#x20;

A client is a type of application that allows users to interact directly with the DIMO protocol. Typically, this will mean creating and managing their account, creating and managing their vehicle identity, adding and removing credentials in their identity glovebox (e.g., insurance and registration), adding and removing telemetry devices, and viewing back their own data.&#x20;

Clients are to DIMO what Metamask and Rainbow Wallet are to Ethereum. [DIMO Mobile](https://onelink.to/dimo) is an example of a client.

#### Applications&#x20;

An application is a like a light client. It allows users to gain additional value from the protocol by leveraging the data from their vehicle. It will read data and issue commands, but does not mint new vehicles and manage vehicle connections (e.g., pairing a hardware device). Typically this will mean logging in with DIMO to the application and allowing it to access your vehicle data, where the application extends the available insights, enables new savings, or new features on top of the protocol.&#x20;

Some examples of apps include peer-to-peer car rentals, efficient online car marketplaces, defi auto lending, smart insurance, and web3 ride hailing. Uber, Geico, eBay Motors, and Hertz could be rebuilt as leaner, cheaper, and more effective protocols on top of DIMO. [DIMO Explorer](https://explorer.dimo.zone) is an  example of an application.&#x20;

#### Data Consumers

A data consumer is an entity that subscribes to user data. Various businesses will want to purchase traffic, battery, self-driving, video, and other telemetry data. McKinsey published an  overview on the value of data consumption [here](https://www.mckinsey.com/industries/automotive-and-assembly/our-insights/unlocking-the-full-life-cycle-value-from-connected-car-data).

### Licensing

Prospective Clients and Nodes may receive a license by passing a DIP using the [License Approval Template](templates/license-approval-template.md).

Applications and Data Consumers do not require a governance vote to receive a developer license, but must comply with all terms in the Obligations and Bonding sections in order to interact with DIMO Users and their data. The DIMO Foundation is able to issue developer licenses in its discretion.

### Bonding

Clients, Nodes, Applications, and Data Consumers must bond $DIMO (or must have someone do it on their behalf) as defined below. If a licensee violates their obligations as specified below, their license may be suspended or revoked. They may renounce their license and receive back their bonded deposit six months later.

**Nodes**: Must bond 500,000 $DIMO as a one-time deposit.

**Clients**: Must bond 20,000 $DIMO as a one-time deposit.

**Applications & Data Consumers**: Do not need to bond $DIMO for now.

Should applicants not have $DIMO or not want to interact with tokens, they may purchase $DIMO from the Foundation and/or have the Foundation put up the bond on their behalf.

The amounts for bonding, as well as the exchange rate for $DIMO offered by the Foundation, may be altered by any future governance vote.

### Obligations

Clients, Nodes, Apps, and Data Consumers commit to maintaining strict quality and security standards, provide support for their services, always act in good faith, and agree not to engage in unlawful activities. The following is illustrative but not exhaustive.

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

### Temporary Licenses

For six months after the passage of this DIP, the following companies are have a temporary license. Following twelve months, they will need to apply for a permanent license per the process defined above.

* Digital Infrastructure Inc is licensed to operate:
  * Node: [DIMO Web Services](https://devices-api.dimo.zone)
  * Client: [DIMO Mobile](https://onelink.to/dimo)

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

Mar 29, 2023: passed [DIP-4 & 5: Amendment 1](amendments/dip4-and-5a1.md)

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
