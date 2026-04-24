# Prompt Engineering Learning Tracker
# Project: Startup Evaluation System (Mutable / Edge Computing)
# ─────────────────────────────────────────────────────────────────────────────

## Progress Overview

| Day | Skill | Status | Key Output |
|-----|-------|--------|------------|
| Day 1 | Clear instructions, role, objective | ✅ Done | Baseline investor prompt (single mega-prompt) |
| Day 2 | Multi-step reasoning, evidence vs judgment separation | ✅ Done | Prompt 1 + Prompt 2 system |
| Day 3 | Output contracts (audience, tone, success criteria) | ✅ Done | Contract-grade Prompt 2 |
| Day 4 | Few-shot prompting (0 / 1 / 3 examples) | 🔄 In progress | Run 1, Run 2, Run 3 of Prompt 2 |
| Day 5 | Decision trigger prompt | ⏳ Next | Prompt 3 |
| Day 6 | Validation roadmap | ⏳ Planned | Prompt 4 |

---

## What You Learned Each Day

### Day 1 — Clear Instructions
**Core skill:** Writing a structured prompt with role, objective, rules, and output format.
**Problem with Day 1 prompt:** Evidence + analysis + decision all mixed in one pass.
**Key insight:** A well-defined prompt improves output quality immediately.
**File:** `baseline-investor-prompt.md`

---

### Day 2 — Multi-Step System
**Core skill:** Separating evidence extraction from judgment into two sequential prompts.
**Why this matters:** Mixing facts and conclusions leads to hidden hallucinations.
**Key insight:** Prompt 1 builds the data layer. Prompt 2 builds the decision layer.
**Files:** `prompts/01_evidence_extraction.md` → `prompts/02_judgment_run1_zero_shot.md`

**The pipeline:**
```
Prompt 1 (Evidence) → output → Prompt 2 (Judgment)
```

---

### Day 3 — Output Contracts
**Core skill:** Turning prompts into structured contracts with 5 elements.
**The 5 contract elements:**
1. **Audience** — who is this for?
2. **Task** — what exactly to do?
3. **Constraints** — what NOT to do / limits
4. **Output format** — how it must look
5. **Success criteria** — what "good" looks like

**Key upgrades made to Prompt 2:**
- Added `Audience:` after Role
- Added `Tone:` inside Critical rules
- Added `Success criteria:` at the end
- Tightened scoring rules (missing data → lower score)

**Key insight:** A contract removes ambiguity. The model executes a specification, not an improvisation.

---

### Day 4 — Few-Shot Prompting
**Core skill:** Adding examples to shape output style, tone, and consistency.
**The three-run method:**

| Run | Examples | Effect |
|-----|----------|--------|
| Run 1 (Zero-shot) | None | Establishes baseline — may be slightly generic |
| Run 2 (One-shot) | 1 investment summary | Improves tone and decision sharpness |
| Run 3 (Few-shot) | 3 examples (summary + risks + scorecard) | Near-professional consistency |

**Key insight:** Examples modify behavior, NOT input. Dataset (Prompt 1 output) always stays in the Input section.

**What changes between runs:**
- Tone becomes sharper and more investor-like
- Scoring becomes more conservative and evidence-anchored
- Sections become more consistent and less repetitive

**Files:**
- `prompts/02_judgment_run1_zero_shot.md`
- `prompts/02_judgment_run2_one_shot.md`
- `prompts/02_judgment_run3_few_shot.md`

---

### Day 5 — Decision Trigger Prompt (NEXT)
**Core skill:** Identifying the minimum evidence that would change the investment decision.
**Why this matters:** Converts analysis → specific actionable next steps.
**Key insight:** This is the bridge between "what we know" and "what we must find out."
**File:** `prompts/03_decision_trigger.md`

---

### Day 6 — Validation Roadmap (PLANNED)
**Core skill:** Turning decision triggers into a concrete 7–10 day execution plan.
**Why this matters:** Moves from investor analysis to real-world de-risking.
**File:** `prompts/04_validation_roadmap.md`

---

## Key Concepts Mastered

### Evidence Classification System
| Class | Definition |
|-------|-----------|
| Current fact | Directly evidenced present-state information |
| Historical fact | Past signal — does NOT prove current traction |
| Inference | Logical interpretation, not directly proven |
| Assumption | Must be true for the business to work |
| Unknown | Critical missing info that cannot be verified |

### Prompt Types by Purpose
| Prompt | Type | Risk |
|--------|------|------|
| Day 1 mega-prompt | Judgment + recommendation | ⚠️ Medium (can overreach) |
| Prompt 1 | Evidence structuring | ✅ Low (very safe) |
| Prompt 2 (Run 1–3) | Constrained judgment | ✅ Best balance |
| Prompt 3 | Decision triggers | ✅ Action-oriented |
| Prompt 4 | Validation roadmap | ✅ Execution-focused |

### The "When to Use" Rule
| Task | Prompts needed |
|------|---------------|
| Evaluate a company | Prompt 1 → Prompt 2 |
| De-risk a decision | + Prompt 3 |
| Execute validation | + Prompt 4 |
| Build a startup | Prompt 0 (pain discovery) → Prompt 1 → Prompt 2 |

---

## Mistakes to Avoid
- ❌ Running Prompt 2 without Prompt 1 output (it will invent facts)
- ❌ Mixing examples into the Input section (examples go AFTER success criteria)
- ❌ Adding too many examples (2–4 high-quality ones is optimal)
- ❌ Treating historical signals as proof of current traction
- ❌ Skipping zero-shot Run 1 (you need a baseline to measure improvement)
- ❌ Combining 3 jobs into one mega-prompt

---

## Reflection Checklist (after each run)
- [ ] Does the output strictly use the provided evidence?
- [ ] Are unknowns explicitly reflected in risks and scoring?
- [ ] Are scores conservative when data is missing?
- [ ] Is the tone truly investor-style, not generic?
- [ ] Is the final recommendation grounded in evidence?
- [ ] Are there any repetitions across sections?
