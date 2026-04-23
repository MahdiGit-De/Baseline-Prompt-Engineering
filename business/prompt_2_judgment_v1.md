## Changelog
- v1.0: Initial version (Day 6 system build)

# Prompt 2: Judgment Evaluation

## Version
v1.0

## Purpose
This prompt evaluates a startup's commercial credibility based on a provided evidence base, producing structured analysis, scoring, risks, and recommendations.

## When to Use
Use this prompt after completing Prompt 1. It takes the evidence base as input and generates a comprehensive evaluation report.

## Full Prompt

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
- Mutable raised a $1.5M seed round in 2020. (public reporting)
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
- Scores must reflect evidence strength (missing data → lower score).
- Unknowns must appear explicitly in risks and final recommendation.
- No section may exceed 5–6 bullet points or short paragraphs.

Examples (follow these styles exactly):

Example 1 — Investment summary:
"The company presents a plausible approach to monetizing underutilized edge infrastructure by enabling operators to convert idle capacity into distributed compute resources. However, there is no verified evidence of current customer adoption, production deployments, or repeatable go-to-market execution. The primary commercial concern is whether fragmented supply can be aggregated into a reliable platform with sufficient demand-side pull. As a result, while the strategic direction is aligned with broader edge computing trends, the business remains insufficiently de-risked from a commercial perspective."

Example 2 — Risk section style:
- No verified demand-side adoption: absence of customer evidence limits confidence in real market need.
- No proven supply-side commitments: lack of confirmed operator contracts creates execution uncertainty.
- Two-sided marketplace risk: requires simultaneous supply and demand scaling.
- Unclear unit economics: no data on pricing, utilization, or margins.
- GTM uncertainty: no evidence of repeatable sales motion.

Example 3 — Scorecard style:
- problem-solution fit: 3/5 — plausible but not evidenced by adoption
- GTM feasibility: 2/5 — no proof of repeatable customer acquisition
- scalability: 2/5 — dependent on multi-party coordination and standardization

---

Now perform the full evaluation using the provided evidence base.

## Usage Instructions
1. Replace the Input section with the actual evidence base from Prompt 1 output.
2. Update the startup name ("Mutable") and date as needed.
3. Provide the prompt to an AI model.
4. The output will be a complete evaluation report.
5. Save the output in the `/evals` folder as `prompt-2-evaluation-[startup].md`.

## Notes for Improvement
- Add customizable scoring rubrics for different investment stages.
- Integrate quantitative metrics for more objective scoring.
- Develop modular sections for easier customization per industry.