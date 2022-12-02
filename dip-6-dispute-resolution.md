# DIP-6: Dispute Resolution

> **Author**: Diego Moro, Marisa Zelip, [Rob Solomon](https://twitter.com/robmsolomon)&#x20;
>
> **Status**: Draft
>
> **Headline**: A conflict resolution process for disputes within the DIMO ecosystem
>
> **Voting Format \[URL]**: [\[Snapshot\]](https://snapshot.org/#/dimo.eth/proposal/0x096a7ee8ebc3bb90c5aab4afa516ab0700aa436c5f4f92c0a7d7fec24457646d)

## Abstract&#x20;

This proposal defines how conflicts are resolved via a dispute resolution process which includes a challenge, mediation, and resolution among two or more parties in the DIMO value chain (seen below) including, but not limited to, drivers, fleet operators, app developers, node operators, and certified hardware manufacturers.

![](<.gitbook/assets/image (5).png>)

To resolve disputes, this DIMO Improvement Proposal #2 outlines the creation of the DIMO Court, a council composed of reputable experts with experience on IoT, data privacy, and blockchain related arbitration and/or mediation.&#x20;

## Motivation&#x20;

DIMO will preempt conflicts with objective protocols and smart contracts where possible. For everything else, it is crucial for DIMO to have a clear and transparent method to resolve issues and maintain the right incentives among the various participants in the ecosystem.

The goal for this proposal is to design and deploy a transparent and unbiased conflict resolution process that increases trust amongst DIMO users.&#x20;

## Specification&#x20;

### Actors&#x20;

#### Challenger

The Challenger is the individual or group that initiates the dispute resolution process. They may challenge another party if there is reasonable suspicion that that such party is acting against the rules set forth to govern interactions within the DIMO community, causing harm to the Challenger and/or the DIMO community in general.

To mitigate frivolous challenges and to ensure funding for the arbitration process, the Challenger must post an initial $DIMO deposit (this staking schedule can be found in [Challenge](dip-6-dispute-resolution.md#challenge) below). This deposit will be returned plus a reward if the DIMO Court rules in favor of the Challenger. The entire deposit may, and most likely will be, lost if the Defendant is instead favored. More information can be found below in the [Resolution](dip-6-dispute-resolution.md#resolution) section.

In the event that there are multiple individuals challenging a Defendant on the same issue, the first Challenger to move forward with the process will be named on the documentation. They may, however, work with other individuals to collect evidence and prove their case.&#x20;

#### Defendant

The Defendant is the counterparty pursued by the Challenger. If they have $DIMO staked (e.g., licensed hardware manufacturers, node operators, etc.) their stake will be locked until the conflict has been resolved.&#x20;

Should the DIMO Court favor the Challenger over the Defendant, the Defendant may lose some or all of their staked $DIMO and/or their license.

As an example, a hardware user may suspect that the manufacturer has hacked devices to stream data to their private server and sell it without compensating the data providers. In this case the user would be the challenger, and they would collect evidence and stake $DIMO to challenge the hardware manufacturer, the defendant, who should already have $DIMO staked.&#x20;

#### DIMO Court&#x20;

The DIMO Court is composed of lawyers, experts on cryptocurrency and blockchain related mediation and/or arbitration. The DIMO Court members will initially be picked by the DIMO Foundation from the [JAMS neutrals database](https://www.jamsadr.com/neutrals/) and will be drawn at random as mediators and arbitrators for a challenge when one has been raised.

To avoid any conflict of interest, the mediators and arbitrators will not be allowed to hold $DIMO at any point of time. They will also remain anonymous until they declare a verdict to avoid unethical behavior such as bribery.

To become a DIMO Court member, prospective candidate must have:

* At least 5 (five) years of experience in mediation and arbitration;&#x20;
* Experience with mediation of multiple disputes arising from smart contract transactions; and&#x20;
* A track record of successfully mediated and arbitrated disputes.

Plus bonus points if they've also been recognized as a certified Blockchain Professional by IIB Council (optional).&#x20;



### Dispute Resolution Process&#x20;

#### Challenge&#x20;

A Challenge is the first step in which any person(s) (challenger) officially states their claim that they have suspicion or evidence that another party is acting with negligence or in bad faith within the DIMO ecosystem.

The challenger must first initiate a formal challenge. (how to properly initiate - in #dispute-resolution ?) Next, the challenger must stake $DIMO. The amount that must be staked can be seen here.

The accused party (the defendant) must already have $DIMO staked.&#x20;

#### Mediation&#x20;

Mediation is a voluntary, non-binding process using a neutral third party to help the parties reach a mutually beneficial resolution of their dispute. A mediator may help the parties reach a resolution by facilitating communication, promoting understanding, assisting them in identifying and exploring issues, interests and possible bases for agreement, and in some matters, helping parties evaluate the likely outcome in court or arbitration if they cannot reach settlement through mediation.

After a challenge is formally initiated, a mediator shall be selected either at random by the DIMO Foundation from the DIMO Court or by both parties from the [JAMS neutrals database](https://www.jamsadr.com/neutrals/). Under the mediator’s guidance, the defendant may state their case, both parties may show further evidence, and both parties may settle the dispute through mediation.

It is important to note that mediation does not have the formalities of arbitration and no binding decision is made.&#x20;

#### Arbitration&#x20;

Arbitration is a binding, adjudicatory procedure in which both parties produce evidence for their case then, at the end of an arbitration hearing, the overseeing arbitrator renders a decision that is final and binding.

The Federal Arbitration Act, coupled with any arbitration laws of the place of arbitration, shall govern the process. JAMS arbitration rules shall govern the procedure.

If no settlement was reached during mediation between the challenger and defendant, then the case shall move into arbitration. An arbitrator will be selected at random by the DIMO Foundation from the DIMO Court to oversee the dispute.

The challenger and the defendant shall enter a pre-dispute contract, in which they agree that the dispute in question shall not be moved into an official court system during or after the arbitration process, and waive their right to a trial by jury of their peers. Additionally, both parties shall not have a de novo (second trial) after entering the pre-dispute contract. Unless otherwise agreed, the decision is legally binding, except in extremely limited circumstances, such as in the case of fraud or collusion on the part of the arbitrator.

The arbitrator may recommend a formal process for arbitration. In any case, both parties shall state their cases and provide evidence. The arbitrator shall declare a verdict and shall define the damage to be repaired (if any) in $DIMO amount.

If either party is not content with the verdict or the reparation amount, then they may appeal the decision. A new arbitrator shall be selected at random and a new round of arbitration shall take place. It is worth noting that the new arbitrator will have no previous knowledge of the prior verdict or reparation amount in order to keep their decision impartial. New evidence may be provided by both parties.

After the second hearing, the arbitrator shall declare a verdict and the damage $DIMO amount to be repaired (if any). If the verdict coincides with the previous, then the case will be considered closed and the reparations due will be that of the second arbitration round. If it doesn’t coincide with the previous verdict, a final round will occur in which a final arbitrator shall determine a final verdict.

In the case that the second arbitrator agrees with the first arbitrator on the verdict but disagrees on the reparation amount, the challenger or the defendant may appeal the decision once more.

In the final round of arbitration, the newest arbitrator shall make a final hearing of both parties and declare the final decision and reparation amount. This decision is final and binding.&#x20;

#### Resolution&#x20;

Reparations to be paid will be as follows:

_The Challenger_

If the Challenger wins, they will receive 1% of the total reparation to be paid by the defendant with a minimum of twice the amount the challenger staked.&#x20;

If the challenger loses, they will lose all their staked tokens. These tokens will be used as compensation for the arbitrator(s) services (plus any difference). Excess tokens will be burned.

_The Defendant_

If the defendant wins, they will keep all their staked tokens.&#x20;

If the defendant loses, they will be responsible for the payment of the reparation $DIMO amount stated by the arbitrator (with a minimum of twice the amount staked by the challenger) plus the arbitrator(s) compensation. This will be taken from their previously staked $DIMO (plus any difference).

## Implementation&#x20;

If passed, this DIP-2 will be in effect immediately after the four-day timeclock concludes.&#x20;

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)&#x20;

## Citation&#x20;

Please cite this document as: Diego Moro, Marisa Zelip, Rob Solomon, "DIP-2: Dispute Resolution", no. 2, May 2022. \[Online serial]. Available: \[https://github.com/DIMO-Network/DIP]

## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
