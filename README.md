# team-up-with-martha

Martha, the marketing specialist for
[team-up](https://github.com/Bumblebiber/team-up).

One repository, one specialist. This one holds a manifest, instructions, seven
skills and an eval suite — no code, no model names, no install hooks.

## What Martha does

Positioning and messaging, marketing copy (landing pages, READMEs, launch
posts, emails, ads), market and competitor research with sources, go-to-market
and launch plans, content strategy and SEO, funnel metrics and experiment
design, and reviews of existing marketing material.

Every claim she writes traces to a proof point or is marked `[NEEDS PROOF]`.
Copy goes through a claims and compliance check (substantiation under UWG/FTC,
consent for email under DSGVO, ad labelling, no dark patterns).

She does not publish, post, send or schedule anything, does not spend ad
budget, and never invents statistics, testimonials or social proof. She runs
read-only with network access and delivers through the mailbox.

## Skills

| Skill | Covers |
|---|---|
| `positioning-messaging` | Alternatives, ICP, JTBD, category, messaging house |
| `copywriting` | Frameworks by situation, variants, claims and compliance check |
| `market-research` | Competitor teardowns, voice of customer, sourced findings |
| `gtm-launch` | Motion, channel selection, pricing input, launch plan |
| `content-seo` | Search intent, topic clusters, on-page checklist, distribution |
| `growth-analytics` | Funnel metrics, unit economics, experiment design with sample size |
| `marketing-review` | Prioritised review of existing material |

## Install

```bash
git clone https://github.com/Bumblebiber/team-up-with-martha
team-up specialist inspect ./team-up-with-martha     # read-only, always first
team-up specialist install ./team-up-with-martha
team-up specialist approve marketing.martha@0.1.0 --project /abs/path/to/project
```

## Run

```bash
team-up specialist run --id marketing.martha --call-type consult \
  --objective "Position this project and draft the README hero" \
  --project /abs/path/to/project
```
