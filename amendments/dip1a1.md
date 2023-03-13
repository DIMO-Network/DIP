# DIP-1: Amendment 1

> **Headline**: Formalizing a procedure to amend DIPs
>
> **Author**: The DIMO Foundation
>
> **Submitter(s)**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Review (until March 22, 2023 at 12:00 UTC)
>
> **Voting URL**: Pending
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: Level 3

## Abstract

This proposal formalizes the procedure to repeal or enact amendments to DIPs. The voting protocols are the same as normal DIPs, but the result in an alteration of the original DIP. More detail below.

## Motivation

To allow improvement proposals to be revised or repealed without creating unnecessary document clutter and confusion.

## Specification

If passed, this proposal would append the following to the end of the DIP-1 Specification section:&#x20;

\---

### <mark style="color:red;">**Amending & repealing DIPs**</mark>

<mark style="color:red;">After a DIP has been passed, future proposals may amend or repeal that DIP. Such a proposal is subject to the same requirements as a standard DIP. This means that the requirements for proposal submission, voting, and all other specifications still apply. This also includes the requirement to follow the same structural format as any other DIP, complete with a header, abstract, motivation, specification, implementation, copyright, citation, changelog, and disclaimer section.</mark>

<mark style="color:red;">Any proposal amending or repealing a DIP need only amend or repeal the original DIP. In other words, it does not need to make updates to prior amendments.</mark>

#### <mark style="color:red;">If amending a DIP</mark>

<mark style="color:red;">The proposal must clearly specify exactly where and how the DIP should be amended to leave zero ambiguity as to how changes would be implemented in the original document if the proposal were to pass. The amendment proposal should use a red font to denote the text that will be inserted into the original DIP and red font with a strikethrough to denote the text that will be deleted. See</mark> [dip1a1.md](dip1a1.md "mention") <mark style="color:red;">for an example of this formatting.</mark>

<mark style="color:red;">The amendment need not specify the language for the changelog, however the editor must note and link to the amendment in a new changelog entry once implemented.</mark>&#x20;

\---

This proposal would also add a new Status option under the bullet for "Withdrawn" such that the list in DIP-1 would now read:

* _Failed_ - vote concluded and proposal failed to reach majority and/or quorum; ~~<mark style="color:red;">or</mark>~~
* _Withdrawn_ - sponsor(s) withdrew the proposal while it was in the _Review_ stage, prior to voting~~<mark style="color:red;">.</mark>~~<mark style="color:red;">; or</mark>
* <mark style="color:red;">Repealed - proposal had been deployed but was later repealed.</mark>&#x20;

## Implementation

If passed, DIP-1 would be updated as specified above after the four day timelock concludes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, " DIP 1 Amendment 1", February 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Mar 3, 2023: adjusted the date that the proposal is in review from March 3 to March 15. This is to create more time discussion and hopefully the introduction of a fourth proposal related to marketplace issuance that can be voted alongside the three that are currently in review.

Mar 13, 2023: extended the review period from March 15 to March 22. This is to continue to provide more time for discussion and hopefully the introduction of a fourth proposal related to marketplace issuance that can be voted alongside the three that are currently in review.

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
