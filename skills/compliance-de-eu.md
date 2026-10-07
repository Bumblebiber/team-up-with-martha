# Compliance check for marketing in Germany and the EU

A pre-publication checklist. You flag; you do not give legal advice. Where the
law is unsettled or the stakes are high, the output says "check with a
lawyer". Every rule below carries the date it was last verified — if a rule
decides the outcome and is older than three months, re-check its source.

## How to run it

1. List every claim, tracking element, data collection point, label and
   AI-generated asset in the material.
2. Check each against the rules below.
3. Output a table: item | rule | status (ok / flag / block) | fix | source.
   `block` means it must not ship as is.

## Rules — verified on TODO(round2)

TODO(round2): each rule gets its statute or authority source, URL and verify
date. Round-1 drafts below; S-sourced items stay flagged until confirmed.

1. **Misleading and comparative claims (UWG §§5, 5a, 6)** — superlatives,
   "#1", "fastest", "better than X" need provable facts at the time of
   publication. Comparisons must be objective, verifiable and fair. Cite proof
   or remove.
2. **Email advertising (UWG §7)** — prior express consent (§7 Abs. 2);
   double opt-in is how consent gets proven. Existing-customer exception
   (§7 Abs. 3) only when all its conditions hold: address obtained in a
   sale, advertising own similar products, no objection, and a clear opt-out
   notice both at collection and in every mail. Keep proof of consent.
3. **Tracking (§25 TDDDG)** — consent for anything that is not strictly
   necessary; reject as easy as accept; no pre-ticked boxes or nudging
   designs. TODO(round2): position on cookieless analytics.
4. **Impressum (§5 DDG, formerly TMG)** — on every business site and
   business social profile, reachable easily; a link from the profile is
   acceptable.
5. **Ad and sponsorship labels (UWG §5a Abs. 4, §6 DDG)** — paid, affiliate
   or gifted content labelled "Werbung" or "Anzeige", up front and visible,
   in the language of the audience.
6. **Environmental claims (EmpCo, implemented in UWG)** — TODO(round2):
   confirm date in force and transition rules. Generic claims
   ("klimafreundlich", "nachhaltig", "grün", "umweltfreundlich") need
   recognised excellent environmental performance; "climate neutral" based on
   offsetting is prohibited; self-made sustainability labels are prohibited;
   future claims ("net zero by 2030") need a verifiable plan. For software:
   flag "green hosting" and "carbon-neutral AI" claims.
7. **AI-generated content (AI Act Art. 50)** — TODO(round2): confirm dates
   and the effect of any EU Digital Omnibus deferral. Deepfakes (realistic
   synthetic images, audio, video of people, places or events) must be
   disclosed. AI-generated text published to inform the public on matters
   of public interest must be disclosed unless a human reviewed it and an
   editor or the company takes responsibility. Chatbots must say they are AI.
   Marketers using AI tools are deployers; machine-readable marking is the
   tool provider's duty. Platform rules (YouTube, Meta, TikTok, LinkedIn) may
   require labels beyond the law — check them for the channel.
8. **Data protection (DSGVO)** — privacy notice for every form, list and
   tracker; a data-processing agreement with every email, analytics and CRM
   provider; data minimisation in forms.
9. **Dark patterns** — no fake countdowns, fake scarcity ("only 2 left" when
   untrue), confirmshaming, hidden costs or pre-ticked add-ons. Also
   prohibited for online platforms under the EU Digital Services Act.
10. **Prices (PAngV)** — consumer prices shown as final prices including VAT;
    strike-through prices only against the lowest price of the last 30 days.

## Outside Germany

For US audiences: FTC rules on endorsements (disclose material connections)
and substantiation of claims, CAN-SPAM for email. Flag rather than assess
other jurisdictions.
