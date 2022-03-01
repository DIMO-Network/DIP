> **Author**: [robmsolomon](https://twitter.com/robmsolomon)
> 
> **Status**: Living [passed January, 28 2022 at 0:00 UTC]
> 
> **Headline**: A general procedure for submitting and voting on proposals.
> 
> **Voting Format [URL]**: [[Snapshot]](https://snapshot.org/#/dimo.eth/proposal/0x096a7ee8ebc3bb90c5aab4afa516ab0700aa436c5f4f92c0a7d7fec24457646d)

# Abstract
This document outlines the format for DIMO governance proposals (DIPs), as well as the procedure for deliberating and voting on them. DIPs may be used to allocate tokens from the treasury, delegate authority to [d]Teams, ratify a change to the DIMO logo, or anything else the community may choose to vote on.

This document may be amended at any time by the DAO in a future DIP. As a living document, DIP-1 will be updated to reflect current amendments once future DIPs alter any of the terms of this proposal.

# Motivation
If DIMO is going to be an effective DAO, it must have concise, transparent, and effective proposals; a strong culture of engagement and debate on proposals; a clear and practical voting procedure; and effective follow through. This document seeks to establish the foundation for all of these things.

# Specification
Governance proposals are called DIMO Improvement Proposals (DIP). They are formatted, generated, submitted, deliberated, voted on, and implemented as follows.

#### DIP format 
While not strictly required, it is strongly requested that all DIPs adopt the outline of this document. Specifically, the outline should include:

- **Title**: "DIP[#]: Title Name"
- **Author**: The name of the person or people responsible for creating the proposal. Typically their Discord username.
- **Status**: Options include:
*Draft* - still being worked on
*Review* - actively being reviewed and deliberated;
*Voting* - in the process of being voted on;
*Final* - vote concluded and passed — this document will never be edited and may be superseded by a future DIP;
*Failed* - vote concluded and failed;
*Withdrawn* - sponsor(s) withdrew the proposal while it was in the *Review* stage, prior to voting; or 
*Living* - vote concluded and passed — this document may be edited and will always be kept up-to-date.
*Review* and *Voting* must also specify when that period ends by adding "(until Month Day, Year at 24hr Clock UTC Time)." E.g., **Status**: Review (until January 20th, 2022 at 22:00:00 UTC)
- **Headline**: This should be a brief, one sentence TLDR explaining the proposal.
- **Voting Format [URL]**: The format that will be used by $DIMO holders for voting. Current options include [Snapshot](https://snapshot.org/#/) and [Tally](https://www.withtally.com/). In brackets, next to the format, should be a URL linking to the voting page. For proposals in *Draft* or *Review* status, please write [URL pending].
- **Abstract**: This is a slightly longer 3-5 sentence summary of the proposal.
- **Motivation**: This explains the rationale and goals for the DIP.
- **Specification**: The highly detailed description of the DIP including precise terms, software updates, blockchain transactions and smart contract code, and more. 
- **Implementation**: A description of the implementation procedure that would follow if the DIP were to achieve a successful vote.
- **Copyright**: The copyright terms of the DIP. Please use the same text that is used here.
- **Citation**:  How others should site this DIP in other locations. Please copy the format here and update the author, name, number, date, and url.
- **Changelog**: Any changes made while the DIP is the *Review* stage must be summarized in this section including the date and time of the change. See the bottom of this document for an example.
 

#### Proposal generation & submission
Any person(s) may craft a new DIP. In order for a proposal to be formally added to [gov.dimo.zone](https://gov.dimo.zone/) and submitted for review and voting, the DIP must have the support of 10,000,000 $DIMO worth of voting power. E.g., one person who wields +10,000,000 $DIMO of delegated voting power (aka a Steward, see DIP-2) or ten $DIMO holders who collectively wield +10,000,000 $DIMO in delegated voting power have the ability to formally sponsor and introduce a DIP.

#### Proposal deliberation & withdrawal 
DIPs that have been sponsored and introduced will be posted on [gov.dimo.zone](https://gov.dimo.zone/) and announced in [#📝governance-proposals](https://dao.dimo.zone/). After seven days (168 hours) of deliberation without withdrawal, the DIP goes to a vote.

At any time prior to voting, if the proposals does not maintain the support of at least 10,000,000 $DIMO worth of voting power (because token holders undelegated their tokens from sponsors or sponsors publicly withdraw their support), the proposal status is changed to "Withdrawn". Once the proposal reaches full sponsorship again, if ever, it will go back into *Review*, an announcement will go out in [#📝governance-proposals](https://dao.dimo.zone/), and the seven day deliberation window begins again.

Authors may make edits to a proposal that has already been put into *Review*. Any edits should be summarized in the changelog section. If the edits have major effects on the purpose, interpretation, or implementation of the DIP, it is highly encouraged to reset the seven day voting window and notify the community with an update in [#📝governance-proposals](https://dao.dimo.zone/). Edits should not completely scrap the original proposal and replace it with something new (e.g., edit the proposal to go from a vote on the DIMO logo to a vote on token issuance). To do this, withdraw the DIP and submit a new one.

#### Voting protocol 
After seven days of deliberation, the DIP goes to a vote. Once a vote beings, the voting protocol works as follows.
- **Venue**: [Snapshot](https://snapshot.org/#/) for off-chain voting or [Tally](https://www.withtally.com/) for on-chain voting, as specified in the proposal, depending on the nature of the DIP.
- **Duration**: Voting will be open for seven days (168 hours). Voters may change their votes during the seven day window.
- **Withdrawal**: Once in *Voting*, the proposal may not be withdrawn by the sponsors. It will either pass or fail.
- **Voting options**: The only allowable options for voting are *Approve*, *Reject*, and *Abstain*;
- **Delegation**: $DIMO holders can delegate their voting power to themselves (allowing them to vote directly) or to someone else (without giving up their tokens).
- **Weighting**: Voting is directly proportional to the amount of $DIMO a user has been delegated (by themselves or others);
- **Majority**: A simple majority where the balance of $DIMO representing *Approve* exceeds the balance of $DIMO representing *Reject* is required for a vote to pass.
- **Quorum**: At the close of voting, 40,000,000 $DIMO must be represented in the vote OR there must be enough $DIMO representing *Approve* votes such that the vote would still pass even if every additional vote required to reach quorum were cast as *Reject*. E.g., if 25,000,000 worth of $DIMO votes to approve an initiative, 5,000,000 abstain, and 5,000,000 reject, the vote will still be considered to have reached quorum given that it would have passed had there been another 5,000,000 *Reject* votes.
- **Implementation**: There will be a four day (96 hour) timelock after the vote is completed before execution. This gives various stakeholders the opportunity to make any necessary preparations based on the outcome (e.g., connecting or disconnecting a car, staking or unstaking their tokens, etc.).

To determine the outcome, we only look at the state of the vote at the moment the vote closes. If a vote has majority and quorum at the exact end of seven days, then the status changes to *Final* and the four day timelock prior to execution begins. If a vote does not meet that criteria, the DIP fails to pass and the status changes to "Failed".

# Implementation
If passed, this DIP-1 will be in effect immediately after the four day timelock concludes.

# Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

# Citation

Please cite this document as:

[Rob Solomon](https://twitter.com/robmsolomon), "DIP-1: DIMO Governance Guidelines* , no. 1, January 2022. [Online serial]. Available: [https://github.com/DIMO-Network/DIP]

# Changelog
**Jan 20, 2022 23:27 UTC**: added URL linking to Snapshot or Tally vote to the header. Changed the protocol for making edits (see Proposal deliberation & withdrawal section). TLDR: authors can make edits while in review stage prior to voting. They must add changes to a changelog section (like this one).

**Feb 23, 2022 21:21 UTC**: migrated from Discourse to Github.
