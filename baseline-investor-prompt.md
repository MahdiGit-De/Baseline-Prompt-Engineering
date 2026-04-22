Prompt(Final)Role:
Act as a rigorous research analyst specializing in deep-tech infrastructure startups, telecom partnerships, edge computing, and B2B infrastructure markets.

Objective:
Build a structured evidence base for evaluating Mutable as of April 9, 2026.

Rules:
- Use only publicly available information available on or before April 9, 2026.
- Do NOT draw conclusions, recommendations, scores, or investment judgments.
- Do NOT perform business evaluation or strategic analysis.
- Do NOT infer traction, adoption, customer success, revenue quality, or commercial scale unless directly evidenced.
- If critical commercial information is not explicitly evidenced, it MUST be listed under Unknowns.
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
- past signals such as funding, pilots, accelerators, recognitions
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

Prompt 2 (Judgment Layer) — CLEAN VERSION:

Role:
Act as a senior Business Developer and Business Analyst specializing in deep-tech infrastructure startups, telecom partnerships, edge computing, and B2B go-to-market strategy.

Audience:
Investor-style decision maker evaluating startup opportunities.

Task / Objective:
Evaluate Mutable’s commercial credibility strictly based on the provided evidence base.

Input:
You are given an evidence base structured as:
A. Current facts
B. Historical facts
C. Inferences
D. Assumptions
E. Unknowns
F. Conflicts / inconsistencies
G. Source quality notes


Critical rules:
- Use ONLY the provided evidence.
- Do NOT introduce new facts or external knowledge.
- Do NOT upgrade assumptions or inferences into facts.
- If something is unknown ? treat it as a risk.
- Unknowns must explicitly influence:
  - risk analysis
  - scoring (lower confidence)
  - final recommendation
- Base all conclusions primarily on current facts, not historical signals.
- If evidence is weak or incomplete, reflect this in lower confidence and more conservative scoring.
- Do NOT repeat the same point across sections.

Tone:
- Write in a direct, analytical, investor-style tone.
- Avoid storytelling or narrative fluff.

Evaluation dimensions:
- problem-solution fit
- market attractiveness
- differentiation
- go-to-market feasibility
- scalability
- defensibility

Scoring:
Rate each from 1–5:
1 = weak / unsupported  
3 = plausible but not de-risked  
5 = strong with clear supporting evidence  

- Scores must be justified using evidence.
- If evidence is missing ? default to lower scores.

Output format:
A. Investment summary (4–6 sentences)
- core thesis
- why it matters
- main concern
- recommendation

B. Business development analysis
- target customers
- economic buyers
- entry motion
- partnership pathways
- expansion logic

C. Business analysis
- problem-solution fit
- market timing
- business model logic
- competitive dynamics
- scalability
- execution risk

D. Scorecard (1–5 with justification)

E. Counterargument
- strongest possible bull case

F. Top 5 risks
- based on evidence gaps and assumptions

G. Top 5 diligence questions
- what would most change the decision

H. Final recommendation:
- attractive / watchlist / too early / weak opportunity

I. Confidence level:
- low / medium / high
- explain briefly based on evidence quality and completeness

Success criteria:
- Each claim must link to evidence from the input.
- Scores must reflect evidence strength (missing data ? lower score).
- Unknowns must appear explicitly in risks and final recommendation.
- No section may exceed 5–6 bullet points or short paragraphs.

Prompt 2 — (FULL VERSION WITH DATASET)
Role:
Act as a senior Business Developer and Business Analyst specializing in deep-tech infrastructure startups, telecom partnerships, edge computing, and B2B go-to-market strategy.

Audience:
Investor-style decision maker evaluating startup opportunities.

Task / Objective:
Evaluate Mutable’s commercial credibility strictly based on the provided evidence base.

Input:

A. Current facts:
- Mutable’s live public website describes the company as “The Public Edge Cloud.” (mutable.cloud)
- Mutable’s website states it upgrades underutilized operator-owned servers into monetizable edge compute capacity. (mutable.cloud)
- Mutable’s website lists product components including Mutable OS, Mutable Kubernetes Platform, Mutable Node, Mutable Mesh, and a Marketplace. (mutable.cloud)
- Mutable’s website lists application areas including AR/VR, IoT, robotics, autonomous vehicles, and cloud gaming. (mutable.cloud)
- A public GitHub organization named Mutable exists and describes itself as “Airbnb for servers, the public edge cloud.” (github.com/mutable)
- A current Momenta portfolio page lists Mutable as a portfolio company. (momenta.vc)

