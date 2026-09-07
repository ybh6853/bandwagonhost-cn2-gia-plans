# cheap cn2 gia vps: BandwagonHost plans compared, from $49.99/year limited editions to premium Hong Kong lines

You typed "cheap cn2 gia vps" into the search box, which means you probably want one of two things: either the cheapest possible VPS that runs on China Telecom's CN2 GIA backbone, or a clear answer on whether the cheap CN2 GIA options are actually usable versus the expensive ones. Both questions are legitimate, and the gap between them is wider than most providers admit.

CN2 GIA (Global Internet Access, AS4809) is China Telecom's premium transit tier. It is the most stable route between China and overseas datacenters, with the lowest packet loss during peak hours — and also the most expensive transit you can buy (raw IP transit on this network can run up to roughly $120 per Mbps in some markets, per BandwagonHost's own explainer). That cost structure is why truly "cheap" CN2 GIA VPS plans are almost always either limited editions, low-configuration boxes, or based in Los Angeles rather than Hong Kong/Tokyo. There is no secret cheap Hong Kong CN2 GIA with full bandwidth; if someone is selling one, read the fine print.

This article walks through what CN2 GIA actually is, where BandwagonHost (the brand behind bwh81.net) fits in, every currently-sold plan in their CN2 GIA family with verified prices and product IDs, and how to pick between the $49.99/year limited editions and the $89.99/month Hong Kong premium line.

## What CN2 GIA actually is — and why "cheap" is relative

China Telecom operates several tiers of China-bound transit. The common one, AS4134 (ChinaNet/163), is cheap and high-capacity but congested during peak hours, with packet loss that can spike above 30% — enough to break web conferencing, gaming, and reliable content delivery. CN2 GT (AS4809 Global Transit) was meant to fix this but, per BandwagonHost's own network page, has been roughly as congested as ChinaNet since 2019 despite costing more.

CN2 GIA (AS4809 Global Internet Access) is the top tier. It is the route you want for VOIP, web conferencing, serving content to Chinese visitors, online gaming, or any scenario where packet loss and jitter matter more than raw megabits. BandwagonHost also treats the newer CTGNet (AS23764) as practically equivalent to CN2 GIA in both pricing and performance.

The trade-off: CN2 GIA has very limited capacity and is not DDoS-tolerant. BandwagonHost explicitly notes they have to null-route IPs under attack on this network because there is no headroom to absorb it. So "cheap CN2 GIA" always means you are sharing a constrained, expensive pipe — and the cheap plans are correspondingly small.

## BandwagonHost's CN2 GIA footprint

BandwagonHost runs CN2 GIA / CTGNet across several locations:

- **Los Angeles DC6 (CN2 GIA-E)** — the workhorse. E-Commerce plans here start at $49.99/quarter and are the sweet spot for price-to-performance.
- **Los Angeles DC9 (CN2 GIA)** — similar performance to DC6, slightly different peering mix; both send China-bound traffic via CN2 GIA (AS4809), CMIN2 (China Mobile AS58807), and China Unicom Premium (AS10099).
- **Hong Kong** — Equinix IX, Google, Cloudflare, RETN, NTT, China Mobile, CN2 GIA peering. Lowest latency to mainland China, but the most expensive: plans start at $89.99/month.
- **Tokyo (CN2 GIA)** — 1.2 Gbps link, same pricing tier as Hong Kong.
- **Osaka (CN2 GIA)** — 1.5 Gbps link, slightly cheaper than HK/Tokyo at $49.99/month entry.
- **Singapore (SG_8, CN2 GIA)** — new in 2026, three-network CN2 GIA return path, from $49.99/month.

Any E-Commerce or Ultra (HK/Japan/Singapore) plan can be migrated between datacenters at any time free of charge, without data loss, via the KiwiVM panel. This matters a lot for the cheap CN2 GIA-E plans: you buy one box and you can hop between DC6, DC9, the Japan Softbank node, and the Netherlands Unicom node as availability and performance shift.

