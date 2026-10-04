# Oxylabs review: what you get from $30 to $2,500 a month, who it fits, and a pay-per-IP alternative for smaller budgets

Oxylabs has been around since 2015, runs out of Vilnius in Lithuania, and sells residential, datacenter, ISP and mobile proxies plus a set of scraping APIs. That combination is why it shows up at the top of nearly every "best proxy" list — and also why a lot of people who search for an Oxylabs review end up confused. The company is built for teams pulling hundreds of gigabytes or hundreds of IPs a month. Buy one gigabyte of residential traffic to test it and you'll find yourself dealing with KYC questions, a three-day refund window and pricing tiers that assume you're spending real money.

So here's what the money actually buys, where the friction sits, and what to do if your scrape is smaller than Oxylabs' target customer.

## What Oxylabs actually sells

Four proxy types and a separate API line:

- **Residential proxies** — 175M+ IPs across 195 locations according to the product page (the homepage has said 188+ countries, so the marketing numbers don't match each other). Targeting goes down to country, state, city, ZIP, coordinates and ASN, with no advertised cap on concurrent sessions.
- **Datacenter proxies** — 2M+ IPs, split into shared and dedicated, billed either per IP or per GB.
- **ISP proxies** — no published pool size, available across 25 countries.
- **Mobile proxies** — 20M+ IPs from real devices.
- **Scraping APIs** — Web Scraper API from $49/month (from $0.25 per 1,000 results), Web Unblocker at $5/GB currently discounted 40% to $3/GB, a Headless Browser at $4.70/GB, and a newer Fast Search API aimed at AI workflows.

Every self-service residential plan includes unlimited concurrent sessions, three proxy users, ten whitelisted IPs, sticky sessions that can hold the same IP for up to 24 hours, and HTTP(S), HTTP3 and SOCKS5 support. Two features are locked behind the top tier: IPv4/IPv6 selection and OS filters only switch on for plans that come with a dedicated account manager, which in practice means Corporate and above.

The datacenter and ISP side runs under a fair-use policy instead of "unlimited": you get 100 sessions per IP up to 50GB of traffic in a billing cycle, then it drops to 10.

## Oxylabs pricing: four residential tiers, and a lot of fine print

Residential is the product most people are here for, and it's sold as monthly commitment tiers rather than a flexible balance:

| Plan | Traffic | Monthly price | Effective rate |
| --- | --- | --- | --- |
| Starter | 5GB | $30 | $6/GB |
| Basic | 20GB | $100 | $5/GB |
| Advanced | 125GB | $500 | $4/GB |
| Corporate | 1TB | $2,500 | $2.50/GB |

Pay-as-you-go residential sits around $8/GB as the standard rate, with a capped promotional rate near $4/GB that some buyers have picked up with a coupon — PCMag's reviewer paid $8 for a gigabyte of traffic and $4 after a discount code. The awkward part: pay-as-you-go is **non-refundable**, and on other plans you have to ask within three calendar days of your first payment while having used under 20% of your traffic (10% on enterprise plans). Refunds take up to 15 business days to land. Dedicated datacenter bought through enterprise is non-refundable unless you report a billing error within 30 days.

Two more things you only notice after you commit:

1. **Tax comes on top.** Published prices exclude VAT or sales tax, which Oxylabs adds where required. In a high-VAT jurisdiction that's roughly a fifth added to every number above.
2. **The pages contradict each other.** The residential FAQ has quoted a $99/11GB entry while the plan cards start at $30/5GB; the navigation menu advertises residential "from $2.50/GB" while the pricing page says "from $6/GB". Treat the four plan cards as the real checkout grid and everything else as copy that wasn't updated when the tiers changed.

Other product lines, for context: shared datacenter runs from $0.44/GB pay-as-you-go, dedicated datacenter from $2.25 per IP on a three-IP minimum ($6.75/month), shared datacenter per IP from $1.20 per IP on ten IPs, and the Web Scraper API entry point is $49/month.

## What Oxylabs genuinely does well

Performance is the strongest argument. CNET's proxy testing gave Oxylabs the second-highest performance score in the field, with success rates and response times that sit at the top of the table. Oxylabs' own cards quote an average 0.6-second response time and 99.95% success.

The developer surface is broad, too. If you need a managed unblocker for Cloudflare, PerimeterX or DataDome-protected targets, or parsed JSON out of a search results page without writing the parser, those products already exist and are documented. Its compliance paperwork is unusually complete for this market — ISO/IEC 27001:2022, SOC 2, and per third-party directories, ISO 27701 for privacy management — which is exactly what procurement teams in regulated industries ask for.

On sourcing, Oxylabs publishes a tier framework for how residential IPs are acquired, states all residential traffic qualifies for tiers that include the device owner's consent, and names Honeygain as a long-term bandwidth partner. Some providers won't answer that question at all, so a public answer counts for something.

## Where the experience gets rough

The complaints that come up repeatedly are about fit rather than quality.

**KYC is mandatory.** There's no anonymous self-serve signup at any price. Directory reviewers report a 24–48 hour clearance window for clean business accounts, and in some cases a short interview covering your company, target domains and expected volume. If you need proxies working this afternoon, this is the wrong vendor. The free trial is also request-only — one time, through a contact form or sales email, not a button in the dashboard.

**Target restrictions apply at any price level.** Oxylabs publishes a list of restricted targets for its residential network: Apple domains including the App Store and iTunes, banking and financial institutions, some Google properties, government sites, plus streaming, ticketing and mailing services. The list isn't exhaustive. If your target is on it, the per-gigabyte rate is irrelevant. The sensible pre-purchase move is to name your exact targets to support over live chat and get the answer in writing before you commit a month.

**There's a hole in the middle of the ladder.** Between 20GB and 125GB there's no tier. Needing 60GB a month means buying Advanced at $500 or topping up Basic repeatedly at the same per-GB rate.

**Small buyers get a worse deal than enterprise ones.** Review-aggregator sentiment on Oxylabs splits the same way the plan structure does: teams with account managers are happy, self-service buyers who hit the refund window or the onboarding queue are not. If you're a solo operator or a small affiliate scraper running a few gigabytes a month, you're paying for compliance overhead that doesn't do anything for you. If you want Oxylabs-adjacent infrastructure at consumer prices, the brand usually recommended instead is Decodo, the rebranded Smartproxy product.

## So who should actually buy Oxylabs

Buy it if three or more of these are true:

- You're moving 100GB+ of residential traffic a month and the per-GB rate at that volume ($4 or below) beats everything else you've priced.
- Procurement needs ISO 27001 or SOC 2 documentation before a signature.
- Cloudflare/DataDome-protected targets are the whole point, and you'd rather pay for a managed unblocker than maintain your own.
- You want parsed output, not raw HTML, and the Web Scraper API's $0.25 per 1,000 results fits your budget model.
- Your team size needs sub-users, whitelisted IPs and a dashboard that isn't a fight.

Skip it — or at least don't make it your first purchase — if your monthly data bill is under roughly $50, if you need same-day access, if you can't wait through KYC, or if the whole workload is small-volume scraping where paying per IP with unlimited bandwidth is cheaper than paying per gigabyte.

## The pay-per-IP alternative worth pricing first

That last case is where 9Proxy enters the picture, and the pricing model is the reason. Instead of a minimum monthly commitment, 9Proxy sells balance-based packages in two currencies: **IPs** and **gigabytes**. An IP-based package gives you a fixed number of residential IPs with unlimited bandwidth, and unused IPs never expire. A GB-based package gives you unlimited proxy endpoints and charges against your traffic balance, with 180-day validity (it becomes unlimited on Enterprise).

There are practical differences you should know before buying either:

- **IP-based plans need the desktop app.** Authentication runs through local port forwarding, optionally with proxy authentication on top. IPs stay live for a few hours up to about 24 hours, and rotation happens through the auto-rotation proxy on selected ports.
- **GB-based plans run entirely in the dashboard.** Username/password or IP whitelisting, sticky or rotating sessions you configure yourself, and targeting by country, state, city, ZIP or ISP in the proxy generator.

The network is advertised as 20M+ residential IPs across 90+ locations with 99.95% uptime and HTTP(S)/SOCKS5 support. Payment options are wider than you'd expect for a smaller provider: credit cards, bank cards, crypto (USDT, BTC, ETH, LTC, DOGE and others), Alipay, Apple Pay and Google Pay.

Pricing changed once since launch. IP-based packages and bundles went up on **June 1, 2026**; GB-based packages were left alone. You'll still see "from $0.015/IP" quoted around the web — that's the old list. The deepest published tier now works out to roughly $0.018 per IP.

### 9Proxy packages and current prices

| Model | Package | Effective rate | Price | Purchase |
| --- | --- | --- | --- | --- |
| IP-based | 100 IPs | $0.24/IP | $24 | [Get the 100 IP package](https://bit.ly/9-Proxy) |
| IP-based | 500 IPs | $0.144/IP | $72 | [Get the 500 IP package](https://bit.ly/9-Proxy) |
| IP-based | 1,000 IPs + 500 bonus IPs | $0.084/IP | $126 | [Get the 1,500 IP package](https://bit.ly/9-Proxy) |
| IP-based | 2,500 IPs | $0.084/IP | $210 | [Get the 2,500 IP package](https://bit.ly/9-Proxy) |
| IP-based | 5,000 IPs | $0.072/IP | $360 | [Get the 5,000 IP package](https://bit.ly/9-Proxy) |
| IP-based | 15,000 IPs | $0.048/IP | $720 | [Get the 15,000 IP package](https://bit.ly/9-Proxy) |
| IP-based | 25,000 IPs | $0.035/IP | $863 | [Get the 25,000 IP package](https://bit.ly/9-Proxy) |
| IP-based | 50,000 IPs | $0.029/IP | $1,438 | [Get the 50,000 IP package](https://bit.ly/9-Proxy) |
| Business IP | 100,000 IPs | $0.023/IP | $2,300 | [Get the 100,000 IP package](https://bit.ly/9-Proxy) |
| Business IP | 200,000 IPs | $0.021/IP | $4,140 | [Get the 200,000 IP package](https://bit.ly/9-Proxy) |
| Business IP | 500,000 IPs | $0.018/IP | $8,625 | [Get the 500,000 IP package](https://bit.ly/9-Proxy) |
| GB-based | 5GB | $3.00/GB | $15 | [Get the 5GB package](https://bit.ly/9-Proxy) |
| GB-based | 50GB + 5GB bonus | $2.10/GB | $105 | [Get the 55GB package](https://bit.ly/9-Proxy) |
| GB-based | 100GB | $1.50/GB | $150 | [Get the 100GB package](https://bit.ly/9-Proxy) |
| GB-based | 200GB | $1.00/GB | $200 | [Get the 200GB package](https://bit.ly/9-Proxy) |
| GB-based | 1,000GB | $0.80/GB | $800 | [Get the 1,000GB package](https://bit.ly/9-Proxy) |
| GB-based | 2,000GB | $0.75/GB | $1,500 | [Get the 2,000GB package](https://bit.ly/9-Proxy) |
| Bundle | Starter — 100 IPs + 5GB | — | $30 | [Get the Starter bundle](https://bit.ly/9-Proxy) |
| Bundle | Popular — 1,500 IPs + 50GB | — | $180 | [Get the Popular bundle](https://bit.ly/9-Proxy) |
| Bundle | Pro — 5,000 IPs + 500GB | — | $720 | [Get the Pro bundle](https://bit.ly/9-Proxy) |

GB packages carry 180-day validity; Enterprise upgrades remove the expiry and add team mode with one owner plus up to five members, per-member traffic controls and activity logs. New-user trials exist but are limited and allocated by availability — you request one from support and specify whether you want IP-based or GB-based access.

For anyone comparing against the Oxylabs ladder, the interesting number is the 1,000 + 500 IP package: $126 for 1,500 residential IPs with unlimited bandwidth, versus $500 for 125GB on Oxylabs' Advanced tier. Different products, different guarantees, wildly different entry points.

## Oxylabs vs 9Proxy at a glance

|  | Oxylabs | 9Proxy |
| --- | --- | --- |
| Pool | 175M+ residential IPs, 195 locations | 20M+ residential IPs, 90+ locations |
| Billing model | Monthly commitment tiers + pay-per-GB | Balance-based: per IP or per GB |
| Residential entry | $30 for 5GB | $15 for 5GB, or $24 for 100 IPs |
| Minimum spend | Monthly plan required on everything but shared datacenter PAYG | No subscription; buy a package when you need one |
| Expiry | Unused traffic expires with the cycle | IPs don't expire; GB balance valid 180 days |
| Refunds | 3-day window, under 20% usage, self-service only | Not published in the same detail — confirm with support before buying |
| Onboarding | Mandatory KYC, reported 24–48h plus possible interview | Self-serve signup, dashboard or app access |
| Extra products | Datacenter, ISP, mobile, unblocker, scraper APIs | Residential only (datacenter listed as coming) |
| Best for | High-volume enterprise scraping with compliance requirements | Smaller budgets, session-based tasks, teams that want to buy IPs once |

## How to pick between them in a few minutes

Ask yourself three questions and the decision usually makes itself.

**How much traffic will you actually move each month?** Under ~50GB, per-GB pricing at Oxylabs' rates gets expensive fast and the package model wins on cost. At 500GB+, Oxylabs' $2.50/GB (the Corporate rate) plus its certifications and managed unblocking is a defensible spend.

**Do your targets tolerate residential endpoints at all?** Run them past support. Apple properties, banks, several Google domains and ticketing sites are blocked on Oxylabs' residential network, and that list is published. If you're on it, no plan fixes it.

**Can you wait two days for access and do you need invoices with compliance attachments?** If yes, Oxylabs. If you want to buy 100 IPs, keep them for months without expiry and start scraping tonight, 9Proxy's model fits better — and if that's where you land, 👉 [grab a package and check the current rates here](https://bit.ly/9-Proxy).

## FAQ

**Does Oxylabs have a free trial?** Yes, but it's request-only — one time per customer, arranged through the sales contact form or the support email, not a self-serve checkout. Oxylabs also hands out five free datacenter IPs on signup, which is a low-cost way to test basic connectivity.

**Is Oxylabs worth it for a small business?** Only if your volume is already in the tens of gigabytes a month or you need the compliance documentation. Below that, you're paying for KYC overhead and enterprise support you won't use.

**Can I use Oxylabs with Scrapy, Puppeteer or Playwright?** Yes — the endpoint follows the standard `pr.oxylabs.io` format with unlimited concurrent sessions on residential, and the documentation covers the common integrations.

**What's the cheapest way to get residential proxies?** Depends on the shape of your workload. If each request uses little data but needs frequent IP changes, per-GB pricing wins. If you need the same IP to hold across a long session with heavy transfer, per-IP with unlimited bandwidth is usually cheaper — which is the whole reason 9Proxy's IP-based packages exist. 👉 [See the per-IP rates and current packages](https://bit.ly/9-Proxy)

## The short version

Oxylabs is a serious provider with real performance numbers, a deep product line and the compliance paperwork that enterprise procurement wants. It's also built around monthly commitments, mandatory verification, a narrow refund window and a target blocklist that overrides everything else. Nothing here is hidden — it's just not the part that shows up in rate comparison tables.

If you're scraping 100GB+ a month, price the Advanced and Corporate tiers properly, ask support about your specific targets in writing, and skip anything based on the "$2.50/GB" figure that turns out to be the $2,500 tier. If your workload is smaller, budget-driven, or session-based, the per-IP model is the cheaper structure — and that's where a 9Proxy package starts at $15. 👉 [Check the current 9Proxy packages and start with a small one](https://bit.ly/9-Proxy) before committing anywhere near $500 a month.
