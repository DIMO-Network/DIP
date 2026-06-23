# DIP-12: The Business Direction

> **Headline**: Put every vehicle on-chain as a verifiable asset, focus DIMO on the business revenue that unlocks, route that revenue back to $DIMO through a rules-based fee burn, move DIMO's session infrastructure (vehicle identity and attestations) onto Ethereum, and tighten baseline issuance to reward only real, verified vehicles
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

DIMO's founding belief is that a vehicle is one of the most valuable assets a person or business owns, and that it should live on-chain, with a verifiable identity and an owner-controlled record of its history and condition. This proposal sets DIMO's new direction. After several years running a consumer rewards model, DIMO found its real market in businesses: fleet and rental operators, OEM captive finance, tolling, and insurance companies that pay real money for vehicle session infrastructure (digital keys, scoped telemetry, spend controls, and verifiable attestations). This DIP makes four changes to match governance and tokenomics to that. First, it makes serving businesses DIMO's primary focus. Second, it links the $DIMO token to network use through a transparent, rules-based fee burn paid for by network fees, and burns 150,000,000 $DIMO from the treasury to bring the Foundation under 20% of the supply. Third, it moves DIMO's session infrastructure (vehicle identity, attestations, and consent records) onto Ethereum, the neutral, well-secured chain where the $DIMO token has always lived. Fourth, it reforms baseline issuance so rewards flow only to vehicles that prove ownership and are actually in use (amending [DIP-2](../improvement-proposals/dip2.md)).

## Motivation

DIMO's original [Baseline Issuance](../improvement-proposals/dip2.md) model paid drivers newly issued $DIMO for connecting a car and sending data. It did one thing well: it grew the network past 200,000 connected vehicles across four continents. But it did not build a durable protocol. It produced a lot of low-value data, drew in dormant and low-quality connections that existed mainly to farm rewards, and diluted token holders every week without creating demand to offset the new supply. The token's value had little to do with any real economic activity.

DIMO's real customers turned out to be businesses that use vehicles to make money. They mostly came inbound, not through outbound sales: fleet and rental operators replacing five disconnected tools with one integration; captive finance lenders who finance a computer on wheels but only see it once a quarter; tolling and insurance companies that need signed, tamper-proof vehicle data. These customers pay in dollars, on recurring contracts, today.

That points to a clear mandate. DIMO should orient the protocol, the treasury, and the token around real network usage instead of inflationary rewards. The token's value should track how much the network is used, rather than a weekly subsidy paid to bootstrap a network that is now largely built. This DIP makes that explicit and changes the tokenomics to match.

## Specification

### Vision: a vehicle is an asset that belongs on-chain

A vehicle is, for most people and most businesses, one of the largest assets they will ever own or operate. It gets bought and sold, financed, leased, insured, and rented. Yet it lives almost entirely off-chain. Its title sits on paper in a drawer. Its history is scattered across dealerships and DMV records. Its real condition stays unknown until something breaks. Its ownership and use can't be verified by anyone who isn't standing next to it. A multi-trillion-dollar asset class is economically illegible.

DIMO wants to change that. Every vehicle should have a real on-chain presence: a verifiable identity tied to its VIN, an owner-controlled record of where it has been and what condition it is in, and signed attestations (VIN, odometer, position, health) that any third party can trust without having to trust DIMO. A vehicle on-chain this way becomes something a lender can mark to truth in real time, something a fleet can grant and revoke access to in a single transaction, and an asset whose data the owner, not the manufacturer, decides to monetize. On-chain does not mean public, and it does not mean giving up control: the owner holds the keys, and any consent is explicit and revocable.

Serving businesses is how that vision pays for itself. Businesses are the first to pay real money for vehicles that are legible on-chain, because verified identity, history, and condition are exactly what lenders, insurers, fleets, and OEMs need. Their spending funds the protocol, and through the fee burn below it reduces token supply. Every vehicle DIMO brings on-chain makes the network, and the asset class it stands for, more valuable.

### 1. The new direction

Going forward, DIMO's primary purpose is to be the infrastructure for vehicle sessions: the layer that lets a business grant, scope, meter, and revoke access to a vehicle and its data, with cryptographically verifiable records of what happened. Put plainly, every time someone uses a vehicle they don't own, whether a rental, a car-share, a financed lease, or a fleet assignment, that is a session, and a session needs infrastructure: identity, consent, data, payments, and an audit trail. DIMO already provides that across more than 50 vehicle brands through a single integration.

The goal is to serve the people and businesses that depend on a vehicle to make a living: fleet and rental operators, Turo hosts, Uber and Lyft drivers, delivery and service companies, owner-operators. For them a car is a working asset, not a lifestyle purchase. Keeping it insured, maintained, and on the road is the difference between a good month and a bad one. This is where DIMO's automation earns its keep. One integration handles access, tracks condition, proves mileage, and settles payments, in place of five separate tools and a spreadsheet. The reformed baseline issuance in §4 aims rewards at these vehicles: the ones that are insured, documented, and actually driven for work.

