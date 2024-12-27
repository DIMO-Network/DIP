# DIP-1: Governance Guidelines



> **Headline**: A general procedure for submitting and voting on proposals
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
> **Vote Type**: [Level 3](dip1.md#voting-protocol)

## Abstract

This document outlines the procedure for deliberating and voting on DIMO Improvement Proposals (DIPs) and DIMO License Proposals (DLPs).&#x20;

DIPs may be used to vote on anything the community may want to do, from major events like allocating tokens from the treasury, delegating authority, and updating DIMO smart contracts, or minor things like changing the DIMO logo.

This process may be amended at any time by the token holders in a future DIP.

## Motivation

If DIMO is going to be effective, it must have concise, transparent, and effective proposals; a strong culture of engagement and debate on proposals; a clear and practical voting procedure; and effective follow through. This document seeks to establish the foundation for all of these things.

## Specification

Governance proposals are called DIMO Improvement Proposals (DIP) and proposals to issue any type of license are called DIMO License Proposals (DLP) . They are formatted, generated, submitted, deliberated, voted on, and implemented as follows.

### **Format**

It is required that all DIPs and DLPs include the following in a format similar to this one (see the [Templates folder](https://github.com/DIMO-Network/DIP/tree/main/templates)). DIPs and DLPs may add additional sections as needed, so long as they include the following:

* **Title**: "\[DIP or DLP] \[#]: Title Name"
* **Header:**
  * **Headline**: A brief, one sentence TLDR explaining the proposal.
  * **Author**: The name of the entity(ies) responsible for creating the proposal. This can be pseudonyms.
  * **Submitter**: The name of the entity(ies) responsible for submitting the proposal. This can be pseudonyms. They must include the 0x address of the wallet that held sufficient voting power at the time of submission in brackets (see example above).
  *   **Status**: Options include:&#x20;

      * _Review_ - for review and discussion by community (the author may still make changes);&#x20;
      * _Voting_ - in the process of being voted on;
      * _Approved_ - vote concluded and proposal passed, but not implemented yet;&#x20;
      * _Deployed -_ vote concluded and proposal passed and implemented;
      * _Failed_ - vote concluded and proposal failed to reach majority and/or quorum; or
      * _Withdrawn_ - sponsor(s) withdrew the proposal while it was in the _Review_ stage, prior to voting.

      _Review_ and _Voting_ must also specify when that period ends by adding "(until Month Day, Year at 24hr Clock UTC Time)." E.g., **Status**: Voting (until January 20th, 2022 at 22:00:00 UTC).
  * **Voting URL**: A link to the vote on [Snapshot](https://snapshot.org/#/dimo.eth). For proposals in _Review_ status, write "Pending".
  * **Discussion Forum**: Where the community is encouraged to discuse the proposal.
  * **Vote Type**: Either a vote level 1, 2, or 3. See types below, under **Terms**.
* **Abstract**: This is a slightly longer 3-5 sentence summary of the proposal.
* **Motivation**: This explains the rationale and goals for the DIP or DLP.
* **Specification**: The highly detailed description of the DIP or DLP including precise terms, protocol updates, blockchain transactions and smart contract code that will be executed with comments, and more.
* **Implementation**: A description of the implementation procedure that would follow if the DIP or DLP achieves a successful vote.
* **Copyright**: The copyright terms of the DIP or DLP, which must say "Copyright and related rights waived via [CC0"](https://creativecommons.org/publicdomain/zero/1.0)
* **Citation**: How others should site this DIP or DLP in other locations. Please copy the format here and update the author, name, number, date, and url.
* **Changelog**: Any changes made while the DIP or DLP is the _Review_ stage must be summarized in this section including the date and time of the change.

### **Proposal generation & submission**

Any person(s) may craft a new DIP or DLP. In order for a proposal to be formally added to the [Repo](https://github.com/DIMO-Network/DIP) and submitted for review and voting, the DIP or DLP must have the support of 5,000,000 $DIMO worth of voting power. For example, one person who wields 5,000,000 $DIMO of delegated voting power or five $DIMO holders who each represent 1,000,000 $DIMO in delegated voting power have the ability to formally sponsor and introduce a DIP or DLP.&#x20;

Due to current technical limitations, the DIMO Foundation must assist in posting DIPs and DLPs that rely on more than one sponsor to reach the threshold. Email support@dimo.zone for help.

### **Proposal deliberation & withdrawal**

DIPs and DLPs that have been sponsored and introduced will be posted in the [Repo](https://github.com/DIMO-Network/DIP) and announced in the #📣announcements channel in [Discord](https://discord.com/invite/dimonetwork). After a the specified review period (ideally seven days) the DIP or DLP goes to a vote. The sponsor(s) may extend the review period if they choose.

At any time prior to voting, if the proposals does not maintain the support of at least 5,000,000 $DIMO worth of voting power (because token holders undelegated their tokens from sponsors or sponsors publicly withdraw their support), the proposal status is changed to "Withdrawn". Once the proposal reaches full sponsorship again, if ever, it will go back into _Review_, an announcement will go out in #📣announcements, and the review period begins again.

Authors may make edits to a proposal that has already been put into _Review_. Any edits should be summarized in the changelog section. If the edits have major effects on the purpose, interpretation, or implementation of the DIP or DLP, it is highly encouraged to reset the seven day review window and notify the community with an update in #📣announcements. Edits should not completely scrap the original proposal and replace it with something new (e.g., edit the proposal to go from a vote on the DIMO logo to a vote on token issuance). To do this, withdraw the DIP or DLP and submit a new one.

### **Voting protocol**

After seven days of deliberation, the DIP or DLP goes to a vote. Once a vote beings, the voting protocol works as follows.

**Definitions**

* **Circulating Supply**: Equals the 1) total supply of $DIMO minus the amount held by the Foundation as treasury or for baseline issuance. This is calculated as of the block that the vote is launched.
* **Voting Formats**: The only allowable formats are:&#x20;
  * Basic Voting: the only voting options are Approve, Reject, and Abstain and the vote is either approved or rejected at the end of the voting period.&#x20;
  * Ranked Choice: an instant runoff method whereby users rank their choices in order. If any option is ranked first by the required majority of voters, that options wins. If no option reaches majority, the option that received the fewest top rank choices by voters is eliminated and the nullified votes for that option are redistributed to each voter's second choice. This process repeats until one option reaches the required majority (and that options wins) or until there are two options left that both fail to reach the majority (e.g., if required majority is 60% and options 1 and 2 have 50% each and there is no winner). These votes must be done as off-chain poles on Snapshot.
  * Multiple Selection: voters are able to select multiple options, and each option that achieves the required majority is accepted. For example, this may be used to elect multiple members to a council. These votes must be done as off-chain poles on Snapshot.
* **Quorum**: This is the amount tokens required to participate in a vote for it to be considered valid. A vote that falls short on participation may still be considered valid if there are enough votes for Approve (in Basic Voting) or the top choice (in Rank Choice) such that majority would still be achieved even if every additional vote required to reach quorum were cast as Reject (in Basic Voting) or for the alternate choice (in Rank Choice).&#x20;

**Terms**

* **Venue**: All voting will occur on [Snapshot](https://snapshot.org/#/dimo.eth).
* **Duration**: Voting will be open for seven days (168 hours) for off-chain votes or 268,800 blocks on the Polygon PoS chain for on-chain votes (roughly 7 days). Voters may change their votes during this window.
* **Withdrawal**: Once in _Voting_, the proposal may not be withdrawn by the sponsors. It will either pass or fail.
* **Delegation**: $DIMO holders can delegate their voting power to themselves (allowing them to vote directly) or to someone else without having to transfer their tokens. To do this, click [here](https://delegate.dimo.zone), connect your wallet, and click "Delegate Tokens". Then enter the 0x address of the person you'd like to delegate your tokens to.  You remain in control of your $DIMO and can revoke or redelegate your tokens at any times. This action will require Matic tokens on the Polygon blockchain.
* **Weighting**: Voting is directly proportional to the amount of $DIMO a user has been delegated (by themselves or others);
* **Formats, Majority, and Quorum**: When possible and appropriate, voting and implementation should be conducted on-chain. Future DIPs and DLPs may enforce this more programatically.
  *   **Level 3 Votes**: For highly impactful votes that entail minting or burning tokens; altering governance; altering issuance; disposing or selling core intellectual property of the Foundation; transferring or committing over 15,000,000 $DIMO; or other very meaningful decisions as may be determined by the DIMO Foundation:

      Majority = 70%

      Quorum = 10% of circulating supply\
      Acceptable Voting Formats = Basic Voting, Ranked Choice
  *   **Level 2 Votes**: For somewhat impactful votes that entail transferring or committing between 5,000,000 to 15,000,000 $DIMO; removing a DIMO Foundation director; altering the DIMO Foundation Bylaws; or other meaningful decisions as may be determined by the DIMO Foundation:

      Majority = 60%

      Quorum = 5% of circulating supply\
      Acceptable Voting Formats = Basic Voting, Ranked Choice
  *   **Level 1 Votes**: For other votes that are less impactful in nature than those listed above, such as issuing non-exclusive licenses to core intellectual property that do not inhibit the DIMO network; transferring under 5,000,000 $DIMO (often for grants); delegating other resources and authority to individuals or groups who are helping to build $DIMO (e.g., recognizing a new DIMO Integrations team and granting it the right to issue licenses to device manufacturers):

      Majority = 50%

      Quorum = 3% of circulating supply\
      Acceptable Voting Formats = Basic Voting, Ranked Choice, Multiple Selection
* **Implementation**: There will be a four day (96 hour) timelock after the vote is completed before execution. This gives various stakeholders the opportunity to make any necessary preparations based on the outcome (e.g., connecting or disconnecting a car, staking or unstaking their tokens, etc.).
* **Voting Limits**: No individual voter shall vote with more than 5% of the circulating supply of $DIMO. Where possible, such as with off-chain votes on Snapshot, wallets that vote with more than 5% will have their vote weight reduced to disregard overages.
* **Invalid Proposals**: Proposals may not be enacted if doing so will result in the contravention of Cayman Islands laws or regulations, if it is non-compliant with the DIMO Foundation Memorandum & Articles and Bylaws, or causes clear harm to the Foundation. Transfers of $DIMO, other crypto, or fiat may be contingent on the recipient completing a Know Your Customer (KYC) process in the case of large grants.

To determine the outcome, we only look at the state of the vote at the moment the vote closes. If a vote has majority and quorum at the exact end of seven days, then the status changes to _Final_ and the four day timelock prior to execution begins. If a vote does not meet that criteria, the DIP or DLP fails to pass and the status changes to "Failed".

### **Amending & repealing DIPs and DLPs**

After a DIP has been passed, future proposals may amend or repeal that DIP. Such a proposal is subject to the same requirements as a standard DIP. This means that the requirements for proposal submission, voting, and all other specifications still apply. This also includes the requirement to follow the same structural format as any other DIP, complete with a header, abstract, motivation, specification, implementation, copyright, citation, changelog, and disclaimer section.

Any proposal amending or repealing a DIP need only amend or repeal the original DIP. In other words, it does not need to make updates to prior amendments. An amendment may alter multiple DIPs so long as it precisely clear what the changes are (e.g., to change terminology used across several DIPs).

#### If amending a DIP or DLP

The proposal must clearly specify exactly where and how the DIP(s) should be amended to leave zero ambiguity as to how changes would be implemented in the original document if the proposal were to pass. The amendment proposal should use a red font to denote the text that will be inserted into the original DIP(s) and red font with a strikethrough to denote the text that will be deleted. See [dip1a1.md](../amendments/dip1a1.md "mention") for an example of this formatting.

The amendment need not specify the language for the changelog, however the editor must note and link to the amendment in a new changelog entry once implemented.&#x20;

## Implementation

If passed, this DIP will be in effect immediately after the four day timelock concludes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP-1: DIMO Governance Guidelines", no. 1, November 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog

Dec 7, 2022: added discussion forum and voting type to the DIP header.

Dec 7, 2022: adjusted review date to give people more time to claim the Airdrop prior to voting going live.

Dec 7, 2022: added clarifying language to the section on voting limits.

Dec 8, 2022: altered quorum thresholds based on data points from other projects.

Dec 8, 2022: added clarity to the definition of circulating supply.

Dec 8, 2022: added additional clarification invalid proposals related to money transfer.

Dec 26, 2023: adjusted review date again to allow for fixes to delegation strategy prior to voting.

Jan 2, 2023: adjusted the terms around review period to remove the requirement for a full seven day review.

Jan 6, 2023: final adjustment to review date — proposals go to vote on Tuesday Jan 10.

Dec 26, 2023: adjusted review date again to allow for fixes to delegation strategy prior to voting.

Jan 2, 2023: adjusted the terms around review period to remove the requirement for a full seven day review.

Mar 29, 2023: passed [DIP-1: Amendment 1](../amendments/dip1a1.md)

Jun 16, 2023: passed [DIP-1: Amendment 2](../amendments/dip1a2.md)

July 6, 2024: disclaimer adjusted and added concept of DLPs

## Disclaimer

Certain statements in this document constitute forward-looking statements. The words “may,” “will,” “should,” “project,” “anticipate,” “believe,” “estimate,” “intend,” “expect,” “continue,” and similar expressions or the negatives thereof are generally intended to identify forward-looking statements. Such forward-looking statements, including the intended actions and performance objectives, involve known and unknown risks, uncertainties, and other important factors that could cause the actual results, performance, or achievements to differ materially from any future results, performance, or achievements expressed or implied by such forward-looking statements. There can be no assurance that such statements will prove to be accurate as actual results and future events could differ materially from those anticipated in such statements. Accordingly, readers should not place undue reliance on forward-looking statements and nothing in this document represents a promise of specific work to be completed in the future.&#x20;

The contract addresses for $DIMO are 0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b on [Ethereum](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b), 0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c on [Base](https://basescan.org/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c) / [Optimism](https://optimistic.etherscan.io/address/0x5eAA326fB2fc97fAcCe6A79A304876daD0F2e96c), and 0xE261D618a959aFfFd53168Cd07D12E37B26761db on [Polygon](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db). Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
