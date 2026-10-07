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

### Channel rule sheet — verified on 2026-10-07

P = the platform's own page, S = third-party. Re-read the source before a
launch; rules move.

| Channel | Rules and what is known | Source |
|---|---|---|
| Show HN | Must be something people can run or try, not a landing page, signup page, blog post or newsletter; easy to try, ideally without signup; never ask friends to upvote or comment. New accounts face Show HN limits since the wave of AI-generated projects (S). LLM-written comments break HN rules. | news.ycombinator.com/showhn.html (P) |
| Product Hunt | Personal accounts only, company accounts prohibited. Never ask for upvotes, ask people to visit and comment. The launch link may be shared anywhere. 12:01 AM Pacific is the suggested launch time. Lower priority for developer tools (hypothesis). | producthunt.com/launch (P) |
| Reddit | Each subreddit has its own rules; read them and the sidebar first. The "9:1" contribution ratio is a third-party paraphrase, not a schedule. Accounts that only promote get removed. Could not be verified — Reddit's pages were unreachable during research; the human checks reddit.com/wiki/selfpromotion before posting. | S only |
| dev.to | AI-assisted articles allowed if in good faith, disclosed and fact-checked; they should not mainly promote a business. AI-written comments are prohibited. Terms: content "not designed primarily for the purposes of promotion or creating backlinks". | dev.to/guidelines-for-ai-assisted-articles-on-dev, dev.to/terms (P) |
| Hashnode | AI content permitted if you review it and take responsibility. Prohibited: bulk or automated posting, engagement farming, SEO abuse, using the platform mainly for self-promotion. | hashnode.com/code-of-conduct (P) |
| X | Ranking code is published: engagement, clicks and dwell time count; out-of-network posts discounted; new authors boosted. No official link penalty is documented. Automated accounts must disclose that they are automated. | github.com/xai-org/x-algorithm (P); automation page unreadable (S) |
| LinkedIn | Feed ranks on dwell time and the viewer's interaction history (LinkedIn engineering, 2026-03). No official link penalty; studies of external links disagree (−19% to −50% reach, company pages behave differently). No AI-disclosure duty; C2PA credentials are shown when present. | LinkedIn engineering blog, help a6282984 (P); link studies (S) |
| Bluesky | No single algorithm — users pick feeds. Guidelines ban spam and disruptive repetitive posting; alternative identities must be labelled. No AI-content rule. | bsky.social community guidelines (P) |
| Mastodon / Threads | Mastodon: each server sets its own bot and automation rules; read the server's. Threads: ranking is undocumented beyond Meta's own statements. | S |
| YouTube incl. Shorts | Disclose realistic altered or synthetic content (real people saying things they did not, altered real events, realistic scenes that did not happen) in Studio. AI help with scripts, titles and thumbnails needs no disclosure. YouTube says disclosure does not limit reach. Mass-produced, repetitive content (e.g. AI voice over slideshows) risks demonetisation (S). | support.google.com/youtube/answer/14328491 (P) |
| Newsletters | Substack and beehiiv have recommendation networks that drive a large share of new subscribers (the platforms' own claims); beehiiv also has paid recommendations. Buttondown has none. | Platform posts (P, snippet-level) |
| Podcasts | No measured evidence for developer tools. Treat a guest appearance as a hypothesis to test, not a default channel. | — |

Default where links may lose reach (X, LinkedIn): put the link in the first
reply or comment. It costs nothing; whether it helps is unproven.

### Developer tools and open source

- **The README is the landing page.** One-line value proposition, who it is
  for (and who it is not for), install in under a minute with copy-paste
  commands, a GIF or short demo, a working first example, badges that say
  something (version, CI, license).
- **Registries and directories**: npm/PyPI metadata (description, keywords,
  homepage), GitHub topics, awesome-lists, and for MCP servers the official
  MCP Registry (modelcontextprotocol.io/registry, still in preview as of
  2026-10-07: a `server.json` pointing at the npm/PyPI/Docker package or a
  remote URL, reverse-DNS namespace verified via GitHub, DNS or HTTP). Most
  people find servers through the aggregators and marketplaces that read
  the registry, so check those listings after publishing.
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
- Verified 2026-10-07: Gmail requires, for senders of 5,000+ mails a day,
  SPF and DKIM, DMARC aligned on From (policy `none` is enough), RFC 8058
  one-click unsubscribe for marketing mail, unsubscribes honoured within 48
  hours, TLS, and a spam rate below 0.1% (0.3% is the hard limit);
  enforcement with rejections has ramped up since November 2025, and bulk
  status never expires (support.google.com/a/answer/14229414, P). Microsoft
  requires SPF, DKIM and DMARC for 5,000+ a day to Outlook.com since
  2025-05-05, junk first, rejection (550 5.7.515) later (S). Smaller senders
  should meet the same bar — inbox placement depends on it.

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
