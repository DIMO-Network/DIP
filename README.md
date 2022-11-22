# DIP-1: Governance Guidelines

> **Headline**: A general procedure for submitting and voting on proposals.
>
> **Author**: The DIMO Foundation
>
> **Submitter**: The DIMO Foundation \[0xCED3c922200559128930180d3f0bfFd4d9f4F123]
>
> **Status**: Draft
>
> **Voting URL**: Pending

## Abstract

This document outlines the format for DIMO Improvement Proposals (DIPs), as well as the procedure for deliberating and voting on them. DIPs may be used to vote on anything the community may want to do, from major events like allocating tokens from the treasury, delegating authority, and updating DIMO smart contracts, or minor things like changing the DIMO logo.

This document may be amended at any time by the token holders in a future DIP. As a living document, DIP-1 will be updated to reflect current amendments once future DIPs alter any of the terms of this proposal.

## Motivation

If DIMO is going to be effective, it must have concise, transparent, and effective proposals; a strong culture of engagement and debate on proposals; a clear and practical voting procedure; and effective follow through. This document seeks to establish the foundation for all of these things.

## Specification

Governance proposals are called DIMO Improvement Proposals (DIP). They are formatted, generated, submitted, deliberated, voted on, and implemented as follows.

### **DIP format**

It is required that all DIPs include the following in a format similar to this one. DIPs may add additional sections as needed, so long as they include the following:

* **Title**: "DIP\[#]: Title Name"
* **Headline**: A brief, one sentence TLDR explaining the proposal.
* **Author**: The name of the entity(ies) responsible for creating the proposal. This can be pseudonyms.
* **Submitter**: The name of the entity(ies) responsible for submitting the proposal. This can be pseudonyms. They must include the 0x address of the wallet that held sufficient voting power at the time of submission in brackets (see example above).
*   **Status**: Options include:&#x20;

    * _Draft_ - still being worked on;&#x20;
    * _Voting_ - in the process of being voted on — must also specify when that period ends by adding "(until Month Day, Year at 24hr Clock UTC Time)." E.g., **Status**: Voting (until January 20th, 2023 at 22:00:00 UTC);
    * _Final_ - vote concluded and passed — this document will never be edited and may be superseded by a future DIP;&#x20;
    * _Failed_ - vote concluded and failed;&#x20;
    * _Withdrawn_ - sponsor(s) withdrew the proposal while it was in the _Review_ stage, prior to voting; or&#x20;
    * _Living_ - vote concluded and passed — this document may be edited and will always be kept up-to-date.&#x20;

    _Voting_ must also specify when that period ends by adding "(until Month Day, Year at 24hr Clock UTC Time)." E.g., **Status**: Voting (until January 20th, 2022 at 22:00:00 UTC)
