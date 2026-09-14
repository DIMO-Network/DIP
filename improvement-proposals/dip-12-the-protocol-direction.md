# DIP-12: The Protocol Direction

> **Headline**: Define DIMO as an open protocol for vehicle data and a future sessions economy, put vehicles on-chain as verifiable assets, execute a one-time burn of 150,000,000 $DIMO from the treasury, authorize moving the protocol's session records onto Ethereum, and stop baseline issuance
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Approved
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/s:dimo.eth/proposal/0x10aa4f704d997b823d6180ffbfb2bd3bf1849fd4ec5b6cf6fcd30f85f28961b8)
>
> **Discussion Forum**: [Discord](https://chat.dimo.org/) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

DIMO's founding belief is that a vehicle is one of the most valuable assets a person or business owns, and that it belongs on-chain, with a verifiable identity and a record of its history and condition that the owner controls. DIMO is an open protocol built around that belief: identity, consent, data, and audit primitives that anyone can build on, for vehicle data today and a sessions economy as it develops. This DIP makes four changes. First, it makes the protocol itself DIMO's focus: open, permissionless, and neutral among the builders that use it. Second, it burns 150,000,000 $DIMO from the treasury, which takes the Foundation under 20% of supply, and authorizes further burns of fee revenue without requiring them. Third, it authorizes, without scheduling or requiring, a move of the protocol's session records (vehicle identity, attestations, consent) to Ethereum, where the $DIMO token has always lived. Fourth, it ends baseline issuance: the weekly distribution stops at enactment and everything already earned is honored (amending [DIP-2](/broken/pages/fc0796d7a412dba32e03108d50485a184a9b5f0c)). A companion proposal, [DIP-13](/broken/pages/002c257cb73bea7cfc873306730346ae898dd8fb) (Foundation Treasury Reform), ends the Foundation's free-spending treasury authority and commits the Foundation to treating every builder on the protocol the same, the labs entity included. Each proposal stands on its own.

## Motivation

The original [Baseline Issuance](/broken/pages/fc0796d7a412dba32e03108d50485a184a9b5f0c) model paid drivers newly issued $DIMO for connecting a car and sending data. It grew the network past 200,000 vehicles on four continents. It also produced a lot of low-value data, attracted connections that existed mainly to farm rewards, and diluted holders every week without creating demand to offset the new supply.

The demand that lasted was for the protocol's core: signed, tamper-proof vehicle data that can be trusted without trusting anyone. Fleet and rental operators want one integration instead of five tools. Lenders finance a computer on wheels they otherwise see once a quarter. Tolling and insurance companies need attestations they can verify. That demand attaches to the protocol, not to any one company's product.

So this DIP orients the protocol, the treasury, and the token around real usage instead of a bootstrap subsidy for a network that is now built, and changes the tokenomics to match.

## Specification

### Vision: a vehicle is an asset that belongs on-chain

A vehicle is one of the largest assets most people or businesses will ever own. It gets bought and sold, financed, leased, insured, and rented. Yet it lives almost entirely off-chain. Its title sits on paper in a drawer. Its history is scattered across dealerships and DMV records. Its condition stays unknown until something breaks. A multi-trillion-dollar asset class is economically illegible.

DIMO exists to change that. A vehicle should have an on-chain identity tied to its VIN, an owner-controlled record of where it has been and what shape it is in, and signed attestations (VIN, odometer, position, health) that a third party can check without trusting DIMO. That would make a vehicle something a lender can price in real time and a fleet can grant or revoke access to in one transaction. On-chain does not mean public: the owner holds the keys, and consent is explicit and revocable.

Verified identity, history, and condition are what lenders, insurers, fleets, and OEMs need. Using the network to get them costs network fees under [DIP-3](/broken/pages/2e71d0fa926050bcbb64d35bac75de825d1edead), and the Foundation may burn part of that fee revenue to reduce token supply (§2). Each vehicle brought on-chain makes the protocol, and the asset class it describes, more useful.

### 1. The protocol direction

DIMO is an open protocol for vehicle data: a verifiable identity tied to a VIN, signed telemetry and attestations attached to it, and owner-controlled consent over who may access what. A sessions economy can grow on top. Every time someone uses a vehicle they don't own (a rental, a car-share, a financed lease, a fleet assignment), that is a session, and a session needs identity, consent, data, payments, and an audit trail. The protocol supplies those primitives and connects to more than 50 vehicle brands through a single integration. What gets built with them is up to builders.

The protocol is most useful where a vehicle is a working asset: fleets, rental operators, Turo hosts, rideshare and delivery drivers, owner-operators. An integration that handles access, tracks condition, proves mileage, and settles payments can replace five tools and a spreadsheet. Those products are for builders to offer. Baseline issuance ends in §4: a working vehicle connects for the product, not the subsidy.

The connected-vehicle base stays part of the open protocol. Consumer apps and data marketplaces are left to independent builders, who may offer them or not; neither the protocol nor the Foundation operates or promises them. The protocol's economics rest on network fees paid by those who use it, and the Foundation's remit narrows to the protocol itself: keeping it open, neutral, and changed only by governance. The Foundation is neutral among builders, including Digital Infrastructure Inc., the independent company that first developed DIMO (the labs entity), which builds on the protocol on the same terms as everyone else. The Foundation provides the labs entity no funding and no preferential terms; [DIP-13](/broken/pages/002c257cb73bea7cfc873306730346ae898dd8fb) sets out the mechanics, and nothing in this DIP creates obligations for the labs entity.

This is a direction, not a reversal. The protocol stays open and permissionless, and users keep ownership and control of their own vehicles and data.

### 2. Supply: a one-time burn, then discretionary burns

$DIMO is the token used to pay for the DIMO network. On supply, this DIP does one binding thing and one permissive thing. The binding one is a one-time burn of 150,000,000 $DIMO from the treasury. The permissive one is an authorization: the Foundation may burn additional $DIMO from network fee revenue when it judges that useful. Nothing in this section is a payment to holders or a claim on the Foundation's revenue or profit.

**One-time supply decentralization.** When this passes, the Foundation will burn a fixed **150,000,000 $DIMO** from its treasury. The Foundation holds about 300,000,000 $DIMO today, roughly 30% of the 1,000,000,000 total supply. A burn reduces the Foundation's holdings and the total supply together, so this takes the Foundation to about 150,000,000 of roughly 850,000,000 remaining: about **17.6%**.

The CLARITY Act expects a "mature blockchain system" to have no issuer or insider group holding or directing 20% or more of tokens or votes, and no party able to unilaterally control or change the network; distribution is only part of that. The Foundation still holds upgrade authority over certain protocol contracts under DIP-6. Removing that control would be a matter for future DIPs, and this DIP makes no commitment on whether or when. Other holders' balances are outside its control, and it makes no commitment about them either. The treasury reform proposed in [DIP-13](/broken/pages/002c257cb73bea7cfc873306730346ae898dd8fb) would remove one unilateral lever now: if it passes, the Foundation loses the ability to sell or spend from the treasury at its own discretion. This DIP does not by itself make the network "mature."

**Discretionary burns.** The Foundation is authorized, but not required, to burn $DIMO it receives as network fees, principally its 60% share of the $DIMO paid for DIMO Credit (DCX) under [DIP-3](/broken/pages/2e71d0fa926050bcbb64d35bac75de825d1edead). This is a permission, not a rule. No amount, share, or cadence is promised, burns may be irregular or may never occur, and holders should not price the token on the expectation of them. The 40% of the DIP-3 pool paid to nodes is untouched, and fees invoiced in fiat or stablecoins are not a source of burns. Any burn that happens goes to a public burn address on **Ethereum**, with supply on other chains reconciled through the canonical bridges in [DIP-10](/broken/pages/7d4a20e69a417a06eb1becfa6c0379088b232dea), and is posted with its transaction so anyone can verify it.

Both kinds of burn are authorized directly by this DIP. A burn pays no counterparty and benefits every holder ratably, so it is not treasury spending that needs budget authorization under [DIP-13](/broken/pages/002c257cb73bea7cfc873306730346ae898dd8fb), if that proposal is enacted. Every other treasury outflow stays governed by DIP-6 as it stands or as amended.

**On classification.** $DIMO is built to work as a digital commodity. Any value it has is meant to come from using and running the network, not from a promise of profit from the Foundation's work. A burn is a supply action, not a dividend, revenue share, or yield, and it gives holders no claim on anyone. Because ongoing burns are discretionary, they are not a mechanism to rely on. The one-time burn, and the DIP-13 treasury reform if that proposal passes, are designed to move $DIMO toward the CLARITY Act's "digital commodity" framework. The Act is not law yet and its wording may change. Nothing here promises any price, profit, or return.

### 3. Session infrastructure on Ethereum

The $DIMO token has always lived on Ethereum, bridged to Base, Optimism, and Polygon per [DIP-10](/broken/pages/7d4a20e69a417a06eb1becfa6c0379088b232dea). This section covers the **session infrastructure** built on DIMO: vehicle identity, attestations (VIN, odometer, position, health), consent records, and the registry that ties them together. This DIP **authorizes** moving those records to **Ethereum mainnet**. Authorization is not a schedule. The migration may proceed in stages, later, or not at all, and no timeline is promised.

The reason is durability. These records are what make a vehicle a verifiable on-chain asset, and a vehicle is a long-lived thing. On Ethereum, a lender, insurer, or buyer can trust its identity and history without trusting DIMO, on the chain built to hold value rather than whichever chain is cheapest this year.

What would go on Ethereum is proof, not personal data. A vehicle's VIN, registration, insurance, and history stay off-chain, encrypted, under the owner's control, where they can be corrected or deleted. Mainnet would hold commitments and signed proofs: a third party can confirm an attestation is genuine, or that a claim holds (a valid VIN, an odometer reading, a clean title), without the underlying data being published. That keeps the records permanent while keeping personal data private and erasable, in a manner intended to be consistent with data-protection law. If the migration is undertaken, the detailed design will be set with privacy counsel. Either way, high-frequency mechanics such as DIMO Credit (DCX) issuance and spend stay on a low-cost Layer 2 (currently Polygon), as they do today.

This section authorizes the migration; it does not require it. The $DIMO token contracts are unchanged and remain as listed in [DIP-10](/broken/pages/7d4a20e69a417a06eb1becfa6c0379088b232dea).

### 4. The end of baseline issuance

Baseline issuance ends. The weekly distribution of newly issued $DIMO under [DIP-2](/broken/pages/fc0796d7a412dba32e03108d50485a184a9b5f0c) stops on enactment; the final distribution is the last one executed before this DIP takes effect.

The subsidy did its job. Issuance started at 1,105,000 $DIMO per week at the December 12, 2022 launch and, after three annual 15% cuts, now runs at about **678,600 per week**. Every week it dilutes holders to buy connections the network no longer needs to buy. The network is built. What remains is use: fees paid in $DIMO, and burns only if and when the Foundation chooses to make them (§2).

What changes and what does not:

* **Issuance stops.** No $DIMO is issued as baseline rewards for any week after enactment. The qualification requirements and the points, streak, and level mechanics of DIP-2 retire with it. Connected users get notice through the Review period, the token-holder vote, and the four-day timelock.
* **Everything earned stays earned.** Distributed rewards are untouched, and locked balances keep the lock terms their holders chose. Nothing is retroactive.
* **The undistributed allocation stays frozen.** $DIMO allocated to Baseline Issuance but not yet distributed stays unissued and cannot be spent, burned, or reallocated without a future token-holder vote.

The amendment in §5 implements this.

### 5. Amendment to DIP-2 (Baseline Issuance)

This DIP amends DIP-2, using the formatting convention from [DIP-1 Amendment 1](/broken/pages/5d96bc94cbf4d430afc3b27b6c694133202a9911): green text marks editor notes, <mark style="color:red;">red text marks insertions</mark>, and ~~<mark style="color:red;">red strikethrough marks deletions</mark>~~.

_<mark style="color:green;">// In the DIP-2 Specification, the weekly issuance paragraph (currently beginning "In year one, DIMO will issue 1,105,000 $DIMO per week…") is replaced to read:</mark>_

> ~~<mark style="color:red;">In year one, DIMO will issue 1,105,000 $DIMO per week to all qualified DIMO users at 5 AM UTC each Monday. This issuance amount will automatically decrease by 15% every 52 weeks following the anniversary of the December 12, 2022 mainnet launch, with Baseline Issuance ending in 40 years, unless modified by a future DIP.</mark>~~ <mark style="color:red;">Baseline Issuance is discontinued as of the enactment of DIP-12. No $DIMO is issued as Baseline Issuance for any week after enactment; the final weekly distribution is the last one executed before DIP-12 took effect. Rewards already distributed, including locked balances and their lock terms, are unaffected. $DIMO allocated to Baseline Issuance but not yet distributed remains unissued and may not be used absent a future token-holder vote.</mark>

_<mark style="color:green;">// The qualification requirements in the DIP-2 Specification (the paragraph beginning "To be qualified for rewards, users must…") and the points, streak, and level mechanics of DIP-2 apply only to distributions executed before enactment; they are retired thereafter, and no new qualification requirements are added.</mark>_

_<mark style="color:green;">// For consistency, the corresponding figures in the DIP-2 Abstract ("start at 1,105,000 $DIMO and will decrease 15% each year") are updated to note that Baseline Issuance was discontinued by this DIP.</mark>_

## Implementation

If passed, this DIP takes effect after the four-day timelock. The Foundation will:

{% stepper %}
{% step %}
### Publish the protocol direction

Publish the protocol direction as DIMO's stated focus.
{% endstep %}

{% step %}
### Execute the one-time burn

Execute the one-time 150,000,000 $DIMO burn with on-chain reporting. Further burns are discretionary under §2, on no schedule.
{% endstep %}

{% step %}
### Treat the migration as authorized but unscheduled

Treat the §3 migration as authorized but unscheduled. DCX stays on a low-cost Layer 2 meanwhile.
{% endstep %}

{% step %}
### Implement the DIP-2 amendment

Implement the DIP-2 amendment in §5, ending weekly baseline issuance at enactment while honoring distributed rewards and existing lock terms. The editor will note and link to the amendment in the changelog of DIP-2 once implemented.
{% endstep %}
{% endstepper %}

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-12: The Protocol Direction", no. 12, June 2026. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.

This document is a governance proposal of the DIMO Foundation. It creates no obligations for, and makes no representations on behalf of, Digital Infrastructure Inc. or any other third party. Nothing in this document is investment, legal, or tax advice, and nothing in it is an offer or solicitation to buy or sell any asset.

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
