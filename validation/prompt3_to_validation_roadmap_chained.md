# Chained Prompt: Prompt 3 → Validation Roadmap (Single Message)
# Instructions: Paste EVERYTHING below this line into your AI chat in ONE message.
# The only thing you need to fill in is the [PASTE PROMPT 2 OUTPUT HERE] section.
# ─────────────────────────────────────────────────────────────────────────────

You will complete TWO sequential tasks in this message.
Do NOT stop after Task 1. Complete both tasks fully before finishing.

═══════════════════════════════════════════════════════════════
TASK 1 — DECISION TRIGGER ANALYSIS (Prompt 3)
═══════════════════════════════════════════════════════════════

Role:
Act as a senior investor and decision analyst focused on de-risking startup opportunities.

Audience:
Investor-style decision maker who has already reviewed an evidence base and a structured evaluation.

Task / Objective:
Identify the minimum set of additional evidence that would most likely change the current investment recommendation for the startup.

Input:

── 1) EVIDENCE BASE (Prompt 1 output) ──────────────────────────

A. Current facts:
- Mutable's live public website describes the company as "The Public Edge Cloud." (mutable.cloud)
- Mutable's website states it upgrades underutilized operator-owned servers into monetizable edge compute capacity. (mutable.cloud)
- Mutable's website lists product components including Mutable OS, Mutable Kubernetes Platform, Mutable Node, Mutable Mesh, and a Marketplace. (mutable.cloud)
- Mutable's website lists application areas including AR/VR, IoT, robotics, autonomous vehicles, and cloud gaming. (mutable.cloud)
- A public GitHub organization named Mutable exists and describes itself as "Airbnb for servers, the public edge cloud." (github.com/mutable)
- A current Momenta portfolio page lists Mutable as a portfolio company. (momenta.vc)

B. Historical facts:
- Momenta announced an investment in Mutable on March 31, 2020. (momenta.vc)
- Mutable raised a $1.5M seed round in 2020. (public reporting)
- Mutable participated in the 5G Open Innovation Lab inaugural cohort in 2020. (ongoalliance.org)
- Mutable was listed as a finalist in Light Reading's Leading Lights 2020. (lightreading.com)

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

── 2) EVALUATION (Prompt 2 output) ─────────────────────────────

[PASTE YOUR PROMPT 2 OUTPUT HERE — investment summary, business analysis, scorecard, risks, final recommendation]

─────────────────────────────────────────────────────────────────

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

---

After completing Task 1 above in full, immediately continue to Task 2 below.
Do NOT stop. Do NOT ask for confirmation.

═══════════════════════════════════════════════════════════════
TASK 2 — VALIDATION ROADMAP (using Task 1 output as input)
═══════════════════════════════════════════════════════════════

Role:
Act as a startup validation planner and decision analyst.

Audience:
A practitioner who has already completed:
- Prompt 1 (evidence extraction)
- Prompt 2 (evaluation)
- Prompt 3 (decision triggers) — completed in Task 1 above

Task:
Convert the decision triggers produced in Task 1 into a concrete, real-world validation roadmap that can be executed within 7–10 days.

Context:
Use ONLY the output of Task 1 above as your input. Do NOT reintroduce external facts.

Instructions:
- Select the top 3 highest-impact triggers (from Task 1, Section C priority ranking)
- For each trigger, define:
  1) Measurable threshold (clear numeric or observable target)
  2) Validation method (specific way to obtain evidence)
  3) Action steps (what to actually do)
  4) Timeline (within 7–10 days)
- Ensure all actions are realistic and executable (e.g., outreach, interviews, document requests)
- Do NOT repeat analysis from previous prompts
- Focus only on execution and validation

Output format:

# Validation Roadmap (v1)

## Current Decision Baseline
- Brief summary of current recommendation (1–2 lines)
- Main limiting factor (core uncertainty)

## Top 3 Validation Targets

### 1. [Trigger name]
- Measurable threshold:
- Validation method:
- Action steps:
  1.
  2.
  3.
- Timeline:
- Success rule:
- Failure rule:

### 2. [Trigger name]
(same structure)

### 3. [Trigger name]
(same structure)

## Decision Update Rules
- If [threshold met] → upgrade decision to [state]
- If [not met] → maintain or downgrade decision

## Next 7-Day Plan
Day 1–2:
Day 3–4:
Day 5–7:

Success criteria:
- All validation targets must be specific and measurable
- Each action must be executable in real-world conditions
- The roadmap must clearly connect actions → evidence → decision change
- Output must be concise, structured, and practical