* **Voting URL**: A link to the vote on [Snapshot](https://snapshot.org/#/dimo.eth) or [Tally](https://www.tally.xyz/gov/eip155:137:0xD203e37D96cC0b9b7Dc00fC3fDfcf1b1A2E8c547). For proposals in _Draft_ status, write "Pending".
* **Abstract**: This is a slightly longer 3-5 sentence summary of the proposal.
* **Motivation**: This explains the rationale and goals for the DIP.
* **Specification**: The highly detailed description of the DIP including precise terms, protocol updates, blockchain transactions and smart contract code that will be executed with comments, and more.
* **Implementation**: A description of the implementation procedure that would follow if the DIP achieves a successful vote.
* **Copyright**: The copyright terms of the DIP, which must say "Copyright and related rights waived via [CC0"](https://creativecommons.org/publicdomain/zero/1.0)
* **Citation**: How others should site this DIP in other locations. Please copy the format here and update the author, name, number, date, and url.
* **Changelog**: Any changes made while the DIP is the _Review_ stage must be summarized in this section including the date and time of the change. See the bottom of this document for an example.

### **Proposal generation & submission**

Any person(s) may craft a new DIP. In order for a proposal to be formally added to the [DIP Repo](https://github.com/DIMO-Network/DIP) and submitted for review and voting, the DIP must have the support of 5,000,000 $DIMO worth of voting power. For example, one person who wields 5,000,000 $DIMO of delegated voting power or five $DIMO holders who each represent 1,000,000 $DIMO in delegated voting power have the ability to formally sponsor and introduce a DIP.&#x20;

Due to current technical limitations, the DIMO Foundation must assist in posting DIPs that rely on more than one sponsor to reach the threshold. Email support@dimo.zone for help.

### **Proposal deliberation & withdrawal**

DIPs that have been sponsored and introduced will be posted in the [DIP Repo](https://github.com/DIMO-Network/DIP) and announced in [#📣annoucements](https://dao.dimo.zone/). After seven days (168 hours) of deliberation without withdrawal, the DIP goes to a vote.

At any time prior to voting, if the proposals does not maintain the support of at least 5,000,000 $DIMO worth of voting power (because token holders undelegated their tokens from sponsors or sponsors publicly withdraw their support), the proposal status is changed to "Withdrawn". Once the proposal reaches full sponsorship again, if ever, it will go back into _Review_, an announcement will go out in [#📣annoucements](https://dao.dimo.zone/), and the seven day deliberation window begins again.

Authors may make edits to a proposal that has already been put into _Review_. Any edits should be summarized in the changelog section. If the edits have major effects on the purpose, interpretation, or implementation of the DIP, it is highly encouraged to reset the seven day voting window and notify the community with an update in [#📣annoucements](https://dao.dimo.zone/). Edits should not completely scrap the original proposal and replace it with something new (e.g., edit the proposal to go from a vote on the DIMO logo to a vote on token issuance). To do this, withdraw the DIP and submit a new one.

### **Voting protocol**

After seven days of deliberation, the DIP goes to a vote. Once a vote beings, the voting protocol works as follows.

**Definitions**

* **Circulating Supply**: Equals the total supply of $DIMO minus the amount held by the Foundation as treasury or for baseline issuance.
* **Voting Formats**: The only allowable formats are:&#x20;
  * Basic Voting: the only voting options are Approve, Reject, and Abstain and the vote is either approved or rejected at the end of the voting period. These an be on-chain votes on Tally or off-chain polls on Snapshot.
  * Ranked Choice: an instant runoff method whereby users rank their choices in order. If any option is ranked first by the required majority of voters, that options wins. If no option reaches majority, the option that received the fewest top rank choices by voters is eliminated and the nullified votes for that option are redistributed to each voter's second choice. This process repeats until one option reaches the required majority (and that options wins) or until there are two options left that both fail to reach the majority (e.g., if required majority is 60% and options 1 and 2 have 50% each and there is no winner). These votes must be done as off-chain poles on Snapshot.
  * Multiple Selection: voters are able to select multiple options, and each option that achieves the required majority is accepted. For example, this may be used to elect multiple members to a council. These votes must be done as off-chain poles on Snapshot.
* **Quorum**: This is the amount tokens required to participate in a vote for it to be considered valid. A vote that falls short on participation may still be considered valid if there are enough votes for Approve (in Basic Voting) or the top choice (in Rank Choice) such that majority would still be achieved even if every additional vote required to reach quorum were cast as Reject (in Basic Voting) or for the alternate choice (in Rank Choice).&#x20;

**Terms**

* **Venue**: [Snapshot](https://snapshot.org/#/dimo.eth) for off-chain polling or [Tally](https://www.tally.xyz/gov/eip155:137:0xD203e37D96cC0b9b7Dc00fC3fDfcf1b1A2E8c547) for on-chain voting, as specified in the proposal, depending on the nature of the DIP.
* **Duration**: Voting will be open for seven days (168 hours). Voters may change their votes during the seven day window.
* **Withdrawal**: Once in _Voting_, the proposal may not be withdrawn by the sponsors. It will either pass or fail.
* **Delegation**: $DIMO holders can delegate their voting power to themselves (allowing them to vote directly) or to someone else without having to transfer their tokens. To do this, click [here](https://www.tally.xyz/gov/eip155:137:0xD203e37D96cC0b9b7Dc00fC3fDfcf1b1A2E8c547), connect your wallet, and click "Delegate Tokens". Then enter the 0x address of the person you'd like to delegate your tokens to.  You remain in control of your $DIMO and can revoke or redelegate your tokens at any times. This action will require Matic tokens on the Polygon blockchain.
* **Weighting**: Voting is directly proportional to the amount of $DIMO a user has been delegated (by themselves or others);
* **Formats, Majority, and Quorum**:
  *   **Level 3 Votes**: For highly impactful votes that entail minting or burning tokens; altering governance; altering issuance; disposing or selling core intellectual property of the Foundation; transferring or committing over 15,000,000 $DIMO; or other very meaningful decisions as may be determined by the DIMO Foundation:

      Majority = 70%

      Quorum = 15% of circulating supply\
      Acceptable Voting Formats = Basic Voting, Ranked Choice
  *   **Level 2 Votes**: For somewhat impactful votes that entail transferring or committing between 5,000,000 to 15,000,000 $DIMO; removing a DIMO Foundation director; altering the DIMO Foundation Bylaws; or other meaningful decisions as may be determined by the DIMO Foundation:

      Majority = 60%

      Quorum = 10% of circulating supply\
      Acceptable Voting Formats = Basic Voting, Ranked Choice
  *   **Level 1 Votes**: For other votes that are less impactful in nature than those listed above, such as issuing non-exclusive licenses to core intellectual property that do not inhibit the DIMO network; transferring under 5,000,000 $DIMO (often for grants); delegating other resources and authority to individuals or groups who are helping to build $DIMO (e.g., recognizing a new DIMO Integrations team and granting it the right to issue licenses to device manufacturers):

      Majority = 50%

      Quorum = 5% of circulating supply\
      Acceptable Voting Formats = Basic Voting, Ranked Choice, Multiple Selection
* **Implementation**: There will be a four day (96 hour) timelock after the vote is completed before execution. This gives various stakeholders the opportunity to make any necessary preparations based on the outcome (e.g., connecting or disconnecting a car, staking or unstaking their tokens, etc.).
* **Invalid Votes**: Votes may not be enacted if doing so will result in the contravention of Cayman Islands laws or regulations, if it is non-compliant with the DIMO Foundation Memorandum & Articles and Bylaws, or cause clear harm to the Foundation. Transfers of $DIMO may be contingent on the recipient completing a Know Your Customer (KYC) process in the case of large grants.

To determine the outcome, we only look at the state of the vote at the moment the vote closes. If a vote has majority and quorum at the exact end of seven days, then the status changes to _Final_ and the four day timelock prior to execution begins. If a vote does not meet that criteria, the DIP fails to pass and the status changes to "Failed".

## Implementation

If passed, this DIP-1 will be in effect immediately after the four day timelock concludes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-1: DIMO Governance Guidelines", no. 1, November 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]
