# Positioning and research

Positioning decides who the product is for and why it wins for them. Research
supplies the evidence for it. Do both before any copy: copy written without
positioning is decoration.

## 1. Collect evidence

- **The product**: README, docs, site, changelog, issues. What it actually
  does, not what it says about itself.
- **Voice of customer**: issues, forums, Reddit/HN threads, reviews, support
  threads, app-store reviews. Quote people's exact words with links — these
  become headlines.
- **Competitors and alternatives**: teardown table below.
- **How search and AI answer engines frame the category**: search the
  category questions yourself ("best tool for X", "X alternative", "how to do
  X") and record which products and domains come up. You cannot query
  ChatGPT, Claude or Perplexity directly; hand the human a probe protocol
  instead (below).

### Competitor teardown

One row per competitor, plus "do nothing / build it yourself / spreadsheet":

| Dimension | Where to look |
|---|---|
| One-liner and category claimed | Homepage hero, meta description, GitHub description |
| ICP targeted | Case studies, testimonials, pricing tiers, job ads |
| Pricing and packaging | Pricing page: free tier, limits, the tier they push |
| Key claims and proof | Homepage, comparison pages, docs |
| Channels | Blog, social, communities, ads, which queries they rank for |
| Traction signals | Stars, downloads, release cadence, public user counts — with source |
| What users complain about | Issues, Reddit, HN, G2/Capterra, app stores |

Traction signals lie: npm/PyPI downloads include CI and mirror traffic, stars
can be bought, "10,000 users" is usually unaudited. Report them as signals
with that caveat, never as facts about adoption.

The complaints column is usually where the positioning comes from.

### AI answer-engine probe (handed to the human)

Five to ten category questions, the exact prompts, run in ChatGPT, Perplexity,
Claude and Google (AI Overview/AI Mode). For each: date, engine, which products
are named, how the category is framed, which domains are cited. Answers vary
run to run, so the result is a dated snapshot, and the value is in repeating
it monthly with the same prompts. Give the human the prompts and an empty
log table.

## 2. Position

1. **Competitive alternatives** — what the customer does today without the
   product. Usually not a competitor.
2. **Unique attributes** — what the product has that they lack. Verifiable only.
3. **Value** — "so what?" for each attribute until you reach an outcome the
   customer cares about: time, money, risk, status, peace of mind.
4. **Best-fit customer (ICP)** — role or situation, trigger event, what they
   tried already. "Developers" or "small businesses" is not an ICP.
5. **Jobs to be done** — "When <situation>, I want to <motivation>, so I can
   <outcome>", with the functional, emotional and social job.
6. **Market category** — the frame that makes the value obvious. Existing
   category if the product wins there; a new one only if nothing fits.
7. **Objections** — switching cost, trust, price, "I can build this myself".
8. **Language** — write the positioning once; localise the messaging for
   German and English, do not translate it word for word. Decide du/Sie.

For developer tools and agent tooling, the reader is often also the
developer's agent: a README and docs that state plainly what the tool does,
with copy-paste install lines, are read by people and models alike.
(Hypothesis — no measurement shows agents recommend such tools more.)

## 3. Output: the messaging house

- **Positioning statement** (internal): For <ICP> who <need>, <product> is a
  <category> that <key value>. Unlike <main alternative>, it <decisive difference>.
- **One-liner** — under 12 words, what it is and for whom.
- **Value proposition** — headline plus one supporting sentence.
- **Three pillars** — each a benefit with its proof points underneath. A pillar
  without proof is marked `[NEEDS PROOF]`.
- **Objection handling** — objection, answer, proof.
- **Words to use / to avoid** — from customer language where you have it.

Plus, when research was part of the task: the teardown table, the
voice-of-customer quotes, gaps and opportunities, and a sources list including
dead ends.

## Quality bar

- Could a competitor paste the one-liner onto their site unchanged? Rewrite.
- Every external claim has a URL and retrieval date; pricing older than 30
  days is re-checked.
- Specific beats clever. Numbers beat adjectives. Customer words beat yours.
- Thin evidence: give two or three candidate positionings and the test that
  decides between them (interviews, a landing-page split, ad copy test).

## Interviews and surveys (when asked to design them)

Ask about past behaviour, never hypothetical intent ("When did you last hit
this? What did you do?", not "Would you use…?"). Five to eight interviews per
segment usually show the pattern. Surveys: one idea per question, no leading
wording, include "other" and "none".
