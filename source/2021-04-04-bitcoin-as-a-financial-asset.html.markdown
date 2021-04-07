---
title: Bitcoin as a Financial Asset
date: 2021-04-04
tags: bitcoin
---

I was recently approached as a candidate to speak about Bitcoin as a financial asset to a group of professionals in that field. However, plans changed and I ended up not joining panel. Because this is a topic I am deeply interested in, I decided to get it down in writing to use it in the future, and of course, to help others understand Bitcoin.

READMORE

Though I'm not a cryptographer or a distributed systems programmer, having a computer science background allowed me to more easily understand the technical side of Bitcoin. Naturally, while learning the technical side of Bitcoin, I asked the age-old question: **what is money?**

This quickly led me down the deep rabbit-hole of money and its history, banking and its history, fiat currencies, gold standard, economics, and the latest addition, macroeconomics. In 2019, it started to click for me: **Bitcoin is the most important invention since the Internet because of its potential to be a global reserve asset**. Since money is a winner-take-most game, I decided to set my sites exclusively on Bitcoin.

This article is certainly not my original thoughts. I'd like to thank Preston Pysh, Lyn Alden, Greg Foss, Nik Bhatia, and many others who, through their articles and podcasts, have helped me understand Bitcoin from a financial point of view.

In this article, we will cover:

