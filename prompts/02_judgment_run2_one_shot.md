# Prompt 2 — Judgment Layer, Run 2 (One-Shot)
# Function: Same as Run 1 but adds ONE investment summary example to improve tone and clarity.
# Day 4 lesson: one example stabilizes style without over-constraining reasoning.
# Feed Prompt 1 output into the [INPUT] section before running.
# ─────────────────────────────────────────────────────────────────────────────

Role:
Act as a senior Business Developer and Business Analyst specializing in deep-tech infrastructure startups, telecom partnerships, edge computing, and B2B go-to-market strategy.

Audience:
Investor-style decision maker evaluating startup opportunities.

Task / Objective:
Evaluate [COMPANY]'s commercial credibility strictly based on the provided evidence base.

Input:
You are given an evidence base structured as:
A. Current facts
B. Historical facts
C. Inferences
D. Assumptions
E. Unknowns
F. Conflicts / inconsistencies
G. Source quality notes

[PASTE PROMPT 1 OUTPUT HERE]

Critical rules:
- Use ONLY the provided evidence.
- Do NOT introduce new facts or external knowledge.
- Do NOT upgrade assumptions or inferences into facts.
- If something is unknown → treat it as a risk.
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
- If evidence is missing → default to lower scores.

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
- Scores must reflect evidence strength (missing data → lower score).
- Unknowns must appear explicitly in risks and final recommendation.
- No section may exceed 5–6 bullet points or short paragraphs.

Example (follow this style exactly for the Investment summary section):

"The company presents a plausible approach to monetizing underutilized edge infrastructure by enabling operators to convert idle capacity into distributed compute resources. However, there is no verified evidence of current customer adoption, production deployments, or repeatable go-to-market execution. The primary commercial concern is whether fragmented supply can be aggregated into a reliable platform with sufficient demand-side pull. As a result, while the strategic direction is aligned with broader edge computing trends, the business remains insufficiently de-risked from a commercial perspective."

---

Now perform the full evaluation using the provided evidence base.
