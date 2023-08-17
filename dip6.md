# DIP-6: The DIMO Foundation

> **Headline**: Establishing the role of the DIMO Foundation legal entity
>
> **Author**: The DIMO Foundation
>
> **Submitter**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Deployed
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0x74f67d2da46e74e190063932f7b6a27fdafc7fa368ee5a275335db3a9e666499)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 2](dip1.md#voting-protocol)

## Abstract

This DIP makes explicit the powers, process, and expectations of the DIMO Foundation. Notably, it acknowledges the Foundation's role as an administrator on smart contracts and intellectual property rights; explains their role as a bridge to the legacy business world on behalf of the DIMO community; and enables the foundation to use a portion of the treasury to fund operational costs, sell tokens to third parties, and/or make tokens available to market makers.

## Motivation

Forming and delegating rights to a legal entity is necessary for DIMO to interact in today's world among business and governments. This proposal aims to maximize the capabilities of the DIMO protocol while minimizing the liability for participants while preserving transparency.

## Specification

### Team Name

The DIMO Foundation

### Purpose & Mission

The DIMO Foundation has been formed to help DIMO navigate the challenges of operating in a world with legacy businesses and regulations. It exists to help DIMO grow to the become the world's best and biggest network, while remaining compliant. Having an entity in a defined jurisdiction is helpful for the purposes of minimizing community liability, clarifying tax requirements, establishing intellectual property rights, entering into traditional contracts, and more.

The power and importance of the DIMO Foundation should shrink over time as DIMO matures and regulations evolve.&#x20;

### Execution Plan & Team Operating Structure

The DIMO Foundation is controlled by professional directors registered with the Cayman Islands Monetary Authority (CIMA) with extensive legal, financial, and blockchain experience. More information on the structure of the foundation can be found at [DIMO Foundation Information](http://127.0.0.1:5000/o/IDM0isB8NflgM8HmoQc9/s/XrD4OPpblYqPDIzou05o/ "mention").

Notably, Digital Infrastructure Inc., the corporation that initially developed DIMO, continues to contribute under a services agreement. The DIMO Foundation and community will continue to engage various contributors across many companies and geographies to build a distributed network of teams helping to build DIMO.

### Financial Plan & Ask

#### Resources

The Foundation currently has 1,127,503.27 $DAI in its [Wallets](http://127.0.0.1:5000/s/XrD4OPpblYqPDIzou05o/wallets "mention"), which is what remains of the 1,250,000 $DAI donated by Digital Infrastructure Inc.&#x20;

The Foundation is actively working to open up a bank account and would convert some of that $DAI to fiat US dollars.

#### Budget

The DIMO Foundation anticipates spending approximately $800,000 in 2023. $200,000 of that would be on administrative overhead, including directors salaries, legal fees, insurance, KYC services, technology subscriptions, and more. Another $600,000 would be to compensate contributors who build and grow the DIMO protocol. Digital Infrastructure Inc. is under contract to provide services at $150 per hour and is expected to be the largest such contributor.

To leave some extra buffer for the unexpected, **this proposal gives the DIMO Foundation the authority to spend up to 1,000,000 in USD equivalent in 2023 for relevant operations**.

#### Treasury Initiatives

Additionally, this proposal authorizes the DIMO Foundation to sell up to 25,000,000 $DIMO tokens and to loan up to 25,000,000 $DIMO tokens to market makers.

The DIMO Foundation may not sell this specific pool of tokens below $0.30. A minimum one-year lockup is required on token sales unless there is a bona fide expectation that the purchaser will use a majority of those tokens themselves to use DIMO, such as to produce devices or operate a node.

The Foundation will make its best effort to balance regulatory, financial, and strategic considerations to maximize the long-term health of the DIMO protocol.

These tokens would come from the [unallocated treasury pool](https://docs.dimo.zone/overview/dimotoken/token-details-and-distribution) of 250,000,000 $DIMO. This may be amended or deals on other terms (e.g., below $0.30) may be authorized by any valid governance vote.

### Authority & Domain

#### Smart contract admin

The DIMO Foundation Gnosis Safe [Wallets](http://127.0.0.1:5000/s/XrD4OPpblYqPDIzou05o/wallets "mention") are the admins on various protocol [smart contracts](https://dimo.zone/transparency) such the token itself, baseline issuance, governance, and registry contracts. These permissions allow smart contracts to be upgraded.&#x20;

The DIMO Foundation may only utilize this administrative privilege as authorized by governance votes. Eventually, all administrative privileges should be transitioned to on-chain governance contracts.

In order to maximize the speed of new feature deployment, this DIP authorizes the Foundation to deploy upgrades that grant new functionality without taking away previous rights and functionality to smart contracts. E.g., adding roles to the Vehicle ID contract that allow users to delegate access to their car.

#### Treasury

The DIMO Foundation will allocate the treasury as specified by approved valid DIMO governance votes (including this one), but may veto allocations if it makes a good faith determination that such a distribution would violate applicable law. Accordingly, the DIMO Foundation may require KYC for distributions. Note that KYC is not required for issuance as described in other DIPs, but wallets flagged by Chainalysis' [AML tools](https://www.chainalysis.com/free-cryptocurrency-sanctions-screening-tools/) as risky or fraudulent may be denied issuance.

#### Entering into contracts

The DIMO Foundation may execute binding legal contracts as appropriate to carry out its duties described within this proposal. Transparency must be emphasized wherever possible. There may be contracts or legal disputes that cannot be shared or which may require redaction.

#### Utilize intellectual property and represent the brand

The DIMO Foundation may utilize it's IP, including code, trademarks, web domains, and more. The DIMO Foundation may unilaterally authorize the use of the brand by third parties for the promotion of DIMO (e.g., to announce a partnership or promote the project). Digital Infrastructure Inc., the corporation that initially created DIMO and contributed this intellectual property to the DIMO Foundation currently has a license to utilize that IP. Licensing intellectual property for other reasons must be approved by token holder vote.

#### License revocation

For DIPs where licenses can be revoked for negligence or malice that harms users or the  protocol generally, only the DIMO Foundation or a Cayman court of law may determine if that negligence or malice is demonstrable and material.

### Commitments to DIMO

The DIMO Foundation commits to always:

* Act honorably and in the best interest of the protocol;
* Honor governance votes wherever safe and possible;
* Strive to maximize transparency where possible; and
* Avoid conflicts of interest.

### Key Risks

Due to the lack of regulatory clarity, all blockchain projects have risk. No structure, including this one, has been rigorously tested in court. That said, the DIMO Foundation and its contributors have worked with top Cayman and offshore legal counsel, tax firms, and advisors to deploy the best possible entity structure and operating plan. The DIMO Foundation is constructed very similarly to many of the most reputable and successful blockchain communities.

## Implementation

If passed, this DIP will be in effect immediately after the four day timelock concludes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-6: The DIMO Foundation", no. 6, January 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Jan 9, 2023: added financial ask section and combined execution plan and team operating structure sections

Mar 29, 2023: passed [DIP-6: Amendment 1](amendments/dip6a1.md)

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
