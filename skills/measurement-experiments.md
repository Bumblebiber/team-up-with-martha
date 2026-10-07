# Measurement and experiments

Decide what to measure, read what the numbers say, and design experiments
that can answer a question at the traffic the product actually has.

## 1. Funnel and metrics

Map the funnel before choosing metrics. AARRR as the default frame:

| Stage | Question | Example metric |
|---|---|---|
| Acquisition | Do the right people arrive? | Visitors to the landing page or README, by source |
| Activation | Do they reach first value? | % of signups/installs completing the first successful use |
| Retention | Do they come back? | Week-4 active / week-0 cohort |
| Referral | Do they bring others? | Share of new users from word of mouth |
| Revenue | Do they pay? | Free-to-paid conversion, ARPU |

Define each metric: numerator, denominator, window, data source.
"Engagement" is not a metric. One North Star that tracks delivered value, plus
the inputs that drive it. Fix the leakiest stage closest to value first —
usually activation.

## 2. Unit economics

- CAC = acquisition spend including people time / new customers, per channel.
- LTV ≈ ARPU × gross margin / churn rate. Show the assumptions.
- LTV:CAC around 3:1 and payback under about 12 months are rules of thumb,
  not laws.

## 3. Experiments — small traffic first

Compute what the traffic can detect **before** proposing an A/B test.

- Sample size per variant for conversion rates (α = 0.05, 80% power):
  n ≈ 16 · p(1−p) / δ², with p the baseline rate and δ the absolute lift.
  Baseline 5%, detect +1 point: 16 · 0.0475 / 0.0001 ≈ 7,600 per variant.
- If the product cannot reach that in a few weeks, an A/B test cannot answer
  the question. Use instead:
  - a bigger change (a larger δ needs far fewer users — n falls with δ²);
  - before/after comparison with the caveat stated (seasonality, launches);
  - five to eight moderated user sessions or interviews;
  - pooling similar pages into one test;
  - sequential or Bayesian designs where the tool supports them.

Write each experiment down first: hypothesis ("changing X for Y moves Z by ≥ N
because <evidence>"), primary metric, guardrail metrics, sample size and
duration in whole weeks, decision rule. Fixed-horizon tests: no stopping at
the first significant peek. Prioritise the backlog with ICE (impact,
confidence, ease, 1–10) and show the scores.

## 4. Attribution

- Small products: UTM parameters on every link you control, a "How did you
  hear about us?" field (self-reported attribution catches word of mouth,
  podcasts and AI answers that no tracker sees), and AI referrers.
- Marketing-mix modelling and lift tests are for large ad budgets; mention
  them only when spend justifies it.
- Developer tools: package downloads, GitHub traffic and stars, docs visits.
  CLI telemetry only opt-in, documented, minimal.

## 5. Tracking and consent — verified on 2026-10-07

- **§25 TDDDG** (the TTDSG until 2024): storing or reading anything on the
  user's device needs consent unless it is strictly necessary for the
  service the user asked for. "Strictly necessary" is technical, not
  economic. (gesetze-im-internet.de, P)
- **Analytics without consent**: the German data-protection authorities
  (DSK, OH Digitale Dienste v1.2, Rn. 87–92) refuse a blanket exemption for
  reach measurement. Even simple visitor counting is not automatically part
  of the service; the answer depends on the exact configuration and purpose.
  A setup that stores and reads nothing on the device (server logs, a
  cookieless tool configured that way) arguably falls outside §25 — but the
  DSGVO still applies, and no authority or court has blessed a named tool.
  Say "likely consent-free if configured without device access; confirm
  with a lawyer", never "consent-free". (DSK, P; the inference is a
  hypothesis)
- **Google Analytics** needs consent in Germany. Consent Mode v2 signals:
  `ad_storage`, `analytics_storage`, `ad_user_data`, `ad_personalization`.
  Since 2026-06-15 Consent Mode is the single control for advertising data
  to linked Google Ads accounts; the Google-signals switch no longer
  protects you, so `ad_storage` must be denied correctly. Basic mode blocks
  tags until consent; advanced mode sends cookieless pings when denied.
  (support.google.com/analytics answers 17016975 and 9976101, P)
- **GA4 retention**: event-level data 2 or 14 months on standard properties.
  (support.google.com/analytics/answer/7667196, P)
- **Server-side tracking** does not escape the consent rule if it still
  reads from the device; the EDPB reads the ePrivacy rule as covering
  tracking techniques beyond cookies. (EDPB Guidelines 2/2023, S)
- Recommend the least tracking that answers the questions. For a small
  product a cookieless tool plus UTMs and self-reported attribution is
  usually enough.

## 6. Reading data

Segment before concluding (source, cohort, device, new vs. returning). Watch
for Simpson's paradox, survivorship bias, seasonality, bots, and tracking gaps
— ad blockers hide a large share of technical audiences. A dashboard
correlation is a hypothesis for an experiment, not a finding. Report what the
data shows, how confident you are, and what to do next.
