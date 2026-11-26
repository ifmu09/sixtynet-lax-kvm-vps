# Los Angeles KVM VPS: SixtyNet's LAX Plans Start at $200/Year — Which Tier Fits, and How the Price Compares

SixtyNet's cheapest Los Angeles KVM plan is **LAX-STARTER**: 2 cores, 2GB RAM, 40GB NVMe, 5TB of traffic and DDoS protection, listed at **$200 per year** against a $240 list price. That is roughly $16.67 a month, except you pay the whole year up front, so the decision is really whether you want to send $200 before you have pinged the box once.

Below: the full LAX plan table, what the same money buys from other Los Angeles KVM hosts, how to check that "LA" and "KVM" are both true, and the terms worth confirming in writing before you pay for twelve months.

> **The short version.** Every SixtyNet LAX tier costs exactly $100 per gigabyte of RAM per year, so there is no bulk discount for going bigger. Start with **LAX-STARTER at $200/year** if you need a small web node, VPN exit or Docker sandbox; move to **LAX-MICRO at $400/year** only when 4GB is a real requirement.
> 👉 [See the current LAX plan pricing at SixtyNet](https://sixtynet.net/aff.php?aff=39)

## SixtyNet Los Angeles KVM plans

| Plan | vCPU / RAM / NVMe | Traffic and network | Price (billed annually) | Order |
| --- | --- | --- | --- | --- |
| LAX-STARTER | 2 cores / 2GB / 40GB, 12,500 IOPS | 5TB, "2G Premium Network" | $200/yr (list $240) | [LAX-STARTER](https://sixtynet.net/aff.php?aff=39) |
| LAX-MICRO | 4 cores / 4GB / 80GB, 12,500 IOPS | 10TB, "4G Premium Network" | $400/yr (list $480) | [LAX-MICRO](https://sixtynet.net/aff.php?aff=39) |
| LAX-MEDIUM | 8 cores / 8GB / 160GB, 25,000 IOPS | 20TB, "10G Premium Network" | $800/yr (list $960) | [LAX-MEDIUM](https://sixtynet.net/aff.php?aff=39) |
| LAX-LARGE | 8 cores / 16GB / 320GB, 25,000 IOPS | 40TB, "10G Premium Network" | $1,600/yr (list $1,920) | [LAX-LARGE](https://sixtynet.net/aff.php?aff=39) |

All four include DDoS protection. The two smaller plans get 12,500 IOPS and a "2G"/"4G" premium network; the two larger ones step up to 25,000 IOPS and a "10G" network. The page does not say whether those network figures are guaranteed port speeds or burst ceilings, and it does not specify whether the traffic allowance resets monthly or yearly. Both are worth an email before you commit.

The pricing scales in a straight line. RAM doubles each tier and the price doubles with it, storage stays at a flat 20GB per gigabyte of RAM, and traffic stays at 2.5TB per gigabyte of RAM. Only the core count breaks the pattern: LAX-LARGE doubles RAM and disk over LAX-MEDIUM but keeps 8 cores. If you need 16GB, you are paying for memory and bandwidth, not for more CPU.

### Other products on the same page

Three more lines sit alongside the LAX plans:

- **Los Angeles China Unicom-Premium**, $2,500/year against a $3,000 list price. It is sold on AS9929 China Unicom routing, a 100M base port with 3x burst, 95th-percentile billing and free BGP session setup. The plan summary does not publish CPU or RAM figures for it, so it is a network product you would spec with sales rather than a self-serve tier.
- **A residential-IP line** in four sizes (2 cores/2GB/40GB through 16 cores/16GB/320GB, 5TB to 40TB of traffic). These explicitly **cannot open ports 80 and 443** for IP risk-control reasons. They exist for scrapers, ad verification and account work, not for hosting a website.
- **A 4-core/4GB configuration** with 300GB RAID 10 plus 200GB bonus disk, 10TB of traffic and DDoS protection. Price is not shown in the public plan summary.

## What $200 a year buys elsewhere in Los Angeles

Los Angeles KVM is a crowded, cheap market. The entry point from established hosts sits between **$4.99 and $7.99 a month**, and SixtyNet's floor is three times that in monthly terms because it only sells annually.

| Provider and plan | Specs | Price | Annualized |
| --- | --- | --- | --- |
| Owned-Networks LA-KVM-512MB | 1 vCPU / 512MB / 20GB / 1TB / 1Gbps | $4.99/mo | $59.88 |
| Owned-Networks LA-KVM-1GB | 1 vCPU / 1GB / 20GB / 1TB / 1Gbps | $7.99/mo | $95.88 |
| Owned-Networks LA-KVM-2GB | 2 vCPU / 2GB / 40GB / 2TB / 1Gbps | $17.99/mo | $215.88 |
| SpeedyKVM LAX 1 Core | 1 vCPU / 2GB / 60GB / 3TB | $12.10/mo | $145.20 |
| SpeedyKVM LAX 2 Core | 2 vCPU / 4GB / 85GB / 5TB | $24.20/mo | $290.40 |
| SpeedyKVM LAX 6 Core | 6 vCPU / 16GB / 320GB / 6TB | $96.80/mo | $1,161.60 |
| DediRock LA KVM VPS Starter | specs not published on its LA page | $7.99/mo | $95.88 |
| **SixtyNet LAX-STARTER** | **2 cores / 2GB / 40GB / 5TB** | **$200/yr** | **$200** |

Compare the 2GB bracket. SpeedyKVM sells 2GB with one core, 60GB of disk and 3TB of traffic for $145.20 a year. SixtyNet charges $200 for the same 2GB with two cores, 40GB of disk and 5TB of traffic. You pay about $55 more per year for one extra core and two extra terabytes, and you lose 20GB of disk.

Against Owned-Networks, SixtyNet looks better than it first appears. That host's 2GB plan costs $215.88 a year, more than SixtyNet's Starter, with half the traffic and a 1Gbps port instead of the "2G" label. Owned-Networks bills monthly, though, so you can walk away after one month. SixtyNet asks for the year in one payment.

The gap widens as you go up. At 4GB, SpeedyKVM is $290.40 a year against SixtyNet's $400. At 16GB, SpeedyKVM is $1,161.60 against $1,600. SixtyNet is consistently 35 to 40 percent above the cheapest LA KVM host in each bracket. What it puts on the table in exchange is traffic allowance: 5TB to 40TB, against 3TB to 6TB from SpeedyKVM and 1TB to 6TB from Owned-Networks, plus DDoS protection listed on every tier. If your workload is bandwidth-heavy (mirrors, media, backup targets, proxying), that trade can work. If it is CPU- or RAM-bound, you are paying a premium for capacity you will not use.

👉 [Check what the 4-core LAX-MICRO costs today](https://sixtynet.net/aff.php?aff=39)

## How to confirm the box is really in Los Angeles and really KVM

Two things get faked in this market: the location and the virtualization layer.

**Location.** The check that costs nothing: ask for a test IP or a looking glass before you pay, then run whois on the IP and ping it from where your users actually are. A route through a resold rack two time zones away shows up immediately in the traceroute. Hosts with nothing to hide publish the datacenter address. RackNerd, for example, lists its LA DC-03 facility at 1200 W 7th St in downtown Los Angeles, along with its two upstream carriers and a public test point. That is the standard to hold any "Los Angeles" claim against. If a host will not give you an IP to ping, treat the location as unverified. SixtyNet's plan page does not publish a test IP, so ask support for one.

**Virtualization.** KVM gives you a real kernel. That means full root, your own kernel version, custom ISO boot, and the ability to run Docker, WireGuard or a Windows image if the host licenses it. OpenVZ containers share the host kernel, so you cannot change it, cannot boot an ISO, and typically cannot run Docker without workarounds. If a host advertises "KVM" but will not let you boot a custom ISO or check `dmesg` for hardware virtualization flags, the claim is worth questioning. SixtyNet lists full root-level KVM configurations and DDoS protection but does not publish its OS template list or a Windows option; confirm both if either matters to you.

There is also a routing detail specific to this provider. The LAX plans are the general-purpose ones. The China Unicom-Premium product at $2,500 a year is a separate, AS9929-routed service aimed at mainland China latency, sold with 95th-percentile billing and BGP sessions. If your visitors are in Asia and the route matters more than the specs, that is the product line you would ask about. If your visitors are in California, the standard LAX tiers are the relevant ones.

## The money: annual-only billing, renewal, and refunds

Three things to settle before paying.

**Billing cycle.** The four LAX tiers are listed as annual only. There is no monthly price on the page. That removes the usual escape hatch: with a $12-a-month host you can abandon a bad box after 30 days for $12; here a bad first month costs $200.

**Renewal price.** The page shows a $240 list price struck through to $200, labelled "Save 17%". It does not state whether renewal lands at $200 or snaps back to $240. Ask support to confirm the renewal amount in writing, because a $40 difference compounds quietly over three years.

**Refunds.** The LAX plan page does not spell out a refund window. One third-party write-up about SixtyNet reports a three-day money-back window on the account, which is short by any standard, and notes that refunds on some residential products are issued as site credit rather than cash. Treat both as unconfirmed until support answers, and get the answer before you pay. A host that will not put a refund term in a ticket is telling you something.

👉 [Read the plan terms and current pricing before you pay for a year](https://sixtynet.net/aff.php?aff=39)

## Who should not buy this

- **You want a $5 to $8 a month box.** Owned-Networks starts at $4.99 and DediRock lists a $7.99 starter. SixtyNet's floor is $200 charged at once.
- **You want to try before committing.** No monthly option on the LAX tiers means no cheap trial month.
- **You need a public website and were looking at the residential-IP plans.** Ports 80 and 443 are closed on those by policy. The LAX plans are the web-hosting ones.
- **You need a contractual SLA and a long public track record on this specific location.** Budget LA KVM providers rarely publish either, and SixtyNet's LAX page does not.
- **You need the lowest price per core.** SpeedyKVM undercuts SixtyNet at every bracket, and Owned-Networks offers custom configurations beyond its listed plans.

## FAQ

**Will LAX-STARTER run WordPress?**
Yes, for a small site with a caching layer and modest traffic. 2GB of RAM and 2 cores handle WordPress plus MySQL comfortably at low concurrency. WooCommerce, heavy plugin stacks or multiple sites push you to LAX-MICRO at 4GB.

**Can I install Windows?**
KVM supports it technically, but SixtyNet's plan page lists no Windows option or licensing terms. Ask before buying if Windows is the point.

**What happens if I exceed 5TB of traffic?**
Not stated. The page lists "5TB traffic" without saying whether that is monthly or annual, or whether overage means throttling, overage billing or suspension. Get the answer in writing, because 5TB a month and 5TB a year are very different products.

**Can I upgrade to a bigger plan later?**
Not documented on the plan page. Ask whether upgrades are prorated mid-term or only at renewal.

**How fast is setup?**
Not stated on the LAX page. Some Los Angeles hosts advertise provisioning in minutes; SixtyNet does not make that claim here, so confirm the deployment window if you are migrating on a deadline.

## Picking a tier

Match the tier to the constraint that actually binds you:

- A static site, a VPN exit, a bot, a monitoring node: **LAX-STARTER, $200/year**. 2GB is more than these need.
- Docker with a database, a mid-size WordPress install with caching, a small API: **LAX-MICRO, $400/year**. 4GB is the floor for that stack.
- Multiple containers, a game server, real production traffic: **LAX-MEDIUM, $800/year**. Below 8GB you will be tuning instead of shipping.
- Bandwidth-heavy work where 20TB is not enough: **LAX-LARGE, $1,600/year**. Note that you are buying RAM, disk and traffic here, not more cores.

Before you pay, get two answers in writing: whether renewal is $200 or $240, and whether the 5TB (or 10TB, 20TB, 40TB) allowance resets monthly. Both change the real annual cost, and neither is on the page.

👉 [Start with the LAX-STARTER plan at SixtyNet](https://sixtynet.net/aff.php?aff=39)
