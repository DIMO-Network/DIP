---
hidden: true
---

# \*\*\*DIP-3 & 10: Amendment 1

> **Headline**: Upgrading billing formulas and streamlining the means of creating DIMO Credits
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

## NOTES: DELETE BEFORE PUBLISHING

Mint DCX using USDC and reward nodes in USDC

$1.25 gets you 50k requests within 30 days (not a calendar month... 30 days...)

DCX = $0.000025. $1.25 gets you 500,000 DCX.

One DCX gets you one query response line. e.g., lat, long, fuel ever 15s for from 12:00 - 12:01pm = 3 signals \* 4 intervals = 12 DCX

Because costs don't scale linearly, and rather increase, there should be a multiplier on DCX cost based on responses in a single query. E.g., (1 + count of items/1000) DCX per item

Webhooks = 100 DCX per event







## Abstract



## Motivation



## Specification

_<mark style="color:green;">// If passed, this proposal would replace the Abstract with:</mark>_



_<mark style="color:green;">// and would replace the Specifications with:</mark>_



_<mark style="color:green;">// and would adjust the specification section of DIP-10 as follows</mark>_

### DIMO Credit (DCX)

_A stable credit pegged to $0.0001 USD that can only be created and purchased with <mark style="color:red;">USDC</mark>_~~_<mark style="color:red;">$DIMO</mark>_~~_. Once DCX is spent, it is burned and cannot be reused. <mark style="color:red;">60% of all USDC collected by minting DCX is automatically converted into $DIMO and burned.</mark>_

## Implementation

If passed, DIP-3 would be updated as specified above after the four day timelock concludes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-3: Amendment 2", November 2024. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Feb 7, 2025: Corrected a typo. 1 DCX has always equalled $0.0001 USD, not $0.001 USD

## Disclaimer <a href="#disclaimer" id="disclaimer"></a>

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.
