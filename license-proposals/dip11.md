# DIP-11: AutoPi Device Integration

> **Headline**: DIMO hardware license approval for AutoPi
>
> **Author:** The DIMO Foundation
>
> **Submitter(s):** The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Approved
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0x9d93ab79916c69c1cbb3356877fb08b8d12f216511115a0572767bc4eba6c32e)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 1](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

AutoPi.io ApS is a company that produces advanced Internet of Things (IoT) devices based on the Raspberry Pi™ and an extendable cloud platform for vehicles. Their flagship product, the AutoPi, is an LTE OBDII enabled device that is able to transmit vehicle data, in addition to collecting data from onboard sensors. AutoPi is applying for a Manufacturing License to continue producing a DIMO compatible OBD devices.

## Motivation

[AutoPi](https://www.autopi.io/)’s temporary hardware manufacturing license has expired and as per [DIP 4](https://docs.dimo.zone/governance/\~/changes/BVHxKwYX8U5GDtrtGJCU/improvement-proposals/dip4), this proposal serves as a review of their application for a permanent hardware manufacturing license. Additionally, this proposal provides transparency to the DIMO community regarding the new DIMO-compatible hardware that AutoPi.io is already delivering to the ecosystem, and specifies the commitments they must uphold as licensed hardware manufacturer.

## Specification

AutoPi.io has submitted an application to continue to manufacture and support DIMO-compatible devices. Over 13,000 devices have been sold to customers on the DIMO network. From DIMO's early days, AutoPi has been a key partner with DIMO in providing functional devices quickly.

#### **Steps for production are as follows:**

* **Complete**: KYC/B and business audit of the manufacturer, and ongoing orders
* [**Complete**](https://polygonscan.com/tx/0x7420ce4c6e391fe451a004c32cc22b529195ce0bf3472ae840e6f9590e102c29): Bond 100,000 $DIMO to acquire a manufacturing license[ as outlined in DIP-4](https://docs.dimo.zone/governance/dip4#licenses-and-bonding)
* **Complete**: Radio/industrial certifications
  * EN 301 489-1 v2.2.0,&#x20;
  * EN55025:2008,&#x20;
  * EN 50498/ Directive 2004/104/EC
  * ISO 7637-2:2011&#x20;
  * EN 301 489-3 V2.1.1
  * FCC 47 CFR Part 15, Class A:10–1–17 Edition
* **Complete**: Web API audit

{% file src="../.gitbook/assets/AutoPi Web API Audit.pdf" %}

### **Application Type**

Integrations Provider (Hardware)

### Corporate Details

AutoPi.io ApS | VAT: DK38816233 is the legal name of the company with an address at Alexander Foss Gade 13, 3. -2 9000 Aalborg, Denmark

### Description of Services

AutoPi.io is a proven and professional partner to the DIMO ecosystem. AutoPi has demonstrated the ability to build reliable devices at scale, as well as the ability to provide quality management cloud solutions.

### Technical Specifications

The AutoPi device is an LTE enabled OBDII vehicle telematics device, powered by a Raspberry Pi. The architecture diagram and high level BOM are provided below.

**High Level BOM**

<table><thead><tr><th width="291">Component</th><th>Part/description</th></tr></thead><tbody><tr><td>Processor</td><td>Broadcom BCM2711 Quad-core Cortex-A72 (ARM v8) 64-bit SoC @ 1.5GHz</td></tr><tr><td>Memory</td><td><p>1GB LPDDR4 SDRAM</p><p>Upgrade: 2GB, 4GB or 8GB LPDDR4 SDRAM (depending on model)</p></td></tr><tr><td>Storage</td><td><p>8GB on board eMMC</p><p>Upgrade: 16GB and 32GB (depending on model)</p></td></tr><tr><td>Size, Weight and Casing</td><td>Casing: Improved expansion options with exchangeable back shield for external antennas, additional USB ports, ethernet port.</td></tr><tr><td>Modem</td><td><p>Integrated 4G/LTE Cat 4 connection (3G/EDGE fallback)</p><p>150Mbit DL / 50Mbit UL</p><p>Worldwide support in a single device</p><p>4G LTE Bands (Global): B1 / B2 / B3 / B4 / B5 / B7 / B8 / B12 / B13 / B18 / B19 / B20 / B25 / B26 / B28 / B38 / B39 / B40 / B41</p><p>3G Fallback (WCDMA): B1 / B2 / B4 / B5 / B6 / B8 / B19</p><p>EDGE Fallback: B2 / B3 / B5 / B8 / Quad-band</p></td></tr><tr><td>Certifications</td><td>EN 301 489-1 v2.2.0, EN55025:2008, EN 50498 and Directive 2004/104/EC, ISO 7637-2:2011, EN 301 489-3 V2.1.1, FCC 47 CFR Part 15, Class A:10–1–17 Edition</td></tr><tr><td>Security Element (NEW)</td><td><p>Hardware Based Secure Key Management</p><p>Public Key Algorithms: RSA and ECC asymmetric, AES and DES symmetric cryptography algorithms. HMAC, CMAC, SHA-1, SHA-224/256/384/512 operations</p><p>Crypto Curves: ECC NIST, Brainpool, Twisted Edwards Ed2551, Montgomery Curve25519, Koblitz, Barreto-Naehrig Curve, Montgomery Curve448</p><p>Secure Storage of Keys, Certificates and Data</p><p>Unique Serial Number</p><p>Intrusion Detection</p></td></tr><tr><td>GPS</td><td><p>Integrated GPS + A-GPS.</p><p>Supports: GPS/GLONASS/BeiDou/Galileo/QZSS</p></td></tr><tr><td>Power</td><td><p>Line Voltage: 12.5V AC (Car battery power). Up to 35V (Trucks).</p><p>Support for trucks with up to 35V</p><p>Built-in Power Management system to prevent the vehicle’s battery from being drained</p></td></tr><tr><td>Expansion</td><td><p>2 X USB: USB 2.0</p><p>Ethernet: Built in Ethernet</p><p>GPIO: UART/I2C/SPI</p></td></tr><tr><td>Wireless</td><td><p>Built on Cypress CYW43455 Chipset</p><p>WiFi: 2.4GHz and 5GHz IEEE 802.11.b/g/n/ac wireless LAN</p><p>Bluetooth: Bluetooth 5.0 + Bluetooth Low Energy (BLE</p></td></tr><tr><td>Accelerometer</td><td>Built in 3-axis accelerometer</td></tr><tr><td>Gyroscope</td><td>Built in 3-axis gyroscope</td></tr><tr><td>Automotive Interface</td><td><p>2 X CAN: CAN interface with up to 1Mbps Data rate with integrated CAN data filter</p><p>DoIP: Upgradeable to allow support for DoIP</p></td></tr><tr><td>Input slots</td><td>SIM Card: Nano SIM – Not Included</td></tr><tr><td>Audio</td><td>Built-in speakers</td></tr><tr><td>Video Out</td><td>HDMI @ 1080P60 Video Output</td></tr><tr><td><p>Absolute Maximum</p><p>Operating Environment</p></td><td><p>Operating Temperature: -20° TO 70° C (-4° TO 158° F)</p><p>Relative Humidity: 0% TO 75% Noncondensing</p></td></tr><tr><td>Operating System</td><td>Raspbian OS with preconfigured AutoPi Core</td></tr></tbody></table>

### Safety Protocols

The device employs the use of a ‘secure element’ that provides communication encryption between the device and the cloud. Data is stored onboard.

### Commitments to DIMO

AutoPi is committed to:

* Act in best faith towards the DIMO community, producing quality hardware and honoring any commitments, timelines, etc.; and
* Comply with all relevant laws and regulations related to the safe production and usage of their devices.

## Implementation

If passed, this DIP will be in effect immediately after the four day timelock concludes. AutoPi will have the ability to mint valid $DIMO devices, so long as they maintain this license. This DIP will be updated, with history noted in the [Changelog](dip11.md#changelog), if the bond is ever updated.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP - 11: AutoPi Device Integration", no. 11, June 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

