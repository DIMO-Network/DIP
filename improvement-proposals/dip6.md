# DIP-6: The DIMO Foundation

> **Headline**: Establishing the role of the DIMO Foundation legal entity
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
> **Vote Type**: [Level 2](dip1.md#voting-protocol)

## Abstract

This DIP makes explicit the powers, process, and expectations of the DIMO Foundation. Notably, it acknowledges the Foundation's role as an administrator on smart contracts and intellectual property rights; explains their role as a bridge to the legacy business world on behalf of the DIMO community; and enables the foundation to use a portion of the treasury to fund operational costs, sell tokens to third parties, and/or make tokens available to market makers.

## Motivation

Forming and delegating rights to a legal entity is necessary for DIMO to interact in today's world among business and governments. This proposal aims to maximize transparency and the capabilities of the DIMO protocol while minimizing the liability for participants.

## Specification

### Team Name

The DIMO Foundation

### Purpose & Mission

The DIMO Foundation has been formed to help DIMO navigate the challenges of operating in a world with legacy businesses and regulations. It exists to help DIMO grow to the become the world's best and biggest network, while remaining compliant. Having an entity in a defined jurisdiction is helpful for the purposes of minimizing community liability, clarifying tax requirements, establishing intellectual property rights, entering into traditional contracts, and more.

The power and importance of the DIMO Foundation should shrink over time as DIMO matures and regulations evolve.&#x20;

### Execution Plan & Team Operating Structure

The DIMO Foundation is controlled by professional directors registered with the Cayman Islands Monetary Authority (CIMA) with extensive legal, financial, and blockchain experience. More information on the structure of the foundation can be found at [DIMO Foundation Information](https://app.gitbook.com/o/IDM0isB8NflgM8HmoQc9/s/XrD4OPpblYqPDIzou05o/ "mention").

Notably, Digital Infrastructure Inc., the corporation that initially developed DIMO, continues to contribute under a services agreement. The DIMO Foundation and community will continue to engage various contributors across many companies and geographies to build a distributed network of teams helping to build DIMO.

### Financial Plan & Ask

**(a) Resources.** The Foundation may sell $DIMO from treasury without per-sale governance approval to fund operations, liquidity, strategic partnerships, and investments that materially advance the protocol. Sales may be conducted via programmatic execution, RFQ/OTC transactions, auctions, or strategic placements.

**(b) Use of Funds.** Net proceeds may be applied to: (i) protocol R\&D and operations; (ii) ecosystem and distribution partnerships; (iii) incubation, acquisition, or investment in DIMO-aligned products and businesses (including equity, token warrants, SAFEs, and convertibles); (iv) regulatory, security, and risk management functions; and (v) liquidity and market quality programs.

1. The Foundation may invest in or acquire teams and assets that accelerate adoption. Any acquired IP must comply with Section (d). Strategic sales should include use-commitments or lockups where appropriate.
2. The Foundation may provide or loan $DIMO to approved market makers, operate or seed on-chain liquidity, and enter inventory-neutral arrangements to improve spread, depth, and availability.
3. The Foundation may hold and rebalance reserves across fiat, stablecoins, short-duration instruments, and qualified yield vehicles (e.g., registered funds and cash-management vehicles) to extend runway and manage risk, up to 100% of non-$DIMO reserves, subject to compliance and custody controls.
4. All expenditures, contracts, and treasury actions must primarily benefit the DIMO protocol and $DIMO token.

**(c) Operating Envelope.** The Foundation may adopt and revise an internal annual operating plan (OPEX + program spend) without fixed category caps.

**(d) IP & Work Product.** All IP funded by the Foundation must be (i) owned by the Foundation, (ii) perpetually and royalty-free licensed to it, or (iii) open-sourced under a permissive license, with the Foundation retaining perpetual usage rights.

### Authority & Domain

#### Smart contract admin

The DIMO Foundation Gnosis Safe [Wallets](https://app.gitbook.com/s/XrD4OPpblYqPDIzou05o/wallets "mention") are the admins on various protocol [smart contracts](https://dimo.zone/transparency) such the token itself, baseline issuance, governance, and registry contracts. These permissions allow smart contracts to be upgraded.&#x20;

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

#### Canonical Tokens

The DIMO Foundation may unilaterally update DIP-10 to reflect changes to canonical token definitions, including but not limited to the addition or removal of supported blockchains, contract addresses, and token identifiers. Such updates must be made in good faith, solely for the benefit of the DIMO protocol and $DIMO token, and published promptly in the official governance documentation.

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

Mar 29, 2023: passed [DIP-6: Amendment 1](../amendments/dip6a1.md)

Aug 31, 2023: passed [DIP-6: Amendment 2](../amendments/dip6a2.md) and [DIP-6: Amendment 3](../amendments/dip6a3.md)

Jul 6, 2024: disclaimer adjusted and updated per [DIP-6: Amendment 4](../amendments/dip6a4.md)

Dec 27, 2024: passed [DIP-6: Amendment 5](../amendments/dip6a5.md)

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
