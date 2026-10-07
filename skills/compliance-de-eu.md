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

## Rules — verified on 2026-10-07

P = statute, authority or the platform itself; S = law-firm or other
summary. Research behind this list: team-up runs `20261007T094516Z-kxv1` and
`20261007T095044Z-s6sq`. Items tagged `[unverified]` were not part of that
research — likely right, but re-check the source before they decide an
outcome.

1. **Misleading and comparative claims (UWG §§5, 5a, 6)** — superlatives,
   "#1", "fastest", "better than X" need provable facts at the time of
   publication. Comparisons must be objective, verifiable and about
   comparable things. Cite proof or remove. (UWG; §§5, 6 text not re-read — S)
2. **Email advertising (UWG §7)** — prior express consent (§7 Abs. 2 Nr. 2);
   double opt-in is how consent gets proven, so keep the record.
   Existing-customer exception (§7 Abs. 3) only when all four conditions
   hold: address obtained in connection with a sale; advertising own similar
   products; the customer has not objected; a clear opt-out notice both at
   collection and in every mail. (gesetze-im-internet.de/uwg_2004/__7.html, P)
   Technical sender rules are in `gtm-launch.md`.
3. **Tracking (§25 TDDDG)** — consent for storing or reading anything on the
   device unless strictly necessary for the requested service, and
   "strictly necessary" is technical, not economic. Reject must be as easy
   as accept; no pre-ticked boxes or nudging designs. No blanket exemption
   for analytics: the DSK (OH Digitale Dienste v1.2, Rn. 87–92, P) says it
   depends on the exact configuration. Details in
   `measurement-experiments.md`. Status for a consent-free analytics claim:
   `flag`, never `ok`.
4. **Impressum (§5 DDG, formerly TMG)** — on every business site and
   business social profile, easy to reach; a link from the profile to a
   complete Impressum is acceptable. (IHK, S)
5. **Ad and sponsorship labels (UWG §5a Abs. 4, §6 DDG)** — paid, affiliate
   or gifted content is labelled "Werbung" or "Anzeige", up front and
   visible, in the audience's language. An English "#ad" alone is weak for a
   German audience. No label is needed where the commercial intent is
   obvious (a company advertising itself on its own channel). (S)
6. **Environmental claims (EmpCo)** — in force since **2026-09-27** through
   the Drittes Gesetz zur Änderung des UWG, BGBl. 2026 I Nr. 43
   (recht.bund.de, P). `block` unless proven:
   - generic claims — "klimafreundlich", "nachhaltig", "grün",
     "umweltfreundlich" — without recognised excellent
     environmental performance;
   - "climate neutral" or "CO₂-compensated" based on offsetting;
   - sustainability labels that are not state-approved or independently
     monitored schemes — no home-made badges;
   - future claims ("net zero by 2030") without a defined, verifiable,
     time-bound plan.
   The transition rule §15b UWG covers only goods placed on the market
   before 2026-09-27; websites and online advertising get no grace period.
   (Law firms and IHK, S.) For software: flag "green hosting",
   "carbon-neutral AI" and similar.
7. **AI-generated content (AI Act Art. 50)** — applies since
   **2026-08-02**. The Digital Omnibus (Reg. (EU) 2026/1744) gave only tool
   providers a grace period, to 2026-12-02, for machine-readable marking of
   systems already on the market; it did not change the duties below.
   (Commission FAQ, P; Omnibus via summaries, S)
   - **Deepfakes** — realistic generated or manipulated images, audio or
     video of real people, places or events — must be disclosed clearly at
     first exposure. `block` if undisclosed.
   - **AI-generated text** published to inform the public on matters of
     public interest — politics, health, environment, consumer safety,
     economic or scientific developments of public debate — must be
     disclosed, **unless** a person with the right expertise reviewed it and
     a named person or the company holds editorial responsibility.
     (Commission FAQ, P.) The final guidelines reportedly put advertising
     and PR in scope when they inform on such matters (S). Ordinary product
     copy with a human editor is low risk; unreviewed AI text making health,
     environmental or financial claims is `flag`.
   - **Chatbots and AI agents** facing users must say they are AI.
   - Platform rules can go further: YouTube requires disclosure of realistic
     synthetic content; Meta and TikTok require labels on realistic AI
     video, images and audio; LinkedIn shows C2PA credentials but requires
     nothing; dev.to requires disclosure of AI-assisted articles.
     (Platform pages, P except Meta/TikTok, S)
   - Disclosure lowers trust in some studies and not in others (S). Where
     the law or the platform requires it, it is not optional.
8. **Data protection (DSGVO)** `[unverified]` — a privacy notice for every form, list and
   tracker; a data-processing agreement with every email, analytics and CRM
   provider; collect only the fields you need.
9. **Dark patterns** `[unverified]` — no fake countdowns, fake scarcity ("only 2 left" when
   untrue), confirmshaming, hidden costs or pre-ticked add-ons. (UWG
   blacklist; EU Digital Services Act for platforms.)
10. **Prices (PAngV)** `[unverified]` — consumer prices shown as final prices including
    VAT; a "was" price must be the lowest price of the last 30 days.

## Outside Germany

For US audiences: FTC rules on endorsements (disclose material connections)
and substantiation of claims, CAN-SPAM for email. Flag rather than assess
other jurisdictions.