DIMO will keep operating the open protocol and the consumer-facing network. That connected-vehicle base is a real asset and stays the foundation of the data marketplace. What changes is the monetization and token model. The protocol's economics now center on business customers who pay for sessions, data, and attestations, and on routing that revenue back to the token. The Foundation and contributors will prioritize the products, partnerships, and compliance work that serve those businesses, including the data-access regulation now emerging, in line with this direction.

This is a direction, not a reversal. Nothing here removes the open, permissionless nature of the protocol, or a user's ownership and control of their own vehicle and data.

### 2. Token value capture: a rules-based fee burn

$DIMO is the token used to pay for the DIMO network. The protocol ties the token's value to that use with one fixed rule: a set share of the network fees collected in $DIMO is burned every quarter. This is a supply mechanism, the same idea as a network that burns part of its fees. It is not a payment to holders, and it gives no one a claim on the Foundation's revenue or profit.

- **What gets burned.** Each quarter the protocol burns **no less than 50% of the protocol's share of the $DIMO collected as network fees** — principally the Foundation's 60% protocol share of the $DIMO paid for DIMO Credit (DCX) under [DIP-3](../improvement-proposals/dip3.md), plus any other fees actually paid to the protocol in $DIMO. The 40% of the DIP-3 pool paid to nodes is untouched, and fees invoiced in fiat or stablecoins are not a source of burns. The share is set by token-holder vote and runs by rule, not at the Foundation's discretion.
- **Cadence.** Burns happen at least **quarterly**.
- **How.** The $DIMO is sent to a public burn address on **Ethereum**, with supply on the other chains reconciled through the canonical bridges in [DIP-10](../improvement-proposals/dip10.md).
- **Transparency.** Every burn is posted with its on-chain transaction and the fee figure behind it, so anyone can check the math.

**One-time supply decentralization.** When this passes, the Foundation will burn a fixed **150,000,000 $DIMO** from its treasury, drawn from holdings not needed for operating runway so that operations under [DIP-6](../improvement-proposals/dip6.md) are unaffected. As of this proposal the Foundation holds about 300,000,000 $DIMO, roughly 30% of the 1,000,000,000 total supply. Because a burn reduces both the Foundation's holdings and the total supply, this takes the Foundation to about 150,000,000 of roughly 850,000,000 remaining — about **17.6%**, below the 20% line. This is one step toward the decentralization the CLARITY Act expects of a "mature blockchain system," which takes more than token distribution: no issuer or insider group holding 20% or more of the tokens or directing 20% or more of the votes, and no party able to unilaterally control or change the network. To the extent other insiders also hold $DIMO, the Foundation will work to keep the combined insider holding below 20% as well. Today the Foundation still holds administrative (upgrade) authority over certain protocol contracts under DIP-6; reducing and ultimately removing that unilateral control in favor of on-chain governance is a separate step the Foundation commits to pursue through future DIPs. This DIP does not by itself make the network "mature."

This runs under the treasury authority the Foundation already has from [DIP-6](../improvement-proposals/dip6.md); it sets how that authority is used and changes nothing else in DIP-6. The point is simple: the more the network is used, the more $DIMO is burned.

**On classification.** $DIMO is built to work as a digital commodity. Its value comes from using and running the network, not from any promise of profit from the Foundation's work. The fee burn is a protocol rule, not a dividend, a revenue or profit share, or a yield, and it gives holders no claim on the Foundation or anyone else. These choices are designed to move $DIMO toward the CLARITY Act's framework for a "digital commodity," and, in time and with the further steps described in §2, a "mature blockchain system." That Act isn't law yet and its wording may change, so the Foundation will follow the law as it lands and adjust the mechanics if needed to keep $DIMO on the digital-commodity side. Nothing here promises any price, profit, or return.

### 3. Bring the session infrastructure to Ethereum

The $DIMO token has always lived on Ethereum (and is bridged to Base, Optimism, and Polygon, per [DIP-10](../improvement-proposals/dip10.md)). What this DIP moves is the **session infrastructure** built on DIMO: vehicle identity, attestations (VIN, odometer, position, health), consent records, and the registry that ties them together. These records move to **Ethereum mainnet**.

They are the records that make a vehicle a verifiable on-chain asset. Putting them on Ethereum, the most neutral, secure, and permanent chain, lets a lender, insurer, or buyer trust a vehicle's identity and history without trusting DIMO, and keeps those records durable for the life of the vehicle. A vehicle is a valuable, long-lived asset, and its record belongs on the chain built to hold value rather than on whichever chain is cheapest in a given year.

What goes on Ethereum is the proof, not the personal data. A vehicle's VIN, registration, insurance, and detailed history stay off-chain, encrypted and under the owner's control, where they can be corrected or deleted. What lives on mainnet are commitments and signed proofs: a third party can confirm that an attestation is genuine, or that a claim holds (a valid VIN, an odometer reading, a clean title), without the underlying data ever being published. This keeps the records trustworthy and permanent while keeping personal data private and erasable, consistent with data-protection law. The detailed design will be set with privacy counsel.

