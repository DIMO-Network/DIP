# DIMO Nodes & Token Upgrades

The following outlines a **possible** tokenomic upgrade to the DIMO protocol. **This change is not guaranteed to be implemented and this post is shared for feedback and reference purposes only.**

It specifies how applications built on DIMO can pay for access to user vehicle data, once they are authorized by the user, using a stable DIMO Credit (DCX) or $DIMO. It also specifies how DCX is used in other types of transactions, how $DIMO tokens are converted into DCX, and how some of that $DIMO is recycled and rewarded back to both users and the nodes that store their data. This model draws inspiration from Helium, particularly the relationship of HNT to Data Credits and Data Transfer rewards.

For convenience, this is written in the style of a post implementation blog post – describing the DIMOverse as if these changes have already been approved and implemented. A governance vote and additional engineering would be necessary to implement what is described below.

### What is a node

DIMO puts users in control of their data, including where it’s stored. A storage provider on DIMO is known as a “node”, and each one plays a key role in storing, verifying, securing, and transmitting data across the network. Users can choose any public node to store their data with and they can even run their own node and store their own data if they prefer. Nodes are rewarded for performing this function and penalized for excessive downtime.

Developers who build on DIMO (e.g., a usage based insurance policy that users share their location, speed, and vehicle data with) have the experience of interacting with a centralized database, despite the distributed architecture. To help understand, consider other decentralized protocols that feel unified: you submit a transaction to the Ethereum Mainnet regardless of which validator mines it; you simply email anyone regardless of whether you, or they, use Gmail, Outlook, Proton, or your own home server; and you open your browser and access the internet not caring which server a website lives on. This architecture gives users control and adds resiliency and neutrality to the DIMO Network, without compromising usability.

With DIMO, vehicles transmit secure information such as odometer, location, speed, and fuel level to their selected node. Vehicles and drivers also receive credentials from various apps built on DIMO, such as “vehicle is registered”, “insured up to $1,000,000”, “title is clean”, and “licensed to drive taxis in New York”, that are verifiable and digital. Nodes store all of this data for users offchain and make it available to others when the user grants permission. As data is encrypted, nodes aren’t able to read the data that they’re storing; only the user and the apps and individuals that users share their data with can read it.

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

### DCX & $DIMO

DIMO apps and other businesses wishing to acquire DIMO user data and commands (e.g., remote vehicle lock/unlock) can access it from via API, but only when a user gives their consent and only when they pay for it. The DIMO Vehicle ID NFT has a built in permissioning system and contains a URI that points to the location of the node storing the data.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