1. [History](#history)
2. [How Bitcoin is Valued](#how-bitcoin-is-valued)
    - [Compared to Gold](#compared-to-gold)
    - [Compared to Bonds](#compared-to-bonds)
    - [Global Reserve Asset](#global-reserve-asset)
3. [Risks](#risks)
    - [Software Bugs](#software-bugs)
    - [Global Liquidation Events](#global-liquidation-events)
    - [Government Ban](#government-ban)
4. [Trading](#trading)
    - [Sats: The Smallest Unit](#sats)
    - [Fees](#fees)
    - [Taxes](#taxes)
5. [Storage](#storage)
6. [Conclusion](#conclusion)

# History
In November 2008, the pseudonymous creator of Bitcoin going by Satoshi Nakamoto, announced their invention of something called Bitcoin in the cypherpunks mailing list. He described Bitcoin as "electronic cash system that's fully peer-to-peer, with no trusted third party".

Despite the attention it's getting today, Bitcoin was ignored by many for years. The first price appeared about 1.5 years after Satoshi's announcement at a meager [$0.003 per Bitcoin](https://en.bitcoinwiki.org/wiki/Bitcoin_history#Bitcoin_price_history_2009_to_2019).

New Bitcoin is created roughly every 10 minutes by a process called mining. Bitcoin mining halves the issuance of Bitcoin to miners roughly every 4 years, creating a predictable schedule of inflation.

For the first four years, 50 Bitcoin was created every 10 minutes. For the next four years, the issuance rate is halved, just to repeat itself four years later. The event where the issuance rate is cut by half is called commonly referred to as The Halving.

|   Epoch   | Reward every 10 minutes |
|:---------:|:-----------------------:|
| 2008-2012 |            50           |
| 2012-2016 |            25           |
| 2016-2020 |           12.5          |
| 2020-2024 |           6.25          |
| 2024-2028 |          3.125          |

If you sum all of this, Bitcoin will have a little less than 21 million Bitcoin by the year May 2138 -- over 120 years from today.

While new Bitcoin will continue being issued for a while, the halvings are highly correlated with price spikes.

<figure>
<a href="https://digitalik.net/btc/"><img src="/2021/04/04/intro-to-bitcoin/s2f.gif" target="_blank"></a>
<figcaption>
<a href="https://digitalik.net/btc/" target="_blank">Stock-to-flow chart</a> on <a href="https://digitalik.net" target="_blank">digitalik.net</a> dives into this topic more deeply, attempting to model a link between the supply and the price.
</figcaption>
</figure>

# How Bitcoin is Valued

## Compared to Gold
When valuing a new type of asset, the most obvious way is to look at something similar. Since Bitcoin is often touted to be digital gold, it's no surprise we look at gold to attempt to value Bitcoin.

Physical gold has long been the non-sovereign store of value without counter-party risk. Although the gold standard was severed in 1971, central banks today still buy gold. Gold's current market cap is roughly $10 trillion, the exact number being difficult to determine.

Bitcoin's current market cap is $1.2 trillion, and for Bitcoin to reach gold's market cap it would have to go 8.3x from here, or from $60,000 per Bitcoin to $498,000 per Bitcoin.

Even if Bitcoin reaches gold levels and not higher, the upside potential is massive, cementing Bitcoin as the best asymmetric bet one can take today.

Money has always been a technology, and nothing embodies this more than that money becoming software. Since Bitcoin is pure information, the shackles that limits gold have nothing to grasp onto when it comes to Bitcoin. [Settling billions of dollars](https://www.cryptopolitan.com/bitcoin-worth-4-5-billion-transferred/) worth in value can happen in an hour instead of three banking days.

## Compared to Bonds
The total bond market is roughly $100 trillion. This is the amount of debt denominated in corporate and government bonds.

As bond yields lower due to central banks printing and inflation expectations rise, many are forced to allocate at least some portion of their assets to Bitcoin that has had an average returns of 200% per year for the last 10 years.

You already see this shift happening to [private and publicly traded companies](https://bitcointreasuries.org/) and [insurance companies](https://seekingalpha.com/news/3671187-new-york-life-ceo-ted-mathas-warms-to-bitcoin-joins-nydig).

If Bitcoin received 5% percent of this *alone*, not accounting for any store of value premium taken from other assets, Bitcoin would have a market cap of $5 trillion or a little above $238,000 per Bitcoin.

## Global Reserve Asset

[Total global financial assets amount to about $400 trillion](https://www.oecd-ilibrary.org/sites/095705eb-en/index.html?itemId=/content/component/095705eb-en). If Bitcoin takes a mere 5% allocation of this, then Bitcoin would have a market cap of $20 trillion or a little less than a $1 million per Bitcoin.

Since Bitcoin is created via mining, and mining requires energy, due to the lack of physical form of Bitcoin, [many](https://gam.ai/) [entrepreneurs](https://www.upstreamdata.ca/) are catching on to the idea of mining Bitcoin using stranded energy sources.

You even have the likes of large energy players such as Norway's Aker, through their Bitcoin-focused company [Seetee](https://seetee.io), acknowledge Bitcoin's role in balancing global energy usage.

> Seetee will establish mining operations that transfer stranded or intermittent electricity without stable demand locally—wind, solar, hydro power— to economic assets that can be used anywhere. Bitcoin is, in our eyes, a load-balancing economic battery.
>
> -- Kjell Inge Røkke, [letter to shareholders](https://www.seetee.io/)

As more energy companies pour otherwise wasted energy to securing the Bitcoin network, along with the [fraying of the US global currency reserve system](https://www.lynalden.com/fraying-petrodollar-system/), there's a non-miniscule chance that energy providers that to price the energy they produce in Bitcoin. When this occurs, Bitcoin will have its petrodollar moment.

> If you own zero bitcoin right now, you are taking extreme amounts of risk.
>
> -- Greg Foss, [What Bitcoin Did postcast](https://www.whatbitcoindid.com/podcast/bitcoin-as-investment-portfolio-insurance)

# Risks

## Software Bugs
As with all software, Bitcoin is subject to bugs. Some are worse than others, and a fairly recent example is the [inflation bug](https://bitcoincore.org/en/2018/09/20/notice/).

Undoing the effects bugs such as these could involve forking the network if it has been exploited, but what's equally important is knowing when such breaches occur. This is an excellent reason for people to run their own Bitcoin nodes. With this, they may verify the supply without having to trust a third party.

## Global Liquidation Events
In March 2020, there was a global liquidation event in which people sold assets to ensure they would have enough dollars to pay for US dollar denominated debt they had. Bitcoin [plunged to about $4,000](https://www.cnbc.com/2020/03/13/bitcoin-loses-half-of-its-value-in-two-day-plunge.html) from $10,000. Since Bitcoin markets are on 24/7 and are not shut down during extreme market events, it is a good candidate as a source of liquidity. When you're desperate for dollars, you sell what you can, not what you want.

To avoid being affected by this, one can have a longer time horizon when buying Bitcoin, such as at least 5 years.

## Government Ban
One of the oldest worries of investors is having the governments ban Bitcoin. This is a tired topic, one that [has been covered](https://unchained-capital.com/blog/bitcoin-cannot-be-banned/) in greater detail than I could.

While you have had some states ban it, such as [India](https://www.forbes.com/sites/steveforbes/2021/03/18/indias-plan-to-ban-bitcoin-could-the-us-be-next/) and [Nigeria](https://dailypost.ng/2021/02/05/breaking-cbn-bans-nigerians-from-buying-selling-bitcoin-crypto/), the opposite effect occurs -- to the extent that the [price even goes higher](https://news.bitcoin.com/nigeria-crypto-ban-bitcoin-sells-for-76k-as-deposits-on-centralized-exchanges-plummet/).

Such bans beg the question: will strong states like the US ban Bitcoin?

The US government seems to be more open to Bitcoin than every before, including allowing [Coinbase to go public](https://www.marketwatch.com/story/coinbase-set-to-go-public-in-direct-listing-april-14-11617312934), [public companies to buy Bitcoin](https://bitcointreasuries.org/), furthermore, [traditional](https://www.cnbc.com/2021/02/11/bny-mellon-to-offer-bitcoin-services-a-validation-of-crypto-from-a-key-bank-in-the-financial-system.html) [banks](https://www.cnbc.com/2021/03/31/bitcoin-goldman-is-close-to-offering-bitcoin-to-its-richest-clients.html) have been getting into the scene as well.

In the Philippines, Bitcoin is recognized and regulated by the [Bangko Sentral](https://bitpinas.com/feature/list-licensed-virtual-currency-exchanges-philippines/).

# Trading

## Sats: The Smallest Unit {#sats}
One of the most common misconceptions with Bitcoin is the idea that people cannot subdivide a Bitcoin. A single Bitcoin can be subdivided into 100 million subunits called Satoshis, or "sats" for short.

Since there will only be 21 million Bitcoin that will ever exist, this is absolutely integral to be able to ensure that everyone can theoretically own at least a fraction of a Bitcoin.

## Fees
Bitcoin trades like other commodities, through over-the-counter, peer-to-peer, and order book exchanges. Each of these have their version of a fee applied depending on local market conditions.

## Taxes
When you sell Bitcoin, some jurisdictions require you to pay capital gains, while [others do not](https://www.forbes.com/sites/kellyphillipserb/2019/09/19/portugal-tax-authorities-clarify-that-buying-or-selling-cryptocurrency-is-tax-free/).

In the Philippines, I am not aware of anything declared by the BIR.

# Storage
Even through Bitcoin is a digital, non-physical asset, storage of Bitcoin means proper storage of keys. These keys behave like long, secure passwords that give the bearer the ability to send Bitcoin to someone else. There are two types of storage:

- **Non-custodial**. In this scenario, you control the key (or keys) required to send Bitcoin out.
- **Custodial**. You need to ask someone else to send the Bitcoin for you. In the past several years, the infrastructure in this area has grown tremendously, allowing institutions to give custody of their assets to companies such as [Anchorage](https://anchorage.com/).

Although security is not an easy subject, custody of large of amounts of Bitcoin is much easier and cheaper than storing the equivalent in gold. Wallet software such as [Specter Desktop](https://specter.solutions/) make multi-signature (require more than one key to send Bitcoin out) wallets much easier to create, utilizing [signing](https://coldcardwallet.com/) [devices](https://cobo.com/hardware-wallet/cobo-vault) (a.k.a. hardware wallets) that store these secret keys away from potential hackers' prying eyes on machines connected to the Internet.

# Conclusion
While no one will ever understand Bitcoin in its entirety, being able to understand it enough requires hundreds, perhaps even thousands of hours devouring content.

> Owning bitcoins is one of the few asymmetric bets that people across the entire world can participate in. Much like a call option, an investor’s downside is limited to 1x, while their potential upside is still 100x or more.
>
> -- Vijay Voyapati on [The Bullish Case for Bitcoin](https://vijayboyapati.medium.com/the-bullish-case-for-bitcoin-6ecc8bdecc1)

This article only touches the surface of Bitcoin. If you feel like I should have covered something here, or wish that I write about something else, please email me: ramon at tayag.net.
