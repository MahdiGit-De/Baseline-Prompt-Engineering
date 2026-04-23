## Changelog
- v1.0: Initial version (Day 6 system build)

# Prompt 3: Decision Trigger

## Version
v1.0

## Purpose
This prompt identifies the minimum additional evidence needed to change an investment recommendation, focusing on decision sensitivity and actionable validation steps.

## When to Use
Use this prompt after completing Prompt 1 and Prompt 2. It provides the action layer, outlining what evidence would upgrade or downgrade the recommendation and how to obtain it.

## Full Prompt

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

2) Evaluation (Prompt 2 output):
- Investment summary
- Business analysis
- Scorecard
- Risks
- Final recommendation

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

## Usage Instructions
1. Replace the Input section with actual outputs from Prompt 1 and Prompt 2.
2. Update the startup name ("Mutable") as needed.
3. Provide the prompt to an AI model.
4. The output will be a decision trigger roadmap.
5. Save the output in the `/validation` folder as `prompt-3-triggers-[startup].md`.

## Notes for Improvement
- Integrate with automated diligence tools for evidence validation.
- Add prioritization algorithms based on investment thesis strength.
- Develop follow-up prompts for evidence verification workflows.