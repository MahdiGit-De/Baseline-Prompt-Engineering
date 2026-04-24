# Prompt 1 — Evidence Extraction (Final Version)
# Function: Build a structured, classified evidence base before any judgment is made.
# Use this FIRST, then feed output into Prompt 2.
# ─────────────────────────────────────────────────────────────────────────────

Role:
Act as a rigorous research analyst specializing in deep-tech infrastructure startups, telecom partnerships, edge computing, and B2B infrastructure markets.

Objective:
Build a structured evidence base for evaluating [COMPANY] as of [DATE].

Rules:
- Use only publicly available information available on or before [DATE].
- Do NOT draw conclusions, recommendations, scores, or investment judgments.
- Do NOT infer traction, adoption, customer success, revenue quality, or commercial scale unless directly evidenced.
- Classify every material claim into one of the following:
  1. Current fact = directly evidenced present-state information as of the evaluation date
  2. Historical fact = past signal, not proof of current traction
  3. Inference = logical interpretation based on evidence, but not directly proven
  4. Assumption = something that must be true for the business to work commercially
  5. Unknown = critical missing information that cannot be verified

Definition notes:
- A live company website may support current positioning, but not current traction unless traction is directly evidenced.
- Historical announcements, funding rounds, accelerator participation, pilots, awards, and media mentions do not prove current commercial adoption.
- If evidence is weak, mixed, conflicting, self-reported, or unclear, mark that explicitly.
- If critical information cannot be verified, classify it as Unknown.
- Lack of evidence is not proof of absence, but it remains a commercial uncertainty.

Source hierarchy:
Prefer sources in this order:
1. Official company website, product documentation, public filings, direct public statements
2. Primary partner or ecosystem sources
3. Reputable industry or financial media
4. Investor, accelerator, or portfolio pages
5. Platform metadata such as LinkedIn or Crunchbase only as supporting context, not proof of traction

Citation rules:
- Cite the supporting source for every current fact and historical fact.
- For inferences, cite the source(s) supporting the interpretation.
- Each inference must clearly reference supporting facts.
- If no source directly supports a claim, do not classify it as a fact.

Additional guidance:
- Prioritize commercially relevant information (customers, revenue, deployments, partnerships, pricing, GTM).
- Avoid including trivial or purely descriptive details.

Output format:

A. Current facts
- bullet points only
- verified present-state facts only
- each bullet must include a citation

B. Historical facts
- bullet points only
- past signals such as funding, pilots, accelerators, recognitions, or historical product claims
- each bullet must include a citation

C. Inferences
- bullet points only
- logical interpretations based on evidence
- each bullet must cite supporting evidence

D. Key assumptions
- bullet points only
- critical assumptions that must hold for the business to become commercially credible

E. Unknowns / missing critical data
- bullet points only
- use consistent phrasing: "No verified public evidence identified for…"
- especially include:
  - customers
  - revenue
  - production deployments
  - signed partnerships
  - pricing
  - retention
  - unit economics
  - workload utilization
  - developer adoption
  - marketplace liquidity

F. Conflicts / inconsistencies
- bullet points only
- note conflicting signals or unclear present-state status

G. Source quality notes
- brief notes on which evidence is company-claimed, secondary, platform-derived, outdated, or conflicting
