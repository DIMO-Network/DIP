# DIP-1: Amendment 2

> **Headline**: Enabling voting on Ethereum
>
> **Author**: Rob Solomon
>
> **Submitter(s)**: Rob Solomon \[robsolomon.eth]
>
> **Status**: Deployed
>
> **Voting URL**: [Snapshot](https://snapshot.org/#/dimo.eth/proposal/0xf10888550c0e443d0aaec0255f2c397227355c564d93e368916541cf27cfb254)
>
> **Discussion Forum**: [Discord](https://chat.dimo.zone) #🗳️governance forum
>
> **Vote Type**: [Level 3](https://docs.dimo.zone/governance/dip1#voting-protocol)

## Abstract

This proposal calls for an upgrade to $DIMO on Ethereum Mainnet version to give it comparable voting functionality to the $DIMO token on Polygon. Specifically, this proposal would give holders the ability to delegate tokens to another wallet of theirs or to someone else who can vote on their behalf.

## Motivation

As more $DIMO is bridged back to Ethereum Mainnet, it becomes increasingly important for governance participation that holders on both chains can participate in voting. Large holders may elect to use services such as Coinbase Custody, which only supports $DIMO on Ethereum and requires the ability to delegate.

## Specification

The current version of the DIMO token on the Ethereum Mainnet does not have built-in support for user voting. To enable this feature, this proposal would implement the [ERC20VotesUpgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/contracts/token/ERC20/extensions/ERC20VotesUpgradeable.sol) contract as a parent contract of the DIMO token's base contract. This additional contract includes mechanisms for creating checkpoints of the total token supply and individual user balances each time a transfer is made. These checkpoints are then used by the voting system to determine a user's voting power at a specific point in time.

**The specific code to be implemented is visible** [**here**](https://github.com/DIMO-Network/dimo-token/pull/8)**.**

Some may wonder why we cannot simply use the `balanceOf` function to determine a user's voting power. While it is possible to create our own voting method, we believe it is better to follow established standards within the Ethereum community. Just as we use the [ERC20](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/) standard to power the DIMO token, we also rely on the widely accepted [OpenZeppelin Governor](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/contracts/governance/GovernorUpgradeable.sol) contract for executing protocol changes through voting. This contract, along with its [Snapshot](https://snapshot.org/#/) and [Tally](https://www.tally.xyz/) functions, utilizes the `getVotes` function within the `ERC20VotesUpgradeable` contract. This approach is particularly important during the voting period of a proposal, which may last for several days. By using checkpointed balances instead of real-time balances, we can ensure that a user's voting power is locked in during the voting period and cannot be changed by subsequent balance changes.

We recognize that upgrading a smart contract, particularly when inheritance is involved, can be a challenging process. To address this, we have extensively tested the changes on testnets and in forks of the Mainnet, using well-established [OpenZeppelin](https://www.openzeppelin.com/) and [Hardhat](https://hardhat.org/) libraries. Our goal is to ensure that these upgrades do not conflict with existing storage and that users' balances remain unaffected.

Attached is a security audit report conducted by Sayfer that tested this upgrade as well as a few others.

{% file src="../.gitbook/assets/Sayfer - 2023 - Smart Contract Auditing DIMO CFD.pdf" %}

{% file src="../.gitbook/assets/Smart Contract Audit Report for Dimo (1).pdf" %}

#### Amendments to DIP-1

_<mark style="color:green;">// If passed, this proposal would append the following to the end of the DIP-1 Specification section:</mark>_&#x20;

**Delegation**: $DIMO holders can delegate their voting power to themselves (allowing them to vote directly) or to someone else without having to transfer their tokens. To do this, click [here](https://delegate.dimo.zone), connect your wallet, and click "Delegate Tokens". Then enter the 0x address of the person you'd like to delegate your tokens to.  You remain in control of your $DIMO and can revoke or redelegate your tokens at any times. ~~<mark style="color:red;">This action will require Matic tokens on the Polygon blockchain.</mark>~~ <mark style="color:red;"></mark><mark style="color:red;">Delegation is an on-chain event that requires Matic tokens (if delegating on Polygon) or Ether (if delegating on Ethereum Mainnet).</mark>

## Implementation

If passed, the Ethereum Mainnet token will be upgraded as specified [here](https://github.com/DIMO-Network/dimo-token/pull/8) and DIP-1 would be updated as specified above after the four day timelock concludes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0)

## Citation

Please cite this document as:

The DIMO Foundation, "DIP 1 Amendment 2", May 2023. \[Online serial]. Available: \[[https://github.com/DIMO-Network/DIP](https://github.com/DIMO-Network/DIP)]

## Changelog



## Disclaimer

The contract addresses for $DIMO are [0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b](https://etherscan.io/token/0x5fab9761d60419c9eeebe3915a8fa1ed7e8d2e1b) on Ethereum and [0xE261D618a959aFfFd53168Cd07D12E37B26761db](https://polygonscan.com/token/0xE261D618a959aFfFd53168Cd07D12E37B26761db) on Polygon. Please always confirm that you are interacting with these contract addresses and not those of a fraudulent imitator. This proposal may not be enacted if it violates Cayman Islands law. Please triple check that any communications are authentic as it’s common for scammers to try to trick you into sending them crypto or into revealing your private keys.
