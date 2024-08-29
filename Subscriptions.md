# MOR NFA Subscriptions

The Safe Stake Subscription is a component of the NFA smart contract that allows a Smart Agent builder to offer a subscription to recurring agent services. 

## The goals are:
To provide an agentic commerce protocol that incentivizes the agent builder to offer subscriptions to/for/by a Smart Agent on Morpheus. 
- Reward long term staking, decreasing supply
- Increase demand via increased utility of the MOR token and all MOR20 tokens 

## This document focuses on subscriptions. Retail and wholesale sales will be a separate toolset in the NFA contract. 

The SSS mechanism evolves the current staking codebase used by MOR and MOR 20 staking (details tbd) 

## Process
To pay for a subscription, the subscriber stakes an amount of MOR for a predetermined amount of time. As long as that stake is in place, the subscription remains valid. Agent owner sets the staking terms required for a subscription. 

A first use of this is an agent named Neo Picasso who dispatches one unique image per day to every subscriber that stakes one MOR for one year. Neo Picasso is managed by an NFA contract that processes the staking. Inference for the images and conversation come from the Morpheus lumerin node. 

X% of the daily MOR community emissions are distributed pro rata  to an agent owners based on the amount under agent stake.  There is a mechanism that discourages agent owners  from immediately liquidating: tba/tbd. 

The owner of the Neo Picasso Agent is able to sell the agent outright like an nft. All stake rewards follow the agent, so a new owner sees immediate return from staking. There is a mechanism that discourages immediate liquidation, tba/tbd

A transfer fee as part of the sale of an agent that requires updating on-chain Agent data includes a few basis points returned to the platform and developers. 

A subscription may be canceled after X days. A cancellation fee is distributed to the agent owner with a percentage of the cancellation fee passed to the platform and developers. 

## Roles:
- Agent builder 
- Stakes an agent to the network(s)
- Publishes Subscription Service with a registration fee
- Time and amount of stake
- Time of deferment
- Purpose of Agent
- Offers a Subscription of Agent services
- Receives a pro-rata amount of x% of the community emission based on amount staked buy submission

## Agent customer
- Subscribes to agent service.
- Staking X MOR for Y time.
- Uses hash as proof of subscription
- Can auto-renew after staking time is complete
- Can unstake for a single payout fee.

## Suggested subscription parameters:
- What is the current best use of NFT for membership/subscription?
- Proof of stake 
