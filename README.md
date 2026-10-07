# Martha: marketing specialist for team-up

Martha writes and reviews launch copy for your project (README heroes, landing
pages, launch posts, emails) as a read-only
[team-up](https://github.com/Bumblebiber/team-up) specialist you call from
Claude Code. Every claim comes with a source or a `[NEEDS PROOF]` marker,
every draft gets a Germany/EU compliance check, and every review ends in a
SHIP / FIX / BLOCK verdict. She never posts, sends or invents testimonials.

English and German.

One repository, one specialist: a manifest, instructions, seven skills and an
eval suite — no code, no model names, no install hooks.

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

## What you get back

A real, trimmed excerpt: Martha reviewing an earlier version of this README
(run of 2026-10-07, unedited apart from cuts).

> ## Gate: **FIX**
>
> The README is honest and free of hype […]. As marketing it undersells. It
> describes what the repo *contains* […] instead of what a developer *gets*,
> it shows no example output, and it never mentions Claude Code, the
> environment the reader works in. **Biggest problem: no proof of output.**
>
> | # | Angle | Copy | Rationale |
> |---|---|---|---|
> | A | Outcome | **Martha writes and reviews your launch copy, and won't invent proof.** | Names the job and the main differentiator in one line |
>
> | Claim | Proof | Status |
> |---|---|---|
> | "seven skills" | 7 files in `skills/`, 7 listed in `specialist.json` | ok |
> | "Every claim she writes traces to a proof point or is marked `[NEEDS PROOF]`" | `instructions.md` shared rules | ok as a stated behaviour; show an example |
>
> | Item | Rule | Status | Fix |
> |---|---|---|---|
> | Legal-substantiation claims ("UWG/FTC", "DSGVO") | UWG §5 | flag | Correct the email-consent attribution to UWG §7 |
> | AI-assisted README text | AI Act Art. 50 | ok, ordinary product copy, not a public-interest topic | — |

The hero above is her variant A; the other fixes are applied.

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
# team-up specialist approve marketing.martha@0.2.2 --global
```

## Run

```bash
team-up specialist run --id marketing.martha --call-type consult \
  --objective "Position this project and draft the README hero" \
  --project /abs/path/to/project
```