B. Historical facts:
- Momenta announced an investment in Mutable on March 31, 2020. (momenta.vc)
- Mutable raised a .5M seed round in 2020. (public reporting)
- Mutable participated in the 5G Open Innovation Lab inaugural cohort in 2020. (ongoalliance.org)
- Mutable was listed as a finalist in Light Reading’s Leading Lights 2020. (lightreading.com)

C. Inferences:
- Mutable appears to combine infrastructure software, operator enablement, and a marketplace model rather than a single product offering.
- The business appears dependent on both supply-side infrastructure aggregation and demand-side workload adoption, implying two-sided execution risk.
- Public evidence supports positioning and historical visibility more strongly than current commercial traction.

D. Key assumptions:
- Operators have sufficient underutilized infrastructure to monetize.
- There is sufficient demand for low-latency workloads to utilize distributed edge supply.
- Fragmented infrastructure can be standardized into a reliable platform.
- Operators are willing to share infrastructure capacity in a marketplace model.
- Marketplace liquidity can be achieved across supply and demand.

E. Unknowns:
- No verified public evidence identified for named customers as of April 9, 2026.
- No verified public evidence identified for recurring revenue as of April 9, 2026.
- No verified public evidence identified for production deployments at scale as of April 9, 2026.
- No verified public evidence identified for signed operator partnerships as of April 9, 2026.
- No verified public evidence identified for pricing, retention, unit economics, workload utilization, developer adoption, or marketplace liquidity as of April 9, 2026.

F. Conflicts / inconsistencies:
- Current portfolio listing exists, but recent operational proof points are limited compared to historical signals.
- Public claims of partnerships are not clearly supported by verifiable current contracts.

G. Source quality notes:
- Website supports positioning but not traction.
- Investor and accelerator sources are historical signals.
- Secondary media supports visibility, not current adoption.

Critical rules:
- Use ONLY the provided evidence.
- Do NOT introduce new facts or external knowledge.
- Do NOT upgrade assumptions or inferences into facts.
- If something is unknown ? treat it as a risk.
- Unknowns must explicitly influence:
  - risk analysis
  - scoring (lower confidence)
  - final recommendation
- Base all conclusions primarily on current facts, not historical signals.
- If evidence is weak or incomplete, reflect this in lower confidence and more conservative scoring.
- Do NOT repeat the same point across sections.

Tone:
- Write in a direct, analytical, investor-style tone.
- Prioritize clarity, precision, and commercial relevance.
- Avoid storytelling, narrative framing, or generic statements.

Evaluation dimensions:
- problem-solution fit
- market attractiveness
- differentiation
- go-to-market feasibility
- scalability
- defensibility

Scoring:
Rate each from 1–5:
1 = weak / unsupported  
3 = plausible but not de-risked  
5 = strong with clear supporting evidence  

- Scores must be justified using evidence.
- If evidence is missing ? default to lower scores.

Output format:

A. Investment summary (4–6 sentences)
B. Business development analysis
C. Business analysis
D. Scorecard (1–5 with justification)
E. Counterargument
F. Top 5 risks
G. Top 5 diligence questions
H. Final recommendation
I. Confidence level

Success criteria:
- Each claim must link to evidence from the input.
- Scores must reflect evidence strength (missing data ? lower score).
- Unknowns must appear explicitly in risks and final recommendation.
- No section may exceed 5–6 bullet points or short paragraphs.

Example (follow this style exactly for the Investment summary section):

"The company presents a plausible approach to monetizing underutilized edge infrastructure by enabling operators to convert idle capacity into distributed compute resources. However, there is no verified evidence of current customer adoption, production deployments, or repeatable go-to-market execution. The primary commercial concern is whether fragmented supply can be aggregated into a reliable platform with sufficient demand-side pull. As a result, while the strategic direction is aligned with broader edge computing trends, the business remains insufficiently de-risked from a commercial perspective."

---

Now perform the full evaluation using the provided evidence base.
