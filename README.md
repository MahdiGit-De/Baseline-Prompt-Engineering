# Startup Evaluation Prompt System
## A reusable investor-grade analysis pipeline built through prompt engineering

---

## System Architecture

```
Prompt 0 (optional)     Prompt 1              Prompt 2              Prompt 3              Prompt 4
Pain Discovery    →     Evidence         →    Judgment         →    Decision         →    Validation
(if building)           Extraction            Layer                 Triggers              Roadmap
```

---

## How to Use (Quick Start)

### For evaluating a startup:
1. Open `prompts/01_evidence_extraction.md`
2. Replace `[COMPANY]` and `[DATE]`
3. Run → copy full output
4. Open `prompts/02_judgment_run3_few_shot.md`
5. Paste Prompt 1 output into `[PASTE PROMPT 1 OUTPUT HERE]`
6. Run → copy full output
7. Open `prompts/03_decision_trigger.md`
8. Paste both outputs → Run
9. Open `prompts/04_validation_roadmap.md`
10. Paste Prompt 3 output → Run

### For one combined message (Prompt 3 + 4):
Use `validation/prompt3_to_validation_roadmap_chained.md`

---

## Prompt Library

| File | Purpose | Run order |
|------|---------|-----------|
| `prompts/01_evidence_extraction.md` | Evidence base — facts only, no judgment | 1st |
| `prompts/02_judgment_run1_zero_shot.md` | Baseline evaluation — no examples | 2nd (baseline) |
| `prompts/02_judgment_run2_one_shot.md` | Evaluation + 1 style example | 2nd (improved) |
| `prompts/02_judgment_run3_few_shot.md` | Evaluation + 3 examples — recommended | 2nd (best) |
| `prompts/03_decision_trigger.md` | What evidence would change the decision | 3rd |
| `prompts/04_validation_roadmap.md` | 7–10 day execution plan | 4th |
| `validation/prompt3_to_validation_roadmap_chained.md` | Prompt 3 + 4 in one message | Combined |

---

## Key Design Principles

### Evidence discipline
Every claim is classified as: Current fact / Historical fact / Inference / Assumption / Unknown.
Historical signals do NOT prove current commercial traction.

### Separation of concerns
- Prompt 1 = What is true? (no judgment)
- Prompt 2 = What does it mean? (no new facts)
- Prompt 3 = What would change the verdict?
- Prompt 4 = How do we find out?

### Contract-based prompting
Every prompt includes: Role → Audience → Task → Input → Rules → Tone → Output format → Success criteria

### Few-shot calibration (Day 4)
Use Run 3 (3 examples) for production. Use Run 1 to establish baseline for comparison.

---

## Learning Progress
See `learning/progress_tracker.md` for full day-by-day learning log.

---

## Experiment Logs
See `experiments/` for run comparisons and observations.
