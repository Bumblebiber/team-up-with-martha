# Go-to-market, launch and distribution

Plan how the product reaches its ICP: which motion, which channels in what
order, with what offer, and what counts as success. You plan and draft; a
human ships.

## 1. Choose the motion

| Motion | Fits when |
|---|---|
| Product-led (free tier, self-serve, open source) | Low price, fast time to value, users can try it alone |
| Community-led | The audience gathers somewhere and the product gets better when shared |
| Content/search-led | People actively search for the problem; slow, compounding |
| Partner/marketplace-led | A platform's directory or marketplace is where buyers look (app stores, MCP registry, Shopify, plugin directories) |
| Sales-led | High price, several stakeholders, procurement |

Say which motion and why. A small team does one primary channel well, not
seven thinly. Default for a solo founder with no budget: no paid ads until a
channel converts organically and the unit economics are known.

## 2. Pick channels

List candidates, score each on reach to the ICP, cost in money and hours, time
to first signal, and fit with the motion. One primary, one or two secondary.

Before recommending any community, read its current rules and cite them — the
rule sheet below is a starting point, not the rules.

### Channel rule sheet — verified on TODO(round2)

TODO(round2): fill from Reanna round 2 with primary sources and dates —
Show HN, Reddit, Product Hunt, dev.to/Hashnode, X, LinkedIn, Bluesky,
Mastodon/Threads, YouTube/Shorts, newsletters, podcasts.

### Developer tools and open source

- **The README is the landing page.** One-line value proposition, who it is
  for (and who it is not for), install in under a minute with copy-paste
  commands, a GIF or short demo, a working first example, badges that say
  something (version, CI, license).
- **Registries and directories**: npm/PyPI metadata (description, keywords,
  homepage), GitHub topics, awesome-lists, and for MCP servers the official
  MCP Registry. TODO(round2): MCP Registry status and `server.json`
  requirements, verified.
- **Docs as marketing**: the getting-started page converts more than the
  homepage for technical buyers. Tutorials with runnable code, honest
  comparison pages, a public changelog.
- **Launch posts** for technical communities: what it is, why you built it,
  what is different, what is rough. No hype, no marketing voice, and the
  maker answers comments personally.

### B2B and consumer products

- B2B: the buyer and the user differ; give each their own proof (ROI and
  risk for the buyer, workflow for the user). Founder-led outreach and
  content before any paid channel. Industry associations, trade fairs,
  partner resellers and Google Business Profile matter for local and
  German Mittelstand audiences.
- Consumer: one platform where the audience already spends time, short video
  if the product is visual, app-store page optimisation for apps.

## 3. Pricing and packaging (input, not decision)

- Anchor on value delivered and the alternatives' prices, not on cost.
- Value metric: what the customer pays per (seat, project, usage). It should
  grow with the value received.
- Good-better-best tiers; the middle one is the one you want chosen.
- Open source: say plainly what is free forever and what is paid (hosted,
  team, support). Ambiguity reads as bait-and-switch.
- German B2B: show net prices plus VAT; consumers: gross prices.

## 4. Email list for a launch

Mail only to people who opted in and can prove it; `compliance-de-eu.md` has
the consent rules. Technical setup the human must check before the first send:

- SPF, DKIM and DMARC set up for the sending domain, aligned with the From
  address.
- One-click unsubscribe headers plus a visible unsubscribe link; unsubscribes
  honoured promptly.
- Keep the spam-complaint rate low; send from a domain warmed up gradually.
- TODO(round2): exact Gmail/Yahoo/Microsoft thresholds and dates, verified.

## 5. Launch plan

1. **Readiness** — positioning and one-liner final; landing page or README,
   demo, install or signup path tested from zero on a clean machine, docs for
   the first use case, a feedback channel, analytics on the conversion events.
2. **Pre-launch** — warm the channels honestly: early users, a beta list,
   people who will genuinely try it on day one. Never vote rings or "please
   upvote" asks — they break platform rules and get posts removed.
3. **Launch day** — per channel: the exact asset (title, post, first comment),
   posting time in the channel's timezone, who answers comments for the first
   four hours.
4. **Post-launch** — follow-up content, changelog posts, collecting the
   testimonials you were not allowed to invent, second-wave channels.

## Output

A launch brief: motion, ICP, one-liner, primary and secondary channels with
rationale and each channel's rules cited, the asset list per channel (drafts
where asked), timeline, success metrics with targets, risks. Every step a
human must perform is marked as such.
