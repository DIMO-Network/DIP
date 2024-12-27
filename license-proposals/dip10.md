# DLP-1: Hashdog Hardware License



> **Headline:** DIMO hardware license approval for Hashdog, a subsidiary of JDI
>
> **Author:** The DIMO Foundation
>
> **Submitter(s):** The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status:** Deployed
>
> **Voting URL:**[ ](https://snapshot.org/#/dimo.eth/proposal/0x74f67d2da46e74e190063932f7b6a27fdafc7fa368ee5a275335db3a9e666499)[Snapshot](https://snapshot.org/#/dimo.eth/proposal/0xc6303bff64639929d01942b05be5aa9ef71103168089a931519da3c0bb5eedf0)
>
> **Discussion Forum:**[ Discord](https://chat.dimo.zone/) #🗳️governance forum
>
> **Vote Type:** [Level 1](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

Hashdog is an electronics manufacturer based in China. Hashdog is a part of the holding company JDI, which is also the parent company of Bobcat. Bobcat has shipped over 400,000 Helium miners to date, and shares the same engineering team and experience. Hashdog is applying for a Manufacturing License to produce a DIMO compatible OBD dongle that uses the Helium LoRaWAN network along with Bluetooth.&#x20;

## Motivation

This proposal provides transparency to the DIMO community regarding the new DIMO-compatible hardware that Hashdog is planning to bring to the ecosystem and specifies the commitments they must uphold.&#x20;

Granting licenses to new manufacturers broadens the ecosystem and fosters competition with different options for performance, reliability, and cost-effectiveness. Different manufacturers may bring innovative approaches and technologies to the table and reduce single points of failure for the network over time.

Due to its LoRaWAN/Bluetooth connectivity, the Mini OBD Dongle specified below will bring a lower price point (both in terms of upfront cost and ongoing connectivity) for users to connect to the DIMO network.

## Specification

Hashdog has submitted an application to manufacture DIMO-compatible devices and is currently in the Hardware Ecosystem Pipeline. The company has completed a KYC/B review and a Memorandum of Understanding with the DIMO Foundation as part of the application process. Hashdog has [already bonded 100,000 $DIMO](https://polygonscan.com/tx/0x1e7c78d478f70813ae996e0a4d3e87e7864b3e7b03c60afafc236940a17f4cf2) and started working on the development of a LoRaWAN/Bluetooth Mini OBD Dongle.

#### **Steps for production are as follows:**

* **Complete:** KYC/B and business audit of the manufacturer
* [**Complete**](https://polygonscan.com/tx/0x1e7c78d478f70813ae996e0a4d3e87e7864b3e7b03c60afafc236940a17f4cf2)**:** Bond 100,000 $DIMO to acquire a manufacturing license [as outlined in DIP-4](https://docs.dimo.zone/governance/dip4#licenses-and-bonding)
* **Complete:** Radio/industrial certifications
  * FCC
  * ISED
  * UKCA
  * CE
* **Complete:** Device audit
  * Hardware and security audit
  * Hardware test plan and quality control assessment
  * Customer experience assessment
* **Complete:** Spending 25 $DIMO per device to mint them on-chain [as outlined in DIP-4](https://docs.dimo.zone/governance/dip4#cost-of-device-minting)

### **Application Type**

This DLP is an application for a Manufacturing License (Hardware Integration Provider) for Hashdog, enabling them to produce a new DIMO compatible Mini OBD Dongle is currently in the design and manufacturing stage. After completing a thorough audit of the device, and upon obtaining the necessary radio/industrial certifications, an application for a Device certificate will be submitted.

### Corporate Details

HASHDOG PTE.LTD is the legal name of the company with an address at 152 Beach Road #11-05 Gateway East Singapore 189721.

### Description of Services

Hashdog is an IoV (Internet of Vehicles) manufacturer that has the ability to design and manufacture a wide range of automotive accessories and electronics that would benefit the DIMO network. Currently, Hashdog is developing an open source DIMO flagship Mini OBD Dongle.&#x20;

### Technical Specifications

The open sourced flagship DIMO device being developed by Hashdog, is a LoRa/BLE and GPS enabled Mini OBD Dongle. The architecture diagram and high level BOM are provided below.\


**High Level BOM**

<table><thead><tr><th width="322">Component</th><th>Part/Description</th></tr></thead><tbody><tr><td>Microcontroller</td><td>nRF52840</td></tr><tr><td>CAN Controller, Transceiver</td><td>MCP2515, MCP2551</td></tr><tr><td>LoRa Transceiver</td><td>SX1262</td></tr><tr><td>GPS</td><td>UBX-M10050-KB</td></tr><tr><td>Inertial Measurement Unit (IMU)</td><td>LSM6DS3TR-C</td></tr><tr><td>Secure Element</td><td>SE050</td></tr><tr><td>Memory</td><td>32MB NOR Flash</td></tr><tr><td>Power management</td><td>Up to 48V IN, DC to DC</td></tr><tr><td>Connector</td><td>OBD-II Connector, USB-C (OBD-C)</td></tr><tr><td>Antennas</td><td>GPS, LoRa, BLE FPC Antennas</td></tr><tr><td>Enclosure</td><td>Rugged handheld ABS design with external labels and internal electromagnetic shielding</td></tr></tbody></table>

### Safety Protocols

The device employs the use of a ‘secure element’ that provides communication encryption between the device and the cloud. Data is stored onboard on a 32MB NOR flash chip. The device is able to sense the vehicle's acceleration/orientation, track location (both LoRaWAN triangulation and GPS), and access the vehicle's OBDII port.&#x20;

### Commitments to DIMO

Hashdog is committed to:

* Act in best faith towards the DIMO community, producing quality hardware and honoring any commitments, timelines, etc.; and
* Comply with all relevant laws and regulations related to the safe production and usage of their devices.

## Implementation

If passed, this DLP will be in effect immediately after the four day timelock concludes. Hashdog will have the ability to mint valid $DIMO devices, so long as they have completed the aforementioned requirements.

## Copyright

Copyright and related rights waived via[ CC0](https://creativecommons.org/publicdomain/zero/1.0)​

## Citation

Please cite this document as:

The DIMO Foundation, "DLP 1: Hashdog Hardware License", no. 1, August 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

July 6, 2024: disclaimer adjusted,  DLP terminology added, and Steps for Production updated

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

\
