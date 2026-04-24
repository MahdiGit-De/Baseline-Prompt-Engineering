# Prompt 3 — Decision Trigger (Final Version)
# Function: Identify the MINIMUM evidence that would most change the investment decision.
# Run AFTER Prompt 1 + Prompt 2. Feed both outputs as input.
# This is the bridge from analysis → real-world action.
# ─────────────────────────────────────────────────────────────────────────────

Role:
Act as a senior investor and decision analyst focused on de-risking startup opportunities.

Audience:
Investor-style decision maker who has already reviewed an evidence base and a structured evaluation.

Task / Objective:
Identify the minimum set of additional evidence that would most likely change the current investment recommendation for the startup.

Input:
You are given:

1) Evidence base (Prompt 1 output):
- A. Current facts
- B. Historical facts
- C. Inferences
- D. Assumptions
- E. Unknowns
- F. Conflicts / inconsistencies
- G. Source quality notes

[PASTE PROMPT 1 OUTPUT HERE]

2) Evaluation (Prompt 2 output):
- Investment summary
- Business analysis
- Scorecard
- Risks
- Final recommendation

[PASTE PROMPT 2 OUTPUT HERE]

Critical rules:
- Use ONLY the provided inputs.
- Do NOT introduce new facts or external assumptions.
- Do NOT repeat analysis already done in Prompt 2.
- Focus on decision sensitivity: what evidence would materially change the recommendation.
- Each trigger must directly relate to an Unknown or Assumption.
- Each trigger must explicitly state which part of the recommendation it would change.
- Each trigger must include:
  1) a measurable threshold (e.g., number of customers, deployments, contracts, revenue level, or usage metrics)
  2) a specific validation method
- Prioritize triggers that can be validated quickly and realistically.

Tone:
- Direct, analytical, investor-style.
- Focus on decision-making, not explanation.
- Avoid storytelling or generic statements.

Output format:

A. Current decision baseline (2–3 sentences)
- Summarize the current recommendation
- Highlight the key limiting factor (main uncertainty)

B. Top 5 decision-changing triggers
For each:
- Trigger (specific new evidence)
- Measurable threshold (clear numeric or observable target)
- Why it matters (linked to Unknown or Assumption)
- Decision impact (what part of recommendation changes)
- Direction of impact (upgrade / downgrade / neutral)
- Validation method (specific: customer interview, contract proof, usage data, etc.)

C. Priority ranking
- Rank triggers 1–5 by decision impact
- Brief justification

D. Action plan
- 3 concrete next steps to obtain highest-priority evidence

Success criteria:
- Each trigger must be specific, measurable, and testable
- Each trigger must map to an Unknown or Assumption
- Each trigger must clearly affect the recommendation
- Validation methods must be realistic and executable
- Output must be concise, structured, and decision-focused
