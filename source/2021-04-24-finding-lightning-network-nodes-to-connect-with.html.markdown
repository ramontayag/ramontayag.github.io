---
title: Finding Lightning Network Nodes to Connect With
date: 2021-04-24
tags: bitcoin, lightning network
---

In this blog post, I will talk about what I've learned so far trying to find nodes to find lightning nodes connect with that will help one become a routing node and earn some sats.

READMORE

Disclaimer: I am a newbie at this and using this blog as a way to journal my education.

# Why

I've spun up a Lightning Network node with the intention of lending sats over [Lightning Pool](https://pool.lightning.engineering). I quickly learned that no one was taking up my offers to lend, and that was most likely because my node didn't have a reputation.

I want to increase my node's reputation so I may do a wider variety of things, like lend over Lightning Pool, more effectively.

# Reputation?

A reputation is important to those borrowing because when they ask for that liquidity, they want someone who is more likely to be around than not. It makes sense: if you were borrowing and had two nodes offering the same interest rate, you would choose the one with a higher reputation.

One's reputation has to do with:

- uptime
- reliability in being able to forward payments (which implies a other things like well-balanced channels)

It seems that the BOS Score is used to calculate the score of one's node, but the score itself is proprietary.

<figure>
<img src="/2021-04-24/finding-lightning-network-nodes-to-connect-with/bos-question.gif">
<img src="/2021-04-24/finding-lightning-network-nodes-to-connect-with/bos-proprietary-answer.gif">
<figcaption>
Though proprietary, it seems that Lightning Labs is at least going to clarify how it works. (Here's the [link](https://lightningcommunity.slack.com/archives/C6BPPDL7P/p1615914752001800), but it's a public Slack channel so it won't be there for long.)
</figcaption>
</figure>

For now, the best way I've found to understand how to make your Lightning node get a better score is to listen to [Alex Bosworth has to say](https://www.youtube.com/watch?v=HlPIB6jt6ww). Someone has kindly shared their notes [here](http://diyhpl.us/wiki/transcripts/chaincode-labs/2018-10-22-alex-bosworth-channel-management/).

# Ok, now what?

Now that I have a vague idea of what reputation is, what do I do? The first thing I'm looking at is to connect to nodes and provide liquidity. Which nodes though? What assurances (doesn't have to be 100%) I won't be locking up Bitcoin and spending on transaction fees by connecting with a node that isn't going to send or receive that much anyway?

## Lower-fee routes

While browsing [/r/lightningnetwork](https://www.reddit.com/r/lightningnetwork), I found [a post](https://www.reddit.com/r/lightningnetwork/comments/lb7pbk/last_month_i_collected_over_7000_sats_in_fees/) that shared a tool that traverses the network and essentially returns a list of nodes that would likely help you increase your routing activity.

> The idea is that we want to choose channel peers who offer us the greatest benefit to routing diversity across the LN below a given feerate threshold. Since during the payment process LN nodes try lower-fee routes before moving on to higher-fee routes, by increasing the number of ways nodes can reach you/be reached by you at low fee rates, you increase the probability that your node will lie along a successful payment route and thus your share of the LN payments market.
>
> -- ajpwahqgbi

## Nodes that peer with many

I have yet to read the code and understand what it does, but it is a start. As the author has stated, there are other ways to find out which nodes to connect to. I posed the "whom should I connect with" question in a pay-to-join [Telegram group](https://t.me/LNBalancedChannels) (pretty cool, you pay sats) and got this advice:

<figure>
<img src="/2021-04-24/finding-lightning-network-nodes-to-connect-with/peer-with-peer-with-many.gif">
</figure>

This is sounds logical, and I have yet to find/design a way to do this. Two thoughts immediately come to mind:

1. Look at a graph and visually select these nodes
2. Write a script that returns a list of these nodes

Of course, if the first option can do it, I'd rather stick to that, but it also can't be automated because I'll be relying on my vision to do so.

I can also imagine combining these tools together: find nodes that peer with many and run that through the lower-fee routes script.

# End

I'll be posting more as I learn more. These series of posts will not be as polished as the others I share around since they act more like notes than anything else.
