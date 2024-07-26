# DLP-4: Digital Infrastructure Inc.  Device Integration

> **Headline**: DIMO software integration license for Digital Infrastructure Inc.
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

In addition to building DIMO Mobile, hosting data, and contributing R\&D to the DIMO Protocol, Digital Infrastructure. Inc. enables modern vehicles to connect to the DIMO network using their existing cellular subscription, if applicable. Currently, Digital Infrastructure Inc. integrates directly with Tesla APIs and indirectly with other automakers via [Smartcar](https://smartcar.com/), a SOC 2 compliant automotive API aggregator.

## Motivation

Over 200,000,000 vehicles are pre-equipped from the factory with an embedded connectivity service, a number that is [expected to continue to rise rapidly](https://www.juniperresearch.com/press/connected-vehicles-to-surpass-367-million-globally/). DIMO can scale far faster if it can at least partially remove the constraint of aftermarket hardware adapters. In the future, automakers will build their connectivity to a DIMO spec with embedded hardware. Until then, Digital Infrastructure Inc. can make existing integrations compatible by ingesting and transforming data. In this model, connectivity is provided by the OEM and DIMO acts as a storage and consent layer for the user’s vehicle data.

## Specification

Digital Infrastructure Inc. has submitted an application to provide a digital only integration to modern vehicles. The company has completed a KYC/B review and signed a services contract with the DIMO Foundation, but still needs to bond $DIMO per DIP-4 in order to acquire this license.

### Application Type

Integrations Provider (Software)

### Corporate Details

Digital Infrastructure Inc. (https://drivedimo.com) is a Delaware C-Corporation with venture backing by CoinFund, Variant, Slow Ventures, Wonder, Not Boring, Lattice, Borderless, and more. It is the publisher of DIMO Mobile.

### Description of Services

Today, Digital Infrastructure Inc. integrates with [Smartcar](https://smartcar.com) and [Tesla](https://developer.tesla.com/docs/) to access data. This may expand in the future to include more direct integrations (e.g., Ford Pro) or third parties (e.g., High Mobility). Not all vehicles with embedded connectivity will be able to connect depending on compatibility with the provider. The integration will be enabled via synthetic device contracts that are [currently deployed on Polygon](https://polygonscan.com/token/0x4804e8d1661cd1a1e5ddde1ff458a7f878c0ac6d).&#x20;

To connect the synthetic device, users will login to the integration using their OEM credentials (e.g., the email and password they use to login to the Tesla app) and link DIMO to their vehicle. As part of this process, the VehicleID will be minted to the user.&#x20;

The integration provider will give unique signing keys for each device connection to make the data compatible with the storage node and integration requirements. The data will be encrypted with the user’s selected encryption key.

### Technical Specifications

Key Management:

* Data Signing: Each individual embedded device connection signs the data with an individual integration key to make the data compatible with DIMO.
* Enclaves: The keys are dynamically generated and stored in a manner inaccessible to the operator and users of the system.

Encryption

* Data Security: All data is encrypted in transit and is encrypted at rest by the node that stores a user’s data.&#x20;

Ingestion

* Streaming: The data can be received from the integration via an individual stream for a vehicle.
* Polling: For integrations that do not support live data streaming, the integration provider polls the API to retrieve the data on an interval allowed by the integration.

### Commitments to DIMO

Digital Infrastructure Inc. commits to upholding high standards for security, performance, transparency, and collaboration, and will continue to open source the integration code (see code for [Tesla](https://github.com/DIMO-Network/task-worker/blob/d7bd55b8d0b2959fb90e5d4aee1c228e84f75f5e/internal/services/tesla/tesla\_v2.go#L12) and [Smartcar](https://github.com/DIMO-Network/task-worker/blob/d7bd55b8d0b2959fb90e5d4aee1c228e84f75f5e/internal/services/smartcar.go)).

## Implementation

If passed, this DLP will be in effect immediately after the four day timelock concludes and the required bond is posted. This DLP will be updated, with history noted in the [Changelog](dip13.md#changelog), once the bond is posted or updated.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

Yev Khessin & Rob Solomon, "DIP - 13: Digital Infrastructure Inc. Device Integration", no. 13, June 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