High-frequency, low-value mechanics that are not part of that record, such as DIMO Credit (DCX) issuance and spend and weekly reward distribution, continue on a low-cost Layer 2 (currently Polygon), as they do today. The Foundation and contributors will sequence the migration to keep it safe and avoid disrupting users.

This migration is authorized by this DIP. It does not change the $DIMO token contracts, which remain as listed in [DIP-10](../improvement-proposals/dip10.md).

### 4. Baseline issuance reform

Baseline issuance is reformed so that newly issued $DIMO rewards only vehicles that are verifiably owned and actually in use, and so that the amount issued is sharply reduced in favor of value capture through §2.

The substance of the reform:

- **Higher bar to qualify.** In addition to the existing requirements, a vehicle must (a) have valid **ownership documentation** on file (vehicle registration and proof of insurance; an on-chain VIN attestation is encouraged and may substitute as the protocol matures), and (b) meet a **minimum weekly mileage** threshold (at least fifty miles per week), which shows the vehicle is actually driven and not parked to farm rewards.
- **Sharply reduced issuance.** The weekly baseline issuance pool is cut to **200,000 $DIMO per week**, and the automatic decay schedule is retired. Issuance began at 1,105,000 per week at the December 12, 2022 launch and, after three annual 15% reductions, currently runs at about **678,600 per week** — so this is roughly a 70% cut from the current level (about 82% below the original). Value that previously flowed to inflation now reaches holders through the fee burn in §2.
- **Transition.** Existing connected vehicles keep earning under the current rules for a grace period of no less than 90 days after enactment, and their streak and lock levels are preserved through that window. Within it, owners supply ownership documentation and meet the minimum weekly mileage; after it, the new requirements in this section apply to every vehicle. The reduced weekly issuance and the one-time burn take effect on enactment. No current participant is cut off without notice.
- **Privacy.** The registration and insurance used to qualify are held off-chain and never published. Only a proof of eligibility, and where used a VIN commitment rather than the VIN itself, is recorded on-chain, and a vehicle's documents can be deleted on request (see §3).

This is implemented through the amendment to DIP-2 in §5 below. The points, streak, and lock mechanics of DIP-2 are unchanged.

### 5. Amendment to DIP-2 (Baseline Issuance)

This DIP amends DIP-2, using the formatting convention from [DIP-1 Amendment 1](../amendments/dip1a1.md): green text marks editor notes, <mark style="color:red;">red text marks insertions</mark>, and ~~<mark style="color:red;">red strikethrough marks deletions</mark>~~.

_<mark style="color:green;">// In the DIP-2 Specification, the weekly issuance paragraph (currently beginning "In year one, DIMO will issue 1,105,000 $DIMO per week…") is replaced to read:</mark>_

> ~~<mark style="color:red;">In year one, DIMO will issue 1,105,000 $DIMO per week to all qualified DIMO users at 5 AM UTC each Monday. This issuance amount will automatically decrease by 15% every 52 weeks following the anniversary of the December 12, 2022 mainnet launch, with Baseline Issuance ending in 40 years, unless modified by a future DIP.</mark>~~ <mark style="color:red;">DIMO will issue 200,000 $DIMO per week to all qualified DIMO users at 5 AM UTC each Monday. This is a flat weekly amount; the prior automatic 15%-per-year decay schedule is retired. The amount may be modified by a future DIP.</mark>

_<mark style="color:green;">// In the DIP-2 Specification, the qualification paragraph (currently beginning "To be qualified for rewards, users must…") is amended to add the bolded requirements:</mark>_

> To be qualified for rewards, users must: download an authorized DIMO client; add their vehicle and establish an integration; complete vehicle minting and device pairing on-chain as applicable; <mark style="color:red;">provide and maintain valid ownership documentation for the vehicle (current vehicle registration and proof of insurance, held off-chain and not published, with only a proof of eligibility recorded on-chain), where an on-chain VIN attestation (a commitment rather than the raw VIN) is encouraged and may satisfy this requirement as the protocol matures; drive the vehicle at least fifty (50) miles per week;</mark> and transmit data each week. As of the time of this writing, [DIMO Mobile](http://onelink.to/dimo) is the only authorized client.

_<mark style="color:green;">// For consistency, the corresponding figures in the DIP-2 Abstract ("start at 1,105,000 $DIMO and will decrease 15% each year") are updated to reflect the flat 200,000-per-week amount and the retirement of the decay schedule.</mark>_

## Implementation

If passed, this DIP takes effect after the four-day timelock concludes. The Foundation will: (i) publish the business direction as DIMO's stated focus; (ii) execute the one-time 150,000,000 $DIMO decentralization burn, and begin the quarterly fee burn, with the first quarterly execution in the first full quarter after enactment and on-chain reporting thereafter; (iii) migrate the session infrastructure (vehicle identity, attestations, and consent records) to Ethereum mainnet, while keeping DCX and reward distribution on a low-cost Layer 2; and (iv) implement the DIP-2 amendment in §5, including the necessary updates to the rewards eligibility logic operated on behalf of the Foundation. The editor will note and link to the amendment in the changelog of DIP-2 once implemented.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-12: The Business Direction", no. 12, June 2026. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Jun 23, 2026: drafted and placed into Review.

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
