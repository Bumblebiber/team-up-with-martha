# Growth and analytics

Decide what to measure, read what the numbers say, and design experiments that
can actually answer a question.

## Funnel

Map the product's funnel before choosing metrics. AARRR as a default frame:

| Stage | Question | Example metric (dev tool) |
|---|---|---|
| Acquisition | Do the right people arrive? | Unique visitors to README/landing by source |
| Activation | Do they reach first value? | % of installs that complete the first successful run |
| Retention | Do they come back? | Week-4 active users / week-0 cohort |
| Referral | Do they bring others? | Share of new users from referral/word of mouth |
| Revenue | Do they pay? | Free → paid conversion, ARPU |

Define each metric precisely: numerator, denominator, time window, data source.
"Engagement" is not a metric. Pick one North Star that tracks delivered value,
plus the inputs that drive it.

Fix the leakiest stage closest to value first — usually activation. More
traffic into a broken activation step is wasted.

## Unit economics

- CAC = acquisition spend (including people time) / new customers, per channel.
- LTV ≈ ARPU × gross margin / churn rate. Show the assumptions.
- LTV:CAC around 3:1 and CAC payback under ~12 months are common health
  heuristics. They are rules of thumb, not laws; say so.

## Experiments

Write each one down before running it:

- **Hypothesis**: "Changing X for audience Y will move metric Z by ≥ N,
  because <evidence>."
- **Primary metric** and guardrail metrics (what must not get worse).
- **Sample size**: for conversion rates, n per variant ≈ 16 · p(1−p) / δ²
  (α = 0.05, 80% power), where p is the baseline rate and δ the absolute lift
  to detect. Example: baseline 5%, detect +1 point → 16 · 0.0475 / 0.0001 ≈
  7,600 per variant. If traffic cannot reach that in a reasonable time, say
  the test is underpowered and propose a bigger change or a qualitative method
  instead.
- **Duration**: whole weeks, decided up front. No peeking and stopping at the
  first significant result.
- **Decision rule**: what result leads to what action.

Prioritise the backlog with ICE (Impact, Confidence, Ease, 1–10 each) and show
the scores.

## Reading data

- Segment before concluding: source, cohort, platform, new vs. returning.
- Watch for Simpson's paradox, survivorship bias, seasonality, bot traffic and
  tracking gaps (ad blockers hide a large share of developer traffic).
- Correlation in dashboards is a hypothesis for an experiment, not a finding.
- Report: what the data shows, how confident, what you would do next.

## Tracking and privacy

Recommend the minimum tracking that answers the questions. In the EU,
non-essential cookies and analytics need consent (DSGVO/TTDSG); prefer
privacy-friendly, cookieless analytics where it suffices, and UTM parameters
for campaign attribution.