All payments for user data, as well as all other DIMO protocol fees (e.g., the fee to mint a car), requires spending DIMO Credits (DCX) or $DIMO. DCX is always worth $0.001 USD, and the only way to generate DCX is by trading in $DIMO, which converts at the market price. E.g., if $DIMO is currently at $10, swapping 1 $DIMO generates 10,000 DCX. When $DIMO is spent to acquire DCX, some is rewarded back to users and node operators and some is burned. A DCX cannot be converted back into $DIMO and when it is spent, it is burned forever. More on this in [Rewards & burn](dimo-nodes-and-token-upgrades.md#rewards-and-burn) below.

This conversion process is administered by a series of smart contracts that allows anyone to generate DCX permissionlessly. A combination of Uniswap and Chainlink oracles are used to provide the $DIMO price that is needed to calculate the conversion. To prevent manipulation or system failures, the contract is temporarily halted if these two oracles get out of sync with one another.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption><p>A hypothetical conversion of $DIMO to DCX</p></figcaption></figure>

If developers hold $DIMO tokens, they are able mint DCX anytime, or they can simply pay in $DIMO, where conversion to DCX and payment is combined into one step that happens in real-time.

Developers can also purchase DCX directly from services that have already done this conversion for them. This can be done ahead of time (the developer will hold the DCX) or just in time (the developer never holds DCX or $DIMO, which is instead submitted on their behalf after they pay with fiat). This is beneficial for developers who are not yet ready to make the leap into crypto or accept the volatility that comes with it.

Also, DIMO’s wallet as a service includes account abstraction and an ERC-4337 [paymaster](https://www.alchemy.com/blog/account-abstraction-paymasters) that sponsors gas, further simplifying the developer and user experience.

### Using DCX for vehicle data access fees

Once an app developer has a license and a user grants them onchain permission to access their vehicle data, they simply ping the node network and pay the required amount of DCX to access the data they need. The payment gives the app the ability to pull data via API a set number of times per vehicle per data category for one month.&#x20;

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

Additional data types may be added in the future (e.g., video). The price to connect to one car per month is shown below. While apps may only work for certain regions, vehicle types, and users, they may not block access to users based on the node operator they’ve chosen.

Payments are partially refunded if the node operator fails to maintain the 97% uptime, in direct proportion to the amount of downtime (e.g., 20% downtime means 20% is refunded). See [Penalties](dimo-nodes-and-token-upgrades.md#penalties) for more.&#x20;

### Using DCX for flat protocol fees

Previously, hardware manufacturers had to pay 25 $DIMO to mint a hardware device. This was fairly straightforward, but meant that the real cost of minting devices in USD terms was volatile as the price of $DIMO fluctuated.

DCX gives us the opportunity to provide a stable price for hardware minting and these new flat protocol fees without undermining the role of the $DIMO token. The following protocol fees are now implemented.&#x20;

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

As is this case with paying for API access, users can pay all fees in either DCX or $DIMO, which **includes the blockchain gas cost** covered by the paymaster, meaning that users and apps never need MATIC, ETH, or any other gas token. Applications can also sponsor the cost of all fees paid in DCX or $DIMO if they want to provide the user with a streamlined, entirely gasless and paymentless experience**.**

$DIMO token holders can always vote to add and adjust fees in the future as the network matures. Some examples include fees to: transfer a digital vehicle title; issue credentials related to maintenance; or register a car with the DMV onchain.

### Rewards & burn

When $DIMO is converted into DCX, that $DIMO is sent into a rewards pool known as the Market Issuance Pool. The name of this pool acknowledges the fact that this pool is funded by demand side market activity, as opposed to the preset and temporary Baseline Issuance Pool.&#x20;

**Each month, all $DIMO in the Market Issuance Pool is partly distributed to nodes and users and partly burned**. The relative amounts are determined based on the proportion of DCX accumulated, calculated as follows:

* 60% of all DCX spent on vehicle data access fees goes to the node and/or user whose data is being purchased. How the DCX (and, therefore, the $DIMO reward) is split between the node and user is up to those two parties. Nodes can compete on terms and features and users are free to choose the best one for them, similar to email providers. To give an example, if 1,000,000 $DIMO is set to go out in a month and one specific node operator earned 1% of all DCX spent that month, they receive 10,000 $DIMO. If that node operator agreed to a 50/50 split with their users, then the node operator keeps 5,000 $DIMO and distributes the remaining balance to users. The node client software automates this process.
* 40% of all DCX spent on vehicle data access fees and 100% of DCX spent on flat protocol fees is reserved for the DIMO Protocol itself. Any $DIMO that is issued to the DIMO Protocol first replenishes the small amount of resources needed to maintain the paymaster service, and then the rest is burned.&#x20;

<figure><img src="../.gitbook/assets/Img_Distribution (1).png" alt=""><figcaption><p>Distributions in a hypothetical month</p></figcaption></figure>

#### **Rewards & burn FAQ**

Q: What happens as the total $DIMO supply continues to burn towards zero?

A: There are a few options:

1. _Do nothing_: This is the current default option. Even in the most optimistic scenario, $DIMO is unlikely to burn to zero given that $DIMO converts to DCX at market price and is divisible to 18 decimal points (1b $DIMO \* 10^18 decimal points = one octillion units of $DIMO);
2. _Token split_: DIMO could enact a rebase or split, although this may have unfortunate tax consequences for individuals in various jurisdictions;
3. _Mint into the treasury or baseline issuance pool_: The protocol can vote to mint new tokens which could be sold to fund development, added to baseline issuance to increase or extend baseline rewards, or used in some other way; and/or
4. _Automatically Inflate_: DIMO could enact some type of inflationary mechanism (like Ethereum or Bitcoin’s automatic block reward) or equilibrium mechanism (like Helium’s Burn-Mint-Equilibrium) to counterbalance the deflation.

***

Q: Why have a DCX at all rather than simply using $DIMO?

A: This is the simplest way to address the needs of businesses (who perhaps cannot hold most crypto or don’t want to experience volatility) and to develop DIMO Protocol smart contracts that charge fees at stable prices globally.

***

Q: Why not issue the $DIMO in the period where the DCX is spent rather than the immediate period following when it was minted?

A: DCX is a fungible token meaning that it’s impossible to say when the $DIMO was spent to create that DCX. This approach makes a bet that the minting of DCX and spending of it grows smoothly and in relative balance over time.

***

Q: Why issue rewards monthly instead of weekly or instantly?

A: First, node operators are responsible for delivering data on a monthly cycle and they should not be rewarded in week 1 if they go down in weeks 2-4. Second, this helps smooth out irregularities to reduce manipulated or unfair outcomes.

### Being a node operator

#### **How to run a node**

Running a node on DIMO is fairly straightforward. Node operators must:

1. Ensure that their equipment meets the minimum requirements;
2. Bond the required amount of $DIMO tokens in order to mint a license, which is represented by a non-transferrable NFT;
3. Install and run an approved DIMO client (free to use and open source); and
4. Maintain good up-time and top of the stake in the event of slashing.

#### **Penalties**

As previously described in [Using DCX for vehicle data access fees](dimo-nodes-and-token-upgrades.md#using-dcx-for-vehicle-data-access-fees), a node and user only earn the full amount of DCX when there is 3% or less downtime in a given month. Above this threshold, nodes and users will miss out on DCX in proportion to the downtime percentage. Additionally, when downtime is at or above 10%, nodes are subject to additional slashing penalties per the simple formula dB \* 1%, where d is the percent downtime for the month and B is the required bond amount set by the DIMO protocol for node operators (currently 100,000 $DIMO).

This would result in the following slashing penalties for downtime for a given month.

<figure><img src="../.gitbook/assets/Chart_3.png" alt=""><figcaption></figcaption></figure>

If a Node’s bonded amount drops below 80% of the required amount (currently that’s 100,000 \* 80% = 80,000 $DIMO), they will have two months to replenish their bond before their license is revoked.
