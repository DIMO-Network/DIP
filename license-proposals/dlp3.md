# DLP-3: Digital Infrastructure Inc. Node

> **Headline**: DIMO node operator license for Digital Infrastructure Inc.
>
> **Author**: Yev Khessin & Rob Solomon
>
> **Submitter(s)**: zer0stars.eth & robsolomon.eth
>
> **Status**: Approved
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0x9d93ab79916c69c1cbb3356877fb08b8d12f216511115a0572767bc4eba6c32e)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 1](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

Digital Infrastructure Inc. is the corporation that first developed the DIMO protocol and donated its intellectual property to the DIMO Foundation. They are the publishers of the DIMO Mobile app and they continue to contribute to the research and development of DIMO.

This proposal specifies the conditions by which Digital Infrastructure Inc. will develop and run the first DIMO Node, which has four distinct pieces of functionality:

1. Data Storage: DIMO nodes store off-chain data for users and ensure that this data is only shared with authorized parties. This helps in maintaining privacy and control over vehicle data.
2. Indexing: DIMO nodes index on-chain data for users to ensure interoperability and permissioned access.
3. APIs: DIMO nodes provide data retrieval services for on-chain and off-chain data to developers.
4. Plugins: Additional plugins can be deployed as part of the node to provide additional services on top of the raw data from devices and smart contracts.

## Motivation

DIMO must rely on licensed node operators in order to function. Digital Infrastructure Inc. brings significant value to this partnership with its history of security, performance, and contribution to the network. Digital Infrastructure Inc. has committed to open sourcing node software to further decentralization in the future.

## Specification

Digital Infrastructure Inc. has submitted an application to perform as a node operator. The company has completed a KYC/B review and a services contract with the DIMO Foundation. The company still needs to bond $DIMO per DIP-5 in order to acquire this license.

### Application Type

Node operator

### Corporate Details

Digital Infrastructure Inc. (https://drivedimo.com) is a Delaware C-Corporation with venture backing by CoinFund, Variant, Slow Ventures, Wonder, Not Boring, Lattice, Borderless, and more. It is the publisher of DIMO Mobile.

### Description of Services

Secure Storage

* Data Encryption: All data at-rest and in-transit end-to-end must be encrypted using industry-standard encryption protocols to prevent unauthorized access or privacy violations.&#x20;
* Access Control: Implementation of strict access control measures to ensure that only authorized personnel and systems can access sensitive data based on auditable permissions granted by the user in on chain contracts.
* Data Redundancy: Ensuring data redundancy through regular backups and distributed storage solutions to prevent data loss and ensure operational continuity.
* Compliance: Adherence to industry regulations for data security and privacy, ensuring that all data handling practices meet legal and regulatory requirements.&#x20;

Digital Twin Functionality:

* Synchronization: Accurate and real-time mirroring of the on-chain system state into the off-chain digital twin.
* Consistency: Ensuring data consistency between the on-chain and off-chain states, with mechanisms for conflict resolution.
* Scalability: Ability to scale with the growth of the DIMO network by supporting estimated data volumes and integration points.

Service Provision:

* API Services: Provision robust APIs for third-party applications to access and interact within the DIMO platform. This includes core services such as identity, telemetry, and credentials APIs.&#x20;
* Indexing Services: To function, a DIMO node needs to ingest and interoperate with on-chain data.&#x20;
* Performance: The node must support agreed operational level agreements (OLAs) in terms of both functional and non-functional characteristics.

Plugins:

* The node will support a pluggable architecture enabling extensibility. Developers are able to write a custom plug-in themselves leveraging reference implementation or to add optional plug-ins written by ecosystem developers. Examples of plugins include trips, charging and other events data.
* The plugins must follow the same operational and security constraints as the rest of the node hosting plugins. Security boundaries between DIMO nodes can not be crossed.

Compliance and Reporting:

* Reporting: Timely reporting of incidents or anomalies to the DIMO Foundation and community.
* Regulatory Compliance: Adherence to relevant industry regulations and standards for both data management and service provision in the automotive sector.

### Revenue Share

20% of all gross profit made from vehicle data access fees will be returned back to users. For example, if a developer pays the $10,000 worth of $DIMO in one month and $4,000 worth of $DIMO burned, then Digital Infrastructure Inc. will keep $4,800 as gross profit and distribute $1,200 worth of $DIMO to the DIMO Foundation who can distribute this as a reward to users.

### Commitments to DIMO

Digital Infrastructure Inc. commits to upholding high standards for security, performance, transparency, and collaboration, and will open source the source code and deployment scripts via github. The code will be publicly extensible and auditable.

## Implementation

If passed, this DLP will be in effect immediately after the four day timelock concludes and the required bond is posted. This DLP will be updated, with history noted in the [Changelog](dlp3.md#changelog), once the bond is posted or updated.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

Yev Khessin & Rob Solomon, "DLP - 3: Digital Infrastructure Inc. Node", no. 3, June 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