## The full CN2 GIA plan lineup (verified from current stock)

BandwagonHost's CN2 GIA offerings are split into three families: the **CN2 GIA-E E-Commerce** series (Los Angeles-based, migratable to ~15 datacenters), the **Ultra** series (Hong Kong / Tokyo / Osaka / Singapore, premium latency), and a rotating set of **limited edition** plans that are the actual "cheap CN2 GIA vps" most people are hunting for.

Prices below are pulled from the live stock page (stock.bwg.net) and the official order pages as of this writing. Limited editions are mostly out of stock at any given moment — that is by design. I've marked stock status where relevant.

### CN2 GIA-E E-Commerce plans (Los Angeles, migratable)

These are the mainstream CN2 GIA plans. The entry tier bills quarterly at $49.99/3-month (≈ $169.99/year equivalent), not annually — the cheapest annual CN2 GIA-E box is the limited edition, covered below.

| Plan | CPU | RAM | Storage | Monthly transfer | Link speed | Billing | Price | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| CN2 GIA-E 20G | 2 cores | 1 GB | 20 GB RAID-10 SSD | 1 TB | 2.5 Gbps | Quarterly+ | $49.99 / 3 mo | [Get CN2 GIA-E 20G](https://bwh81.net/aff.php?aff=77528&pid=87) |
| CN2 GIA-E 40G | 3 cores | 2 GB | 40 GB RAID-10 SSD | 2 TB | 2.5 Gbps | Quarterly+ | $89.99 / 3 mo | [Get CN2 GIA-E 40G](https://bwh81.net/aff.php?aff=77528&pid=88) |
| CN2 GIA-E 80G | 4 cores | 4 GB | 80 GB RAID-10 SSD | 3 TB | 2.5 Gbps | Monthly+ | $56.99 / mo | [Get CN2 GIA-E 80G](https://bwh81.net/aff.php?aff=77528&pid=89) |
| CN2 GIA-E 160G | 6 cores | 8 GB | 160 GB RAID-10 SSD | 5 TB | 5 Gbps | Monthly+ | $86.99 / mo | [Get CN2 GIA-E 160G](https://bwh81.net/aff.php?aff=77528&pid=90) |
| CN2 GIA-E 320G | 8 cores | 16 GB | 320 GB RAID-10 SSD | 8 TB | 5 Gbps | Monthly+ | $159.99 / mo | [Get CN2 GIA-E 320G](https://bwh81.net/aff.php?aff=77528&pid=91) |
| CN2 GIA-E 640G | 10 cores | 32 GB | 640 GB RAID-10 SSD | 10 TB | 10 Gbps | Monthly+ | $289.99 / mo | [Get CN2 GIA-E 640G](https://bwh81.net/aff.php?aff=77528&pid=92) |
| CN2 GIA-E 1280G | 12 cores | 64 GB | 1280 GB RAID-10 SSD | 12 TB | 10 Gbps | Monthly+ | $549.99 / mo | [Get CN2 GIA-E 1280G](https://bwh81.net/aff.php?aff=77528&pid=93) |
| CN2 GIA-E 1280G 15T | 12 cores | 64 GB | 1280 GB RAID-10 SSD | 15 TB | 10 Gbps | Monthly+ | $679.00 / mo | [Get CN2 GIA-E 1280G 15T](https://bwh81.net/aff.php?aff=77528&pid=160) |
| CN2 GIA-E 1280G 20T | 12 cores | 64 GB | 1280 GB RAID-10 SSD | 20 TB | 10 Gbps | Monthly+ | $899.00 / mo | [Get CN2 GIA-E 1280G 20T](https://bwh81.net/aff.php?aff=77528&pid=161) |

The 20G and 40G tiers bill quarterly, semi-annually, or annually (annual works out cheapest per month). From 80G upward it's monthly billing. All of these can live in DC6 CN2 GIA-E, DC9 CN2 GIA, San Jose CN2 GIA, New York CN2 GIA, Vancouver CN2 GIA, Japan Softbank (JPOS_1), Netherlands Unicom (EUNL_9), and several other datacenters — you pick in KiwiVM and migrate for free.

### Ultra plans — Hong Kong, Tokyo, Osaka, Singapore (lowest latency, highest price)

These are the no-compromise latency plans. Same RAID-10 SSD storage, KVM virtualization, KiwiVM panel. The difference is location and link speed.

| Location | Entry plan | CPU/RAM/Storage/Transfer | Link | Entry price | Buy |
| --- | --- | --- | --- | --- | --- |
| Hong Kong | HK CN2 GIA 40G | 2c / 2GB / 40GB / 500GB | 1 Gbps | $89.99 / mo | [Get HK CN2 GIA 40G](https://bwh81.net/aff.php?aff=77528&pid=95) |
| Hong Kong | HK CN2 GIA 80G | 4c / 4GB / 80GB / 1TB | 1 Gbps | $155.99 / mo | [Get HK CN2 GIA 80G](https://bwh81.net/aff=77528&pid=96) |
| Hong Kong | HK CN2 GIA 160G | 6c / 8GB / 160GB / 2TB | 1 Gbps | $299.99 / mo | [Get HK CN2 GIA 160G](https://bwh81.net/aff.php?aff=77528&pid=97) |
| Hong Kong | HK CN2 GIA 320G | 8c / 16GB / 320GB / 4TB | 1 Gbps | $589.99 / mo | [Get HK CN2 GIA 320G](https://bwh81.net/aff.php?aff=77528&pid=98) |
| Hong Kong | HK CN2 GIA 640G | 10c / 32GB / 640GB / 6TB | 1 Gbps | $989.99 / mo | [Get HK CN2 GIA 640G](https://bwh81.net/aff.php?aff=77528&pid=122) |
| Hong Kong | HK CN2 GIA 1280G | 12c / 64GB / 1280GB / 8TB | 1 Gbps | $1,889.99 / mo | [Get HK CN2 GIA 1280G](https://bwh81.net/aff.php?aff=77528&pid=124) |
| Tokyo | TOKYO CN2 GIA 40G | 2c / 2GB / 40GB / 500GB | 1.2 Gbps | $89.99 / mo | [Get Tokyo CN2 GIA 40G](https://bwh81.net/aff.php?aff=77528&pid=108) |
| Tokyo | TOKYO CN2 GIA 80G | 4c / 4GB / 80GB / 1TB | 1.2 Gbps | $155.99 / mo | [Get Tokyo CN2 GIA 80G](https://bwh81.net/aff.php?aff=77528&pid=109) |
| Tokyo | TOKYO CN2 GIA 160G | 6c / 8GB / 160GB / 2TB | 1.2 Gbps | $299.99 / mo | [Get Tokyo CN2 GIA 160G](https://bwh81.net/aff.php?aff=77528&pid=110) |
| Tokyo | TOKYO CN2 GIA 320G | 8c / 16GB / 320GB / 4TB | 1.2 Gbps | $589.99 / mo | [Get Tokyo CN2 GIA 320G](https://bwh81.net/aff.php?aff=77528&pid=111) |
| Tokyo | TOKYO CN2 GIA 640G | 10c / 32GB / 640GB / 6TB | 1.2 Gbps | $989.99 / mo | [Get Tokyo CN2 GIA 640G](https://bwh81.net/aff.php?aff=77528&pid=123) |
| Tokyo | TOKYO CN2 GIA 1280G | 12c / 64GB / 1280GB / 8TB | 1.2 Gbps | $1,889.99 / mo | [Get Tokyo CN2 GIA 1280G](https://bwh81.net/aff.php?aff=77528&pid=125) |
| Osaka | OSAKA CN2 GIA 40G | 2c / 2GB / 40GB / 500GB | 1.5 Gbps | $49.99 / mo | [Get Osaka CN2 GIA 40G](https://bwh81.net/aff.php?aff=77528&pid=134) |
| Osaka | OSAKA CN2 GIA 80G | 4c / 4GB / 80GB / 1TB | 1.5 Gbps | $86.99 / mo | [Get Osaka CN2 GIA 80G](https://bwh81.net/aff.php?aff=77528&pid=135) |
| Osaka | OSAKA CN2 GIA 160G | 6c / 8GB / 160GB / 2TB | 1.5 Gbps | $165.99 / mo | [Get Osaka CN2 GIA 160G](https://bwh81.net/aff.php?aff=77528&pid=136) |
| Osaka | OSAKA CN2 GIA 320G | 8c / 16GB / 320GB / 4TB | 1.5 Gbps | $329.99 / mo | [Get Osaka CN2 GIA 320G](https://bwh81.net/aff.php?aff=77528&pid=137) |
| Osaka | OSAKA CN2 GIA 640G | 10c / 32GB / 640GB / 6TB | 1.5 Gbps | $549.99 / mo | [Get Osaka CN2 GIA 640G](https://bwh81.net/aff.php?aff=77528&pid=138) |
| Osaka | OSAKA CN2 GIA 1280G | 12c / 64GB / 1280GB / 8TB | 1.5 Gbps | $1,059.99 / mo | [Get Osaka CN2 GIA 1280G](https://bwh81.net/aff.php?aff=77528&pid=139) |
| Singapore | SG CN2 GIA 40G | 2c / 2GB / 40GB / 500GB | 1.5 Gbps | $49.99 / mo | [Get SG CN2 GIA 40G](https://bwh81.net/aff.php?aff=77528&pid=173) |
| Singapore | SG CN2 GIA 80G | 4c / 4GB / 80GB / 1TB | 1.5 Gbps | $86.99 / mo | [Get SG CN2 GIA 80G](https://bwh81.net/aff.php?aff=77528&pid=174) |
| Singapore | SG CN2 GIA 160G | 6c / 8GB / 160GB / 2TB | 2.5 Gbps | $166.66 / mo | [Get SG CN2 GIA 160G](https://bwh81.net/aff.php?aff=77528&pid=175) |
| Singapore | SG CN2 GIA 320G | 8c / 16GB / 320GB / 4TB | 2.5 Gbps | $319.99 / mo | [Get SG CN2 GIA 320G](https://bwh81.net/aff.php?aff=77528&pid=176) |
| Singapore | SG CN2 GIA 640G | 10c / 32GB / 640GB / 6TB | 5 Gbps | $549.99 / mo | [Get SG CN2 GIA 640G](https://bwh81.net/aff.php?aff=77528&pid=177) |
| Singapore | SG CN2 GIA 1280G | 12c / 64GB / 1280GB / 8TB | 5 Gbps | $1,055.99 / mo | [Get SG CN2 GIA 1280G](https://bwh81.net/aff.php?aff=77528&pid=178) |

Hong Kong and Tokyo share identical pricing and specs (HK at 1 Gbps, Tokyo at 1.2 Gbps). Osaka sits one tier cheaper at entry — $49.99/month vs $89.99 — with a 1.5 Gbps link. Singapore mirrors Osaka's pricing. The HK 40G plan can also be migrated to Tokyo, Osaka, or Singapore, so you are not locked to one location.

### Limited edition CN2 GIA plans — the actual "cheap" options

These are the boxes that come up when you search "cheap cn2 gia vps." They are periodically restocked in small batches and sell out within hours. Stock status below reflects the current stock page; by the time you read this, any of them may be back or gone again.

| Plan | CPU | RAM | Storage | Transfer | Link | Datacenters | Price (annual) | Status | Buy |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| CN2 GIA-E 10G LE | 1 core | 512 MB | 10 GB SSD | 500 GB | 1 Gbps | DC6/DC9/SJ/NY/Vancouver + Softbank + NL Unicom + others (15 DCs) | $49.99 / yr | Out of stock | [Get CN2 GIA-E 10G LE](https://bwh81.net/aff.php?aff=77528&pid=94) |
| CN2 GIA-E 20G LE | 1 core | 1 GB | 20 GB SSD | 500 GB | 1 Gbps | Same 15-DC pool | $89.99 / yr | Out of stock | [Get CN2 GIA-E 20G LE](https://bwh81.net/aff.php?aff=77528&pid=105) |
| CN2 GIA-E 40G LE | 2 cores | 2 GB | 40 GB SSD | 1 TB | 2.5 Gbps | Same 15-DC pool | $89.99 / yr | Out of stock | [Get CN2 GIA-E 40G LE](https://bwh81.net/aff.php?aff=77528&pid=132) |
| THE DC6 PLAN LE | 1 core | 1 GB | 20 GB SSD | 1 TB | 2.5 Gbps | DC6 CN2 GIA-E | $53 / yr | Out of stock | [Get THE DC6 PLAN](https://bwh81.net/aff.php?aff=77528&pid=149) |
| THE PLAN LE | 2 cores | 2 GB | 40 GB SSD | 1 TB | 2.5 Gbps | HK85, Softbank, DC6 GIA-E, DC9 GIA + 19 DCs | $99 / yr | Out of stock | [Get THE PLAN](https://bwh81.net/aff.php?aff=77528&pid=147) |
| THE PLAN v2 LE | 2 cores | 2 GB | 40 GB SSD | 2 TB | 2.5 Gbps | Same 19-DC pool | $119 / yr | Out of stock | [Get THE PLAN v2](https://bwh81.net/aff.php?aff=77528&pid=131) |
| DC9 CN2 GIA LE (V1) | 1 core | 768 MB | 15 GB SSD | 750 GB | 1.5 Gbps | DC9 CN2 GIA | $38 / yr | Out of stock | [Get DC9 CN2 GIA V1](https://bwh81.net/aff.php?aff=77528&pid=145) |
| DC9 CN2 GIA LE (V2) | 1 core | 1 GB | 20 GB SSD | 500 GB | 1 Gbps | DC9 GIA + DC3 CN2 + DC8 ZNET + 10 DCs | $79.99 / yr | Out of stock | [Get DC9 CN2 GIA V2](https://bwh81.net/aff.php?aff=77528&pid=112) |
| DC9 CN2 GIA LE (V3) | 1 core | 1 GB | 20 GB SSD | 1 TB | 1 Gbps | Same 10-DC pool | $79.99 / yr | Out of stock | [Get DC9 CN2 GIA V3](https://bwh81.net/aff.php?aff=77528&pid=143) |
| BiggerBox Pro LE | 1 core | 1 GB | 20 GB SSD | 1 TB | 2.5 Gbps | LA DC1 (CN2 GIA + CMIN2 + CUP) | $39 / yr | Out of stock | [Get BiggerBox Pro](https://bwh81.net/aff.php?aff=77528&pid=156) |
| MegaBox Pro LE | 2 cores | 2 GB | 40 GB SSD | 2 TB | 2.5 Gbps | LA DC1 (CN2 GIA + CMIN2 + CUP) | $49 / yr | Out of stock | [Get MegaBox Pro](https://bwh81.net/aff.php?aff=77528&pid=157) |
| HK85 LE | 1 core | 1 GB | 20 GB SSD | 500 GB | 1 Gbps | Hong Kong HK85 (CMI) | $79.99 / yr | Out of stock | [Get HK85 LE](https://bwh81.net/aff.php?aff=77528&pid=121) |

A few things to note if you are chasing these:

- The **CN2 GIA-E 10G limited edition at $49.99/year** is the cheapest true CN2 GIA-E box BandwagonHost has ever sold. It is a 1-core / 512 MB / 10 GB SSD / 500 GB traffic box — fine for a personal proxy, SSH jump host, or low-traffic site, not for anything heavy.
- The **BiggerBox Pro ($39/yr) and MegaBox Pro ($49/yr)** are the current price-floor champions when in stock. They live in LA DC1 with a three-network premium return path (CN2 GIA + CMIN2 + CUP). The MegaBox Pro gives you double the RAM, storage, and traffic of the BiggerBox Pro for $10/year more — that is the better buy if both are available.
- The **THE PLAN** limited editions are the most flexible: 19 swappable datacenters including Hong Kong HK85 and Japan Softbank, which are normally locked behind the $89.99/month Ultra plans.
- All limited editions bill annually only; no monthly option. Renewal is at the same price you paid initially — BandwagonHost does not do teaser-rate hikes on these.

BandwagonHost publishes a live stock monitor. If you want any of the out-of-stock plans, watching that page or the official restock notification channel is the only realistic way to catch them.

## How the cheap options actually compare to the premium ones

The price gap between a $49.99/year limited edition and the $89.99/month Hong Kong Ultra plan is roughly 21x on a monthly basis. What you are paying for at the top end:

- **Latency.** Hong Kong and Tokyo CN2 GIA sit around 20–40ms to major Chinese cities; Los Angeles DC6/DC9 is typically 140–180ms. For proxy or web browsing use, LA is fine. For competitive gaming or real-time voice, HK/Tokyo is the only sensible choice.
- **Link speed.** Limited editions are capped at 1 Gbps; the E-Commerce series goes up to 10 Gbps at the top; Hong Kong is fixed at 1 Gbps but with much lower latency.
- **Stability under load.** CN2 GIA capacity is finite. The same pipe serves everyone, so during Chinese peak hours (roughly 20:00–23:00 Beijing time), a 512 MB / 500 GB limited edition will feel the squeeze sooner than a higher-tier E-Commerce box.
- **Support and SLA.** Standard E-Commerce plans are self-managed with 99.9% uptime. The separate SLA series (DC5, 99.99% uptime, free IP swap every two weeks) is aimed at e-commerce and foreign-trade sites that need guarantees.

If your use case is "personal proxy, light browsing, SSH access, occasional download from China-facing services," a $49.99/year CN2 GIA-E limited edition — when available — is genuinely enough. If you are running a production site serving Chinese users, doing live video or voice, or hosting a game server, the E-Commerce 80G tier ($56.99/month) is the realistic floor, and Hong Kong is the better pick if latency matters and budget allows.

## Picking a plan by use case

**Cheapest possible CN2 GIA-E:** The CN2 GIA-E 10G limited edition (pid 94) at $49.99/year, when in stock. Otherwise, the MegaBox Pro (pid 157) at $49/year on DC1's three-network premium path. Both sell out fast.

**Best value for general use:** The CN2 GIA-E 20G E-Commerce plan (pid 87) at $49.99/quarter. You get 2 cores, 1 GB RAM, 1 TB transfer, 2.5 Gbps port, and migration across 15 datacenters. This is the plan BandwagonHost's own community recommends as the default if you can't decide.

**Light production site / small business:** CN2 GIA-E 80G (pid 89) at $56.99/month — 4 cores, 4 GB RAM, 3 TB transfer. Enough headroom for a real website with Chinese traffic.

**E-commerce / foreign-trade site needing uptime guarantees:** The SLA series on DC5 (pid 164 upward), with 99.99% SLA and free IP swaps. Entry is $65.89/quarter for 2 dedicated cores / 1 GB / 20 GB / 1 TB.

**Lowest latency to mainland China:** Hong Kong CN2 GIA 40G (pid 95) at $89.99/month. If you can tolerate a touch more latency for a lower price, Osaka CN2 GIA 40G (pid 134) at $49.99/month is the best deal in the Ultra family.

**Maximum flexibility across premium locations:** THE PLAN v2 limited edition (pid 131) at $119/year, when in stock — gives you 19 swappable datacenters including HK85 and Softbank for less than two months of the regular Hong Kong plan.

## What you get regardless of tier

Every BandwagonHost VPS, cheap or premium, includes the same baseline:

- **KVM virtualization** with full root access and tun/tap support (PPP and VPN work out of the box).
- **KiwiVM panel** — in-house control panel for start/stop, OS reload, emergency console, rDNS/PTR management, free datacenter migration, snapshots, usage stats, and an API.
- **20+ OS templates**: AlmaLinux, RockyLinux, CentOS, Debian, Ubuntu, CentOS Stream, Fedora, plus custom ISO on request.
- **Enterprise-grade hardware** (BandwagonHost owns its equipment and IP space, no third-party leasing).
- **24/7 monitoring** with per-minute node checks.
- **30-day refund policy** and 99.9% uptime guarantee on standard plans (99.99% on SLA plans).

The cheap limited editions are not a cut-down product — they are the same infrastructure, just smaller allocations on the same CN2 GIA pipe.

## Coupon codes and pricing reality

As of the latest community tracking (the bandwagonhost.net coupon page updated in August 2026), **there are currently no active public coupon codes.** BandwagonHost cancelled their常规 recurring discount codes during the 2025 Double-11 promotion. A short-lived code `NODESEEK2026` appeared briefly in February 2026 and expired within roughly two days.

Historical codes like `BWHCGLUKKB` (around 6.77% recurring) and `BWHNCXNVXV` (around 7% recurring) are referenced around the web, but the official coupon page currently lists nothing as active. Do not rely on third-party coupon sites claiming large discounts — most either point to expired codes or affiliate redirects. The price you see on the order page is the price you pay, and renewal is at the same rate.

If a new coupon drops, it typically appears on the official site banner or via the restock notification channels first.

## Buying flow, briefly

1. Pick a plan from the table above and click the corresponding 👉 link — each one goes to that specific product's order page with the affiliate cookie set.
2. Choose billing cycle (quarterly / semi-annual / annual where available; monthly on higher tiers).
3. Create an account or log in. BandwagonHost accepts Alipay, PayPal, credit card, and a few regional methods.
4. After payment, the VPS is provisioned within minutes. You get a KiwiVM login, the IP, and root credentials.
5. Select your OS in KiwiVM, then either use the box in its default datacenter or migrate it to another CN2 GIA node for free.

No setup fee, no long-term contract — the plan is month-to-month (or quarter/year depending on the billing cycle you chose) and cancellable anytime.

## The honest summary

"Cheap CN2 GIA VPS" is a real category, but it is a small one. BandwagonHost is one of the few providers that actually sells CN2 GIA bandwidth at sub-$100/year price points, and they do it through limited-edition restocks rather than a permanent cheap tier — because the underlying transit is genuinely expensive and capacity-constrained. The realistic options:

- **Sub-$100/year:** Limited editions only (CN2 GIA-E 10G, BiggerBox Pro, MegaBox Pro, THE PLAN series). Catch them when restocked.
- **~$170–300/year:** The CN2 GIA-E E-Commerce 20G/40G plans. Always in stock, migratable, the dependable middle.
- **$50–90/month and up:** Osaka / Singapore entry Ultra plans, then Hong Kong / Tokyo for lowest latency.

If you just want a working CN2 GIA box today without hunting restocks, the CN2 GIA-E 20G E-Commerce plan (pid 87) at $49.99/quarter is the default answer. Everything cheaper is a waiting game; everything more expensive is a latency or SLA decision. 👉 [Start with the CN2 GIA-E 20G plan](https://bwh81.net/aff.php?aff=77528&pid=87) if you want the no-thinking option, or watch the stock page for the limited editions if you are chasing the lowest possible annual price.
