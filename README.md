# cheap singapore vps: what S$4.75 to S$9 a month really buys, and the fine print most lists skip

The cheapest Singapore VPS tracked in late September 2026 is UpCloud's Starter plan at **S$4.75 a month**. Vultr's entry Cloud Compute instance sits just above it at S$6.96 with two and a half times the storage, and OVHcloud will hand you 4 GB of RAM for about US$4.54 — with a traffic catch buried in a footnote. Those three numbers tell you most of what you need to know about this market: at the bottom of the price range, the sticker price is the least interesting figure on the page.

This guide compares the entry plans from the providers with Singapore datacenters, walks through Vultr's full 1 GB lineup (usually the first thing people shortlist from a name they recognize), and covers the details that decide your real bill — Singapore's 9% GST, traffic caps, and "first 24 months" intro pricing.

## Quick picks

> - **Best-known brand at the entry price:** Vultr Cloud Compute, 1 vCPU / 1 GB RAM, 25 GB storage, 1 TB transfer — S$6.96/month incl. GST. 👉 [Check Vultr's current Singapore plan pricing](https://www.vultr.com/pricing/?ref=7268283)
> - **Absolute cheapest:** UpCloud Starter, 1 GB RAM, 10 GB storage, unmetered transfer — S$4.75/month
> - **Most RAM per dollar:** OVHcloud VPS-1, 2 vCores / 4 GB / 40 GB NVMe — from US$4.54 ex. GST, but traffic is capped at 500 GB/month before throttling kicks in
> - **Most raw compute:** Contabo Cloud VPS 4, 4 vCores / 8 GB / 100 GB SSD — €4.40/month for the first 24 months

If you just want a Singapore box from a provider you've heard of, with hourly billing and a clean upgrade path, the Vultr 1 GB plan is the boring-but-sensible default. The rest of this article explains when the other options beat it.

## What the cheapest Singapore VPS plans actually cost

A September 2026 price tracker currently lists 467 plans from 13 providers with a Singapore location. Here are the entry plans worth knowing about, put side by side. SGD prices include Singapore's 9% GST; the last two rows are quoted in the provider's own currency.

| Provider and plan | vCPU / RAM | Storage | Monthly transfer | Price |
| --- | --- | --- | --- | --- |
| UpCloud — Starter | 1 / 1 GB | 10 GB | Unmetered | S$4.75 |
| HostHatch — NVMe | 1 / 2 GB | 10 GB | 500 GB | S$5.57 |
| Kamatera — Basic | 1 / 1 GB | 20 GB | 1 TB | S$5.57 |
| DigitalOcean — Basic | 1 / 0.5 GB | 10 GB | 0.5 TB | S$5.57 |
| Vultr — Cloud Compute | 1 / 1 GB | 25 GB | 1 TB | S$6.96 |
| AWS Lightsail — General Purpose | 2 / 0.5 GB | 20 GB | 1 TB | S$6.96 |
| Linode (Akamai) — Nanode | 1 / 1 GB | 25 GB | 1 TB | S$6.96 |
| Kuroit — SG AVA 1 | 1 / 1 GB | 15 GB | 1 TB | £3.00 |
| OVHcloud — VPS-1 | 2 / 4 GB | 40 GB | 500 GB, then throttled | US$4.54 ex. GST |
| Contabo — Cloud VPS 4 | 4 / 8 GB | 100 GB | Unlimited, fair use | €4.40, first 24 months |

A few observations you won't get from a bare price ranking. The S$5.57 tier is all over the place: HostHatch gives you 2 GB of RAM at that price, DigitalOcean gives you 0.5 GB. Three providers charge the same S$6.96 and deliver anywhere from 512 MB to 1 GB. And the two cheapest-looking rows at the bottom — OVHcloud and Contabo — both have terms attached that matter more than the price, which is where the next sections go.

## Vultr's Singapore plans: the full entry lineup

Vultr currently sells four 1 GB configurations in Singapore across three product lines, priced from S$6.96 to S$8.36 a month including GST. Everything is monthly with no contract, and all four deploy from the same Singapore datacenter.

| Plan | vCPU / RAM | Storage | Transfer | Price/mo (incl. 9% GST) | Deploy |
| --- | --- | --- | --- | --- | --- |
| Cloud Compute — Regular | 1 / 1 GB | 25 GB | 1 TB | S$6.96 | [Get the 1 GB plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| Cloud Compute — High Frequency | 1 / 1 GB | 32 GB | 1 TB | S$8.36 | [See High Frequency pricing](https://www.vultr.com/pricing/?ref=7268283) |
| Cloud Compute — High Performance (AMD) | 1 / 1 GB | 25 GB | 2 TB | S$8.36 | [Check High Performance pricing](https://www.vultr.com/pricing/?ref=7268283) |
| Cloud Compute — High Performance (Intel) | 1 / 1 GB | 25 GB | 2 TB | S$8.36 | [Check High Performance pricing](https://www.vultr.com/pricing/?ref=7268283) |

The S$1.40 jump from Regular to either upgrade line buys different things:

- **High Frequency** gets you 32 GB of storage instead of 25 GB, with the same 1 TB transfer. Pick it if your bottleneck is disk — a growing media library, a chatty database.
- **High Performance** keeps the 25 GB disk but doubles transfer to 2 TB and runs on newer AMD or Intel hardware. Pick it if your bottleneck is traffic. The AMD and Intel variants are priced identically with matching specs; if you have no preference, flip a coin.

### Where the ladder goes next

The Regular Performance line scales in fixed steps, so it's worth knowing the exit route before you commit. List prices are in USD; Singapore accounts pay 9% GST on top.

| USD/month | vCPU | RAM | Storage | Transfer |
| --- | --- | --- | --- | --- |
| $5 | 1 | 1 GB | 25 GB | 1 TB |
| $10 | 1 | 2 GB | 55 GB | 2 TB |
| $20 | 2 | 4 GB | 80 GB | 3 TB |
| $40 | 4 | 8 GB | 160 GB | 4 TB |
| $80 | 8 | 16 GB | 320 GB | 6 TB |

One practical advantage at this end of the market: Vultr meters usage hourly up to the plan's monthly rate. Spin up a Singapore instance, run your load tests, destroy it, and you pay for the hours used. That makes the 1 GB plan a cheap way to check actual latency from your users' locations before committing to anything longer-term. 👉 [Create a Vultr account and deploy a Singapore instance](https://bit.ly/VulTR)

## The fine print that decides your real bill

Four things move the final number at this price tier: GST, the transfer policy, storage size, and intro pricing. Most comparison lists only surface the first one by accident.

### Singapore's 9% GST applies to USD prices too

Vultr, DigitalOcean, Linode and most of the others bill in USD, then add Singapore's 9% GST for Singapore-billed accounts. The SGD figures in the tables above already include it — so Vultr's plan advertised as US$5 a month lands at S$6.96 on a Singapore invoice. Watch the reverse case too: OVHcloud quotes its VPS-1 as US$4.54 *excluding* GST, which comes to roughly US$4.95 once the tax is added. When you compare prices across providers, decide once whether you're comparing GST-inclusive or GST-exclusive, and stick to it.

### Metered, throttled, or "unlimited" — they're not the same deal

This is the biggest trap in the cheap Singapore VPS market, because the word "unlimited" hides three different policies.

- **Vultr meters transfer and bills overage per GB.** The entry plans include 1 TB (2 TB on High Performance). Your base bill is predictable, but a traffic spike costs extra.
- **OVHcloud's APAC plans look unmetered, with a quota.** The VPS-1 in Singapore includes 500 GB per month; after that, bandwidth is capped at 10 Mbps. For a website serving pages that's survivable. For anything moving files, backups or media, it's a wall.
- **Contabo and UpCloud advertise unlimited or unmetered transfer, subject to fair use.** Contabo pairs it with a 200 Mbit/s port on the entry plan, so sustained throughput has a practical ceiling regardless.

Which policy suits you depends on your traffic shape. Steady, heavy traffic favors a metered plan with a big allowance, because you know exactly what 2 TB costs. Small, spiky traffic is usually happier on an unmetered plan where a viral week doesn't produce a surprise invoice.

### "First 24 months" is not the price

Contabo's Cloud VPS 4 is listed at €4.40 a month for the first 24 months, with €5.50 as the regular rate. That's a legitimate deal for 4 vCores and 8 GB of RAM, but budget for the step-up. Some smaller providers run the opposite play and advertise that renewal never jumps — Vebloom, whose Singapore plans start at US$14.99, markets explicitly that you renew at your signup price. Vultr and DigitalOcean keep it simple: the list price is the renewal price.

### Storage is where cheap plans quietly shrink

UpCloud's S$4.75 plan allots 10 GB of disk. HostHatch gives you 2 GB of RAM at S$5.57 but also only 10 GB of disk. For a VPN endpoint or a lightweight bot that's plenty; for a WordPress install with a few years of images, 10 GB fills up faster than you'd think. The S$6.96 tier from Vultr and Linode comes with 25 GB, which is a more realistic floor for anything running a CMS.

## Which cheap Singapore VPS fits your project

Match the plan to your actual bottleneck — price, RAM, disk, or traffic — and the choice gets simple.

- **Personal VPN, proxy, or a small bot:** take the cheapest. UpCloud at S$4.75 does this fine (10 GB disk is irrelevant for a proxy), and Vultr at S$6.96 is the pick if you'd rather have hourly billing and the option to rebuild the box differently later.
- **A small business site or blog:** Vultr or Linode at S$6.96. Twenty-five gigabytes of disk and 1 TB of transfer cover a modest site with room to grow.
- **Databases, staging, or dev environments:** OVHcloud's VPS-1 is the value outlier — 4 GB of RAM for about five US dollars. Just keep monthly traffic under the 500 GB quota, or the 10 Mbps cap will make remote work painful.
- **Traffic-heavy projects:** Vultr's High Performance line at S$8.36 gives you a metered 2 TB, which is the most predictable way to buy bandwidth at this price. Contabo's 8 GB plan is cheaper per GB moved if you're comfortable with the 24-month pricing structure and fair-use port limits.
- **You need a 10Gbps port or Windows:** Kuroit's Singapore line runs a 10 Gbps network on AMD EPYC/Ryzen hardware starting at £3 a month, and supports Windows on a bring-your-own-license basis.

## FAQ

### Is a 1 GB RAM VPS enough for a website?

For static sites and lightly used CMS installs, yes — 1 GB handles a small WordPress or nginx setup comfortably, and adding swap smooths over the occasional spike. It gets tight the moment you run a database and a PHP application under real concurrent load; that's when the 4 GB tier starts earning its keep.

### Why is my Singapore bill higher than the USD list price?

Two reasons: currency conversion and Singapore's 9% GST, which providers add to invoices billed to Singapore. Vultr's US$5 entry plan becoming S$6.96 is exactly this math, with nothing hidden underneath.

### Can I stop paying when I'm not using the server?

With Vultr, yes — instances bill hourly up to the monthly rate, and destroying the instance stops billing. Contabo works differently: the minimum initial contract is one month, and post-paid accounts need four weeks' cancellation notice. If your workload is intermittent (a dev box you spin up on weekends, for example), hourly billing is worth real money over a year.

### How fast will a Singapore VPS be for Southeast Asian visitors?

Singapore is where most of the region's subsea cables land, and the latency figures providers quote reflect that: Kuala Lumpur sits a few milliseconds away, Jakarta around 15–20 ms, and Bangkok, Ho Chi Minh City, Hong Kong and Manila typically in the 30–50 ms range. From a Singapore box, one server can serve the whole region without anyone noticing a delay.

### Do the cheapest plans include backups?

It varies more than you'd expect. Kuroit bundles free automated backups into every listed plan, and OVHcloud's VPS-1 includes a daily backup of the previous 24 hours. On most other budget plans, backups are either a paid add-on or your own job via snapshots — factor that into the "cheap" price before you commit.

## Before you click buy

Two checks save the most regret. First, compare transfer policies against your actual monthly traffic — a 500 GB quota that throttles to 10 Mbps, a metered 1 TB, and a fair-use unlimited are very different products wearing similar prices. Second, on any intro-priced plan, read what the rate becomes after the promo window closes.

For most people searching for a cheap Singapore VPS, the shortlist comes down to this: UpCloud if every cent counts and 10 GB of disk is enough, OVHcloud if you need RAM and can live inside 500 GB, and Vultr at **S$6.96 a month** if you want a mainstream provider with hourly billing, 25 GB of storage, 1 TB of transfer, and a one-click upgrade path for when the project outgrows 1 GB. 👉 [Compare Vultr's Singapore plans and current prices](https://www.vultr.com/pricing/?ref=7268283)
