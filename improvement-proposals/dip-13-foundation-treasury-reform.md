# DIP-13: Foundation Treasury Reform

> **Headline**: End the Foundation's free-spending treasury authority by putting its budget under token-holder approval and commit the Foundation to treating every builder on the protocol the same
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Approved
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/s:dimo.eth/proposal/0xb3698d32abae86a6318c30c97f4a07ed0021dd64913ed307dfcaec68026dfe6a)
>
> **Discussion Forum**: [Discord](https://chat.dimo.org/) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

Under [DIP-6](/broken/pages/9d8c6e299a8cd6f063a54591db512fafc5faf7b6), the DIMO Foundation may sell $DIMO from the treasury without per-sale governance approval and run its operating plan without fixed category caps. This DIP ends that. It replaces those provisions with a simple rule: the Foundation spends only under a budget token holders have approved, with narrow exceptions for a transition window, emergencies, and pre-existing commitments (amending DIP-6). It also commits the Foundation to treating every builder on the protocol the same. That neutrality now extends to Digital Infrastructure Inc., the independent company that first developed DIMO (the labs entity), which builds on DIMO on the same terms as everyone else: no treasury funding and no preferential terms. This DIP imposes no obligations on the labs entity itself. It is a companion to [DIP-12](/broken/pages/bcb881b525d76f78dddf6ac9a34b6d48d767e1d2) (The Protocol Direction) but stands on its own and takes effect whether or not DIP-12 passes.

## Motivation

DIP-6's flexibility helped the Foundation move fast in the bootstrap years. But a protocol that asks token holders to treat the treasury as theirs should not leave its outflows to one entity's discretion. A budget approved by the people the treasury belongs to serves holders and the Foundation alike.

Neutrality serves the same end. Digital Infrastructure Inc. took DIMO from an idea to a network of 200,000 vehicles, and a mature protocol should not lean on any single company, including the one that built it. A steward that funds no builder and favors no builder stays neutral among all of them, and treasury decisions stay clear of product decisions. What remains is a Foundation that spends only by token-holder approval and a labs entity building on the protocol on the same commercial footing as everyone else.

## Specification

### 1. Treasury reform: ending unilateral Foundation spending

[DIP-6](/broken/pages/9d8c6e299a8cd6f063a54591db512fafc5faf7b6) as amended lets the Foundation sell $DIMO from treasury "without per-sale governance approval," apply the proceeds to a broad list of uses including investments and acquisitions, and run an internal operating plan "without fixed category caps." Whatever its merits during bootstrapping, that authority is broader than a maturing protocol should carry, and this DIP replaces it. Once the transition below runs out, the Foundation spends only what token holders have approved. Any budget covers the Foundation's own protocol operations only; consistent with §2, none includes a line item for the labs entity.

The rules:

* **A budget before spending.** To spend from the treasury, the Foundation must first have an operating budget approved by token-holder vote under [DIP-1](/broken/pages/086de18edcab5cb137043b049dc07e133a35bf81). A budget covers no more than twelve months and states planned spending by category in USD equivalent and the maximum $DIMO that may be sold in the period. A budget vote is a resource allocation and carries no less than a Level 2 vote. Nothing requires the Foundation to spend: a Foundation that seeks no budget simply does not spend.
* **No spending outside it.** The Foundation may not sell $DIMO from treasury, nor spend or transfer treasury assets, except under an approved budget, another token-holder vote, the transition allowance below, binding commitments entered into before this DIP takes effect, or an emergency allowance of up to **$1,000,000 USD equivalent per calendar year** for genuine emergencies (security incidents, legal or compliance deadlines), disclosed publicly within 30 days of use. Material changes to an approved budget require an amended vote, and unused authorization expires at the end of its period. Treasury movements in $DIMO are publicly verifiable on-chain in any case.
* **Protocol rules are not discretionary spending.** Payments that run by rule under an adopted DIP, such as the 40% node share under [DIP-3](/broken/pages/2e71d0fa926050bcbb64d35bac75de825d1edead), sit outside the budget; the Foundation has no discretion over them. The same goes for the burns authorized by [DIP-12](/broken/pages/bcb881b525d76f78dddf6ac9a34b6d48d767e1d2), if enacted, since a burn pays no counterparty and benefits every holder ratably. Network fees the protocol keeps and does not burn are treasury assets like any other.
* **Transition.** For no more than 180 days after enactment, the Foundation may operate at a monthly run rate no higher than its trailing twelve-month average and may honor existing commitments. When that window ends, discretionary spending pauses, except the emergency allowance and pre-existing binding commitments, unless and until token holders have approved a budget.

This changes who authorizes spending, not what the Foundation is. Its DIP-6 role continues: holding the protocol's contracts and IP and acting as governance directs, with any spending under a budget its token holders approve. The amendment in §3 implements this.

### 2. A neutral Foundation: every builder on the same terms

The Foundation is neutral among the builders that use the protocol, and that neutrality extends to Digital Infrastructure Inc., the company that first developed DIMO (the labs entity). The labs entity is an independent, separately owned business. It is not a party to this DIP, and nothing here creates obligations for it or speaks on its behalf. What this DIP binds is the Foundation: no funding to the labs entity (no grants, subsidies, investments, or guaranteed contracts) and no preferential fee terms. The labs entity builds on DIMO on the same terms as every other builder. Anything the protocol needs, the Foundation procures from qualified vendors at arm's length under an approved budget. The licenses the labs entity already holds ([DLP-3](/broken/pages/473e766f66a92c642cd6caa8365855141f3f9a61), [DLP-4](/broken/pages/404bb59ba896a6213fc36d56fcbd1cd67e661fa1)) and the IP license noted in DIP-6 continue unchanged.

### 3. Amendment to DIP-6 (The DIMO Foundation)

This DIP amends DIP-6, using the formatting convention from [DIP-1 Amendment 1](/broken/pages/5d96bc94cbf4d430afc3b27b6c694133202a9911): green text marks editor notes, <mark style="color:red;">red text marks insertions</mark>, and ~~<mark style="color:red;">red strikethrough marks deletions</mark>~~.

_<mark style="color:green;">// In the DIP-6 Specification, under "Financial Plan & Ask", clause (a) Resources is replaced to read:</mark>_

> ~~<mark style="color:red;">(a) Resources. The Foundation may sell $DIMO from treasury without per-sale governance approval to fund operations, liquidity, strategic partnerships, and investments that materially advance the protocol. Sales may be conducted via programmatic execution, RFQ/OTC transactions, auctions, or strategic placements.</mark>~~ <mark style="color:red;">(a) Resources. The Foundation may sell $DIMO from treasury only as authorized by an approved operating budget under clause (c) or by another token-holder vote. Authorized sales may be conducted via programmatic execution, RFQ/OTC transactions, auctions, or strategic placements.</mark>

_<mark style="color:green;">// In clause (b) Use of Funds, the following sentence is inserted at the beginning of the clause; the remainder of the clause, including the requirement that all expenditures, contracts, and treasury actions primarily benefit the DIMO protocol and $DIMO token, is unchanged:</mark>_

> <mark style="color:red;">All applications of funds under this clause, including investments, acquisitions, market maker loans, liquidity programs, and reserve rebalancing, are subject to an approved operating budget under clause (c).</mark>

_<mark style="color:green;">// Clause (c) Operating Envelope is replaced in its entirety to read:</mark>_

> ~~<mark style="color:red;">(c) Operating Envelope. The Foundation may adopt and revise an internal annual operating plan (OPEX + program spend) without fixed category caps.</mark>~~ <mark style="color:red;">(c) Operating Budget. The Foundation may not sell $DIMO from treasury, nor spend or transfer treasury assets, except under an operating budget approved by token-holder vote under DIP-1, another token-holder vote, binding commitments entered into before DIP-13 took effect, a transition allowance running no more than 180 days after DIP-13 takes effect (at a monthly run rate no higher than the trailing twelve-month average), or an emergency allowance of up to $1,000,000 USD equivalent per calendar year for security incidents and legal or compliance deadlines, disclosed publicly within 30 days of use. A budget covers a period of no more than twelve months and states total planned spending (OPEX and program spend) by category in USD equivalent and the maximum $DIMO that may be sold from treasury during the period; nothing requires the Foundation to seek a budget or to spend. Material changes to an approved budget require an amended budget vote; unused authorization expires at the end of its period. Payments that run by rule under an adopted DIP (including node payments under DIP-3) are not discretionary spending under this clause, and burns of treasury $DIMO, which pay no counterparty, require no budget authorization.</mark>

_<mark style="color:green;">// At the end of the "Financial Plan & Ask" section, the following paragraph is added:</mark>_

> <mark style="color:red;">Notwithstanding anything else in this DIP or its amendments, the Foundation may not sell, loan, spend, or transfer treasury assets without token-holder approval except as provided in clause (c). Any prior authorization to the contrary is revoked to the extent of the conflict.</mark>

_<mark style="color:green;">// The Foundation's administrative role over smart contracts, its authority to execute legal contracts, its IP provisions (including the existing IP license held by Digital Infrastructure Inc.), and its commitments are unchanged by this amendment.</mark>_

## Implementation

If passed, this DIP takes effect after the four-day timelock. The Foundation will:

{% stepper %}
{% step %}
### Implement the DIP-6 amendment

Implement the DIP-6 amendment in §3.
{% endstep %}

{% step %}
### Operate under transition rules

Operate under the §1 transition rules, seeking budget approval before any spending beyond them.
{% endstep %}
{% endstepper %}

The editor will note and link to the amendment in the changelog of DIP-6 once implemented.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-13: Foundation Treasury Reform", no. 13, July 2026. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.

This document is a governance proposal of the DIMO Foundation. It creates no obligations for, and makes no representations on behalf of, Digital Infrastructure Inc. or any other third party. Nothing in this document is investment, legal, or tax advice, and nothing in it is an offer or solicitation to buy or sell any asset.

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
