# colocation cost: What You'll Actually Pay Per Month, the Fees Nobody Advertises, and Where Sharktech's $79 Entry Price Fits In

Most "colocation cost" searches hit the same wall: a dozen articles that say "it depends" and then list pricing factors without committing to a number. So here are numbers first.

For a single 1U server, retail colocation in a tier-1 US market typically starts around **$85–150 per month**, with limited power and bandwidth. A full 42U cabinet in those same markets commonly runs **$1,000–2,000+ per month** once you factor in roughly 5 kW of power and meaningful bandwidth. On the wholesale side, primary North American markets averaged about **$196.25 per kW per month** for 250–500 kW deployments in late 2025, per CBRE data.

Against that backdrop, Sharktech's published colocation pricing — **1–6U from $79/month, 10–42U full cabinets from $449/month**, both with 10–100Gbps ports, 300TB+ of traffic, and DDoS protection included — lands at the low end of the retail range, and its cabinet floor sits well below the tier-1 entry point.

> **Quick pick:** Housing one or a few servers? Sharktech's 1–6U tier starting at **$79/month** is the relevant option. Filling a rack? The 10–42U tier from **$449/month** with up to 5500W is the one to price out. Both include DDoS protection and five data center locations. 👉 [Check Sharktech's current colocation plans and pricing](https://bit.ly/SharKtech)

## What Colocation Actually Costs Across the Market

Colocation means you own the hardware and rent space, power, cooling, and network in someone else's facility. Costs stack in three layers, and most articles only explain the first one.

The monthly lease is the number everyone quotes — $85–150 for 1U in tier-1 markets, per-cabinet or per-kW pricing above that. Power is where the real bill lives. TRG Datacenters' cost guide breaks the billing into two models: *provisioned power* (a fixed kW reservation you pay for whether you use it or not) and *metered power* (billed per kWh consumed). Redundancy choices move the number too — a single-feed (N) circuit costs less than dual-feed A+B (2N), which a lot of production workloads end up wanting anyway.

Then there's everything else. A typical enterprise deployment of 100 kW in a primary US market runs roughly $12,000–16,000/month for the base lease alone, plus $500–800/month in metered power, $150–500/month per cross-connect (deployments typically need 4–20 of them), and $75–150/hour for smart hands support. Those add-ons, not the lease, are where budgets usually blow up.

Location quietly shapes all of it. Commercial electricity prices vary enormously by state and get passed through to you: as of mid-2026, Texas commercial power ran about 8.47¢/kWh while Illinois hit 15.19¢/kWh, up 11.2% in a year. Ohio and Virginia both climbed around 20% over the same period. Second-tier markets also price 30–50% below tier-1 cities for equivalent space, before you even get to provider-specific deals.

## What Drives the Price of a Colocation Plan

Four things determine your bill, in rough order of impact:

1. **Space (rack units).** 1U for a single server, a partial or full cabinet for serious deployments, a private cage if you need physical separation.
2. **Power draw.** A typical 1U server pulls 200–400W; a loaded cabinet draws 3–5 kW; high-density GPU racks can demand 10–20 kW or more. Over-provisioning power is the most common way people overpay — you're reserving capacity you never touch.
3. **Bandwidth model.** Some plans bundle a fixed transfer allowance (say 300TB) and charge overages; others sell unmetered ports at a fixed speed. Unmetered sounds better until you notice the port speed caps your actual throughput at a hard ceiling.
4. **Location.** Electricity costs plus plain market dynamics. Chicago, for instance, prices noticeably below coastal metros.

Worth knowing the alternative math too: Uptime Institute research found colocation can be 19–64% more cost-effective than building your own Tier 2 data center. That gap only holds if you size the deployment to your actual load, though.

## Sharktech's Colocation Plans and Pricing

Sharktech currently publishes two colocation tiers, and the network portion is identical on both: 10–100Gbps connectivity with traffic starting at 300TB, on a DDoS-protected, multi-100-Gigabit redundant backbone. The tiers differ only in space and power envelope.

| 方案 | 机架空间 | 电力范围 | 网络与流量 | 起步价 | 购买入口 |
| --- | --- | --- | --- | --- | --- |
| 1–6U 托管 | 1–6U | 200–1200W | 10–100Gbps，流量自 300TB 起，含 DDoS 防护 | $79/月 | [ 查看当前 1–6U 托管报价](https://bit.ly/SharKtech) |
| 10–42U 整柜 | 10–42U（部分或整机柜） | 1600–5500W | 10–100Gbps，流量自 300TB 起，含 DDoS 防护 | $449/月 | [ 查看 10–42U 整柜报价](https://bit.ly/SharKtech) |

Anything beyond these tiers — partial cabinets, custom power densities, private cages, multi-rack builds — goes through the sales team as an itemized quote.

Here's the part the headline pricing doesn't spell out: the same two tiers are priced differently by location. Several recent third-party listings of Sharktech's plans report this breakdown:

| 地点 | 1–6U 起价 | 10–42U 整柜起价 |
| --- | --- | --- |
| Chicago | $35/月 | $280/月 |
| Las Vegas | $65/月 | $520/月 |
| Denver | $65/月 | $520/月 |
| Los Angeles | $99/月 | $792/月 |
| Amsterdam | $99/月 | $792/月 |

Treat this table as directional. The official colocation page currently headlines "from $79" without publishing the per-location split, and multiple independent listings (which do agree with each other on the numbers) carry the usual caveat that you should confirm current pricing at the order portal before budgeting. The pattern itself is consistent, though: Chicago is the sharpest-priced market, and the spread between cheapest and most expensive locations reaches roughly 65% on identical hardware specs.

The pricing logic matters for your decision. Every plan includes the same network capacity, the same 300TB+ traffic pool, and the same DDoS protection — the price differences come from location and power allowance. You're paying for geography and watts, nothing else.

Third-party listings also report a **10% discount on the first six months of new colocation contracts**, which would put Chicago's 1–6U tier around $31.50/month during that window. This hasn't appeared on the official pricing page itself, so treat it as something to confirm with sales rather than something to budget around.

## The Hidden Costs Most Colocation Cost Guides Skip

Sticker price rarely equals invoice. These are industry-standard line items that almost never make it into the advertised number:

- **Power overages.** Exceed your allocated wattage and overage penalties kick in. This is why quoting your hardware's realistic draw — not the PSU's rated maximum — matters more than almost anything else.
- **Cross-connects.** Every direct connection to a specific carrier or network bills monthly, commonly $150–500 each, and enterprise deployments routinely need 4–20. At the high end that's thousands per month on its own.
- **IP assignments.** Plans typically include a small subnet (often a /29, or 5 usable IPs); allocations beyond that cost extra.
- **Setup and installation.** Rack-and-stack labor and initial provisioning are frequently one-time charges.
- **After-hours smart hands.** A Sunday 2 AM reboot falls into the $75–150/hour range at many providers unless you've negotiated a support tier.
- **Contract escalators.** Annual increases of 2–5% are common, which compounds meaningfully on a three-year term.

Two Sharktech-specific notes here. First, DDoS protection is bundled rather than upsold: listings describe free 40 Gbps protection baked into every colocation plan, with the company reporting 300Gbps+ of mitigation capacity per location — a meaningful point given that standalone DDoS protection services run $50 to several hundred dollars monthly, and Sharktech has been in the DDoS protection business since it started in 2003. Second, a review caveat: Sharktech's Trustpilot rating sits at 3.4/5 from a small sample of 13 reviews. Recent ones lean positive on reliability and support, but older reviews mention billing friction — specifically that when you cancel, you need to terminate the PayPal subscription yourself. Boring detail, genuinely useful to know.

## Running the Real Numbers: First-Year Cost

Sticker prices mislead because billing cycles and locations differ, so here's straightforward math using the published figures.

Single server, 1–6U tier: at $79/month you're at about **$948 for the first year**. The same unit in a tier-1 market at the typical $85–150/month runs $1,020–1,800. And if the third-party Chicago price holds at $35/month, that's roughly $420 a year — lower than a lot of entry-level VPS plans, except you're bringing your own enterprise hardware.

Full cabinet, 10–42U tier: at the Los Angeles/Amsterdam price of $792/month you're at about **$9,500 in year one**, with up to 5500W and 300TB+ of traffic included. Comparable retail cabinets in primary markets commonly start around $1,000–2,000+ per month once power and bandwidth are factored in, so the gap runs roughly $200–1,200 monthly — $2,400 to $14,000+ over a year. Even against Chicago's wholesale rate of $200–230 per kW per month, a 5 kW allocation alone would run $1,000–1,150 before space and bandwidth; Sharktech's $280 full-cabinet price in that market undercuts the power line item by itself.

One caution on the headline comparisons: wholesale per-kW rates and retail cabinet rates aren't the same product (wholesale assumes you're taking 250+ kW), so use them as context, not as a like-for-like quote.

## Who Colocation Makes Sense For — and Who Should Skip It

Colocation pays off under specific conditions and wastes money under others.

It makes sense if you **already own the hardware** and want enterprise-grade power redundancy, cooling, and network without building a facility. Sharktech's setup fits that use case directly: its facilities sit inside Equinix, CoreSite, H5 Data Centers, and CrownCastle campuses, with fully redundant power, backup generators, 24/7 on-site engineers, and a 99.99% uptime SLA per third-party listings. It also makes sense when you need **control cloud can't give you** — specific GPUs, unusual storage, licensing tied to physical machines. The company's own displayed reviews come from exactly these users: gaming operators surviving multi-gigabit DDoS attacks, an ISP praising flexible custom configs, a five-year customer who originally chose them on price. Sharktech claims over 10,000 business customers, though that's the company's own figure.

Skip colocation if you **don't have hardware yet**. Buying servers plus paying monthly colocation rarely beats renting a dedicated server unless you have a concrete reason to own the metal. It also stops making sense on very short timelines — the logistics of shipping hardware and coordinating installation eat the savings if you're out in six months. And if your workload needs to be near a specific metro for latency or peering reasons, pay the location premium knowingly; if it doesn't, the premium is just a premium.

## How Ordering Works

The flow is standard, with two steps worth getting right:

1. **Pick your location.** This is the biggest price lever given the spread above. Weigh where your users and network carriers are.
2. **Configure in the customer portal.** You select space, power, and connectivity and see a full quote — including any installation or remote-hands charges — before ordering. Have your hardware's actual power draw ready.
3. **Coordinate shipping before anything moves.** The official page emphasizes this explicitly. Send rack units, power draw, port requirements, and expected growth to the team, then arrange delivery and rack installation with them.
4. **Specify network details upfront.** Port speeds, bandwidth commitments, cross-connects, and routing are all set at this stage. Adding a cross-connect later costs more than specifying it in the quote.

Custom builds (cages, higher densities, multiple racks) follow the same path except the quote comes itemized from sales.

## FAQ

**How much does 1U colocation cost per month?**
In tier-1 US markets, typically $85–150/month. Sharktech's published starting price is $79/month for its 1–6U tier, and third-party listings report as low as $35/month at its Chicago location.

**Is colocation cheaper than cloud?**
For steady, predictable workloads on hardware you already own, usually yes over a multi-year horizon. Cloud wins on elasticity — if usage spikes and crashes, paying for reserved rack space means paying for idle capacity. Uptime Institute's research framing (19–64% savings versus self-building a Tier 2 facility) applies to the colocation-versus-DIY question, not the colocation-versus-cloud question.

**Does the Sharktech price include bandwidth and DDoS protection?**
Yes on both counts: every plan includes traffic starting at 300TB on a 10–100Gbps port, plus DDoS-protected connectivity. Listings describe 40 Gbps of free protection per plan, with 300Gbps+ mitigation capacity per location per the company.

**Is Sharktech reliable?**
The company reports 10,000+ business customers, and its Trustpilot rating is 3.4/5 from 13 reviews — recent ones positive on uptime and support, older ones flagging a self-service PayPal cancellation step at billing. Small sample, so read it as a data point rather than a verdict.

## Before You Order

Match your situation to the plan:

- **One to a few owned servers, watching the budget:** the 1–6U tier, and ask about Chicago first — the reported $35/month price is the single biggest saving on the board if latency allows.
- **A rack's worth of hardware:** price the 10–42U cabinet against your realistic power draw. If your gear totals under 5500W, the included allowance covers you without metered-power surprises.
- **Cages, high density, or multiple racks:** skip the published tiers and request an itemized quote — the published pricing is a floor, and custom power is where over-provisioning creeps in.

Two things to nail down before clicking buy: your hardware's realistic wattage (not the PSU rating) and your cross-connect count, because those two numbers decide whether the invoice matches the quote. If you're asked about a first-six-months discount, mention it — the 10% offer is worth confirming even if the rep hasn't volunteered it. When you're ready to price your actual configuration, 👉 [open Sharktech's colocation plans and get a quote for your hardware](https://bit.ly/SharKtech).
