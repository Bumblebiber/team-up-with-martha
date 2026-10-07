# team-up-with-martha

Martha, the marketing specialist for
[team-up](https://github.com/Bumblebiber/team-up): a read-only marketing
worker your Claude Code session can hand positioning, copy, launch plans and
reviews to.

One repository, one specialist. This one holds a manifest, instructions, seven
skills and an eval suite — no code, no model names, no install hooks.

## What Martha does

Positioning and messaging, marketing copy (landing pages, READMEs, launch
posts, emails, ads), market and competitor research with sources, go-to-market
and launch plans, content strategy and SEO, funnel metrics and experiment
design, and reviews of existing marketing material.

Every claim she writes traces to a proof point or is marked `[NEEDS PROOF]`.
Copy goes through a claims and compliance check (substantiation under UWG/FTC,
email consent under UWG §7, ad labelling, green claims, AI Act labelling,
no dark patterns). Every review ends in a SHIP / FIX / BLOCK / UNDECIDED gate.

She does not publish, post, send or schedule anything, does not spend ad
budget, and never invents statistics, testimonials or social proof. She runs
read-only with network access and delivers through the mailbox.

## Skills

Skill files are read by Martha at the start of a task; `instructions.md` maps
tasks to files.

| Skill | Covers |
|---|---|
| `positioning-research` | Alternatives, ICP, JTBD, messaging house; competitor teardown, voice of customer, AI answer-engine probe |
| `copywriting` | Frameworks by situation, variants, anti-slop pass, quotable claims |
| `gtm-launch` | Motion, channel rules, developer-tool and OSS distribution, launch email setup, launch plan |
| `search-visibility` | Intent, content plan, crawl checklist incl. AI crawlers, spam guard, measuring beyond clicks |
| `measurement-experiments` | Funnel metrics, unit economics, small-traffic experiments, attribution, consent |
| `compliance-de-eu` | UWG, email consent, TDDDG, Impressum, ad labels, green claims, AI Act Art. 50, DSGVO, prices |
| `marketing-review` | Prioritised review with a SHIP / FIX / BLOCK / UNDECIDED gate |

Dated rules carry a "verified on" date and get re-checked before they decide
an outcome. Details the underlying research did not cover are tagged
`[unverified]`.

## Install

```bash
git clone https://github.com/Bumblebiber/team-up-with-martha
team-up specialist inspect ./team-up-with-martha     # read-only, always first
team-up specialist install ./team-up-with-martha
# install also grants Martha every project; older team-up needs:
# team-up specialist approve marketing.martha@0.2.1 --global
```

## Run

```bash
team-up specialist run --id marketing.martha --call-type consult \
  --objective "Position this project and draft the README hero" \
  --project /abs/path/to/project
```
