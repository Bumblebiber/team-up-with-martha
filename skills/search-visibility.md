# Search visibility: SEO, content and AI answer engines

Get the product found where the ICP looks — classic search results, AI
Overviews and AI Mode, ChatGPT/Claude/Perplexity answers, docs search — and
earn that with content that is worth citing.

## What holds and what does not — verified on TODO(round2)

TODO(round2): confirm from primary sources and date each line.
- Google: no special requirements for AI Overviews/AI Mode beyond normal SEO
  (indexable, snippet-eligible); AI-feature traffic is inside Search
  Console's normal Web report. [round 1: P]
- Zero-click searches are the majority in the US; clicks drop where an AI
  Overview shows. [round 1: S]
- GEO/AEO: no technique has shown a stable, causal, cross-engine effect on
  being discovered. [round 1: P, preprint]
- llms.txt: no AI system is known to use it; harmless, cheap, not a tactic.
  [round 1: S]
- FAQ/HowTo rich-result status. [round 1: unverified]

Say these limits plainly when someone asks for "GEO hacks".

## 1. Search intent first

| Intent | Query looks like | Content that wins |
|---|---|---|
| Informational | "how to X", "what is X" | Guide, tutorial, explainer |
| Commercial investigation | "best X", "X vs Y", "X alternative" | Honest comparison, alternatives page |
| Transactional | "X pricing", "download X", "X kaufen" | Product, pricing, install page |
| Navigational | brand name | Homepage, docs |

Search the query and look at what ranks; the format that ranks is the intent
the engine has decided on. Record what you saw and when.

## 2. Topic research without paid tools

Autocomplete, "People also ask", related searches; the words customers use in
issues and forums; competitors' strongest pages and what they miss. Prefer
specific long-tail queries with clear intent. Volume estimates without a
keyword tool are guesses — say so.

## 3. Content plan

Topic clusters: one pillar page per core problem, supporting pieces linking to
it. Per piece: target query, intent, angle (why it beats what ranks now:
original data, working code, first-hand experience), format, CTA,
distribution.

What gets cited, by people and by AI engines alike: original numbers with
their method, clear self-contained definitions, step-by-step instructions that
work, honest comparisons that admit where the product loses, named authors
with real experience.

German and English: separate pages per language with hreflang, not
machine-translated duplicates. Localise examples, prices and legal bits.

## 4. Technical and crawl checklist

- Indexable, in the sitemap, canonical set, no duplicate pages competing,
  fast, mobile-friendly.
- One H1; H2/H3 mirror the reader's questions; the answer comes early.
- Title and meta description written as an ad for the click; keep them short
  enough not to truncate (truncation is pixel-based, so treat character
  counts as rough).
- Text as text: code blocks, not screenshots; docs in plain HTML/Markdown.
- Structured data only where it matches visible content.
- **AI crawlers** in robots.txt: decide search/citation bots and training bots
  separately. To be cited in ChatGPT and Claude search, allow their search
  bots; whether to allow training crawlers is a separate business decision.
  TODO(round2): current bot names per vendor, verified.

## 5. Spam guard

Never recommend mass-produced or programmatic pages that add no value, whether
AI-written, scraped or auto-translated — Google's spam policies call it scaled
content abuse. Thin rewritten content is not worth producing; say so when that
is all the input allows.

## 6. Distribution

Publishing is half the job. For each piece: newsletter, platform-specific
social posts (not one post cross-posted), communities where allowed, links
from README and docs, outreach to people who linked to similar work. Being
mentioned on third-party sites (forums, reviews, video, Wikipedia where
notable) likely helps AI citation as much as classic links help ranking —
hypothesis, not measured.

## 7. Measuring

Clicks alone undercount. Track:
- Search Console impressions, clicks and queries (the human exports them).
- Branded search growth — people searching the name after seeing it
  somewhere.
- AI referrals in analytics (referrers such as chatgpt.com, perplexity.ai).
- The monthly AI answer-engine probe from `positioning-research.md`.
