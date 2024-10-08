# DLP-5: Ruptela Device Integration

> **Headline**: DIMO hardware license approval for Ruptela
>
> **Author:** The DIMO Foundation
>
> **Submitter(s):** The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 1](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

[Ruptela](https://www.ruptela.com/) is a global telematics company established in 2007 in Lithuania. Ruptela develops quality devices in-house, working with clients in over 120 countries. Ruptela is applying for a integration license to produce a DIMO-compatible high bandwidth OBD dongle that uses LTE connectivity with 2G fallback.

## Motivation

This proposal provides transparency to the DIMO community regarding the new DIMO-compatible hardware that Ruptela is planning to bring to the ecosystem and specifies the commitments they must uphold.&#x20;

Granting licenses to new manufacturers broadens the ecosystem and fosters competition with different options for performance, reliability, and cost-effectiveness. Different manufacturers may bring innovative approaches and technologies to the table and reduce single points of failure for the network over time.&#x20;

Due to its compact size, wider vehicle signal support, and connectivity options, the device specified below will bring a lower and more affordable price point for the cost of ownership and connectivity for users to connect to the DIMO network.

## Specification

Ruptela has applied to manufacture DIMO-compatible devices and is currently in the Hardware Ecosystem Pipeline. The company has passed KYC, produced 1,000 devices, and bonded 100,000 $DIMO as part of the application process.

#### **Steps for production are as follows:**

* **Complete**: KYC/B and business audit of the manufacturer, and ongoing orders
* [**Complete**](https://polygonscan.com/tx/0xbf51e75db33e862798f5d577605159f7460fdc5921a594400bb0721376918781): Bond 100,000 $DIMO to acquire a manufacturing license[ as outlined in DIP-4](https://docs.dimo.zone/governance/dip4#licenses-and-bonding)
* **Complete**: Radio/industrial certifications
  * FCC
  * IC
  * PTCRB
  * UKCA
  * CE
* **Within 1 year**: Hardware and security audit

### **Application Type**

Integrations Provider (Hardware)

### Corporate Details

UAB “Ruptela” is the legal name of the company with an address at Address: Perkūnkiemio g. 6, Vilnius, Lithuania.

### Description of Services

Ruptela is a telematics device manufacturer that can design and manufacture a wide range of automotive accessories and electronics that would benefit the DIMO network. Currently, Ruptela is developing a new DIMO flagship high bandwidth OBD device.

### Technical Specifications

The new flagship DIMO device being developed by Ruptela is an LTE/BLE and GPS-enabled high bandwidth OBD Dongle. The key features and specifications are as follows:

**High Level BOM**

<table><thead><tr><th width="291">Component</th><th>Part/description</th></tr></thead><tbody><tr><td>Inputs for Ignition detection</td><td>3 (OBDII Pin1 OR Pin3 OR Pin8)</td></tr><tr><td>CAN 1 Interface</td><td>OBDII Pin 6/14</td></tr><tr><td>CAN 2 Interface</td><td><p>Configuration switchable OBDII Pins: </p><p>3/11 , 3/8 , 1/9, 2/10, Pin1(SW CAN)</p></td></tr><tr><td>K-line interface</td><td>OBDII Pin 7</td></tr><tr><td>J1708 interface</td><td>OBDII Pin 2/10</td></tr><tr><td>Power supply</td><td>12/24V</td></tr><tr><td>USB port</td><td>Yes</td></tr><tr><td>SIM card</td><td>Nano SIM (4FF)</td></tr><tr><td>LED's</td><td><p>Red - Power/Ignition status </p><p>Orange – Network Status </p><p>Green – GNSS status </p><p>Blue – Autoconfiguration</p></td></tr><tr><td>Connectivity</td><td><p>North America Variant: 4G CAT-M1</p><p>B2/B4/B12</p><p>+2G fallback</p><p></p><p>EMEA Variant: 4G CAT-M1 B1/B3/B5/B8/B18/B19/ B20/B28 +2G fallback</p></td></tr><tr><td>GNSS</td><td>Ublox M10</td></tr><tr><td>BLE</td><td>5.1</td></tr><tr><td>Accelerometer</td><td>3 axis (auto-calibrating)</td></tr><tr><td>Temperature</td><td><p>Operating: -20 to +60 °C </p><p>Storage: -20 to +45 °C </p><p>Battery charging: 0 to +45 °C </p><p>Battery discharging: -20 to +60 °C</p></td></tr><tr><td>Humidity</td><td>5% to 95% Non-condensing</td></tr><tr><td>Certifications</td><td><p>North America Variant: FCC / IC /PTCRB</p><p></p><p>EMEA Variant: CE /E-mark</p></td></tr><tr><td>Dimensions</td><td>75mm x 51mm x 27mm</td></tr><tr><td>Weight</td><td>65g +/- 2g</td></tr><tr><td>Housing</td><td>Black Plastic</td></tr></tbody></table>

### Safety Protocols

The device employs the use of a ‘secure element’ that provides communication encryption between the device and the cloud. Data is stored onboard on a flash chip. The device is able to sense the vehicle's acceleration/orientation, track location (both GSM triangulation and GPS), and connect to the vehicle's OBD II port.

### Commitments to DIMO

Ruptela is committed to:

* Act in best faith towards the DIMO community, producing quality hardware and honoring any commitments, timelines, etc.; and
* Comply with all relevant laws and regulations related to the safe production and usage of their devices.

## Implementation

If passed, this DLP will be in effect immediately after the four-day timelock concludes. Ruptela will have the ability to mint valid $DIMO devices. This DLP will be updated, with history noted in the [Changelog](dlp5.md#changelog), if the bond is ever updated.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DLP 5: Ruptela Hardware License", no. 5, October 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.

