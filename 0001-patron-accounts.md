# DIP Template

- Author(s): charlesfayal
- Start Date: 2022-02-07
- Category: accounts
- Original DIP PR: <!-- leave this empty; maintainer will fill in ID of this pull request -->
- Tracking Issue: <!-- leave this empty; maintainer will create a discussion issue -->

# Summary
[summary]: #summary

Creating incentives for people "Patrons" to enlist other people "Hosts" onto the network is one of the quickest ways to grow a network. The goal here is to create a way for Patrons to setup their accounts such that rewards for devices in hosts cars are sent to their Patron account. The Patrons can then distribute to their hosts however they see fit. This differs from "Fleets" (the ability to setup a fleet of cars on your account) in that the Patron does not have access to the cars data, only rewards.

# Motivation
[motivation]: #motivation

The goal is to create a hosting arrangement that allows for Patrons to have incentives to quickly grow the network of vehicles.

Currently the incentives are:
* Personal incentives - Incentives for persons who setup their own cars and receives DIMO tokens for it. 
* Fleet arrangements - Incentives for persons who setup a fleet and receives DIMO tokens for those cars. 
* Referral codes - Unknown incentive structure that cannot be defined by the Patron.

None of these incentives aligns well with Patrons who would want to help expand the network by enlisting family/friends/others. A referral code is unlikely to be a strong enough incentive. It also may be advantageous in a number of situations to pay hosts in fiat rather than in DIMO tokens. Allowing the rewards to go to the Patron's account allows them to pay hosts however they deem fit e.g. for example in cash instead of tokens. 

A big benefit of having a Patron model in the DIMO network is that some of the strongest community members in a network like this are Patrons. Patrons have the most incentives to see the network be successful and so are the most willing to dedicate time and resources to build off of the network. Many of the moderators and active members in the Helium community are Patrons.

# Stakeholders
[stakeholders]: #stakeholders

* Who is affected by this DIP?
Patrons i.e. anybody who wants to get other people "hosts" onto the network. 
Hosts i.e. people who connect their car to the DIMO network.


* How are we soliciting feedback on this DIP from these stakeholders? Note that
  they may not be watching the DIPs repository or even aren't directly active in
  the Discord Community Slack channels.

# Detailed Explanation
[detailed-explanation]: #detailed-explanation

- Introduce and explain new concepts.
Patron - Person who enlists others to join the network and directly receives DIMO tokens. A Patron should not have access to the cars data.
Host - Person who is enlisted who does not directly receive DIMO tokens. A Host should also have access to their cars data and be able to control where the data goes. 

A DIMO integration (whether through app or through a AutoPi type device) should be able to have their rewards paid out to one account (Patron account) meanwhile allowing access to the cars data to another account (Host account). 

An added benefit would be for the Patron to be able to automatically pay out to the host on a percentage basis.

- It should be reasonably clear how the proposal would be implemented.

- Provide representative examples that show how this proposal would be commonly
  used.
Much of the Helium network was built off this model.

- Corner cases should be dissected by example.
If a car is connected via a SmartCar integration could they later just sign up as a Patron themselves and skip the middleman.

# Drawbacks
[drawbacks]: #drawbacks

- Why should we *not* do this?

# Rationale and Alternatives
[alternatives]: #rationale-and-alternatives

This is your chance to discuss your proposal in the context of the whole design
space. This is probably the most important section!

- Why is this design the best in the space of possible designs?

- What other designs have been considered and what is the rationale for not
  choosing them?

- What is the impact of not doing this?
Slower network growth.

# Unresolved Questions
[unresolved]: #unresolved-questions

- What parts of the design do you expect to resolve through the DIP process
  before this gets merged?

- What parts of the design do you expect to resolve through the implementation
  of this feature?

- What related issues do you consider out of scope for this DIP that could be
  addressed in the future independently of the solution that comes out of this
  DIP?

# Deployment Impact
[deployment-impact]: #deployment-impact

Describe how this design will be deployed and any potential impact it may have on
current users of this project.

- How will current users be impacted?

- How will existing documentation/knowlegebase need to be supported?

- Is this backwards compatible?

        - If not, what is the procedure to migrate?

# Success Metrics
[success-metrics]: #success-metrics

What metrics can be used to measure the success of this design?

- What should we measure to prove a performance increase?
Number of host arrangements.

- What should we measure to prove an improvement in stability?

- What should we measure to prove a reduction in complexity?

- What should we measure to prove an acceptance of this by it's users?
