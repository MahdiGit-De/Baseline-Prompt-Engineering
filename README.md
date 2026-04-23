# Prompt Engineering Mastery

## Purpose
This repository is built to organize and operationalize a prompt engineering system for evaluating startup opportunities. It structures prompt workflows, captures dataset outputs, compares experiment runs, and documents decision validation roadmaps.

## Workflow
1. **Prompt 1 – Evidence Extraction**: Extract current facts, historical facts, inferences, assumptions, unknowns, conflicts, and source quality notes from public information.
2. **Prompt 2 – Judgment / Evaluation**: Evaluate the evidence base and produce a structured commercial analysis, scoring, risks, and recommendation.
3. **Prompt 3 – Decision Trigger**: Identify the minimum set of evidence that would change the investment recommendation and define validation priorities.

## How to Use
1. Place prompt definitions and templates in the `/business` folder.
2. Run Prompt 1 to generate dataset outputs and save them under `/datasets`.
3. Use Prompt 2 to evaluate the generated dataset and save evaluation reports under `/evals`.
4. Use Prompt 3 to create validation roadmaps and save them under `/validation`.
5. Compare different prompt variants in `/experiments`, including Run 1, Run 2, and Run 3.

## Example Usage
- Read the prompt definitions in `/business/prompt-1.md`, `/business/prompt-2.md`, and `/business/prompt-3.md`.
- Run Prompt 1 and write the output to `/datasets/prompt-1-output.md`.
- Run Prompt 2 using the Prompt 1 output, then save the evaluation to `/evals/prompt-2-evaluation.md`.
- Run Prompt 3 and save the decision triggers to `/validation/prompt-3-triggers.md`.
- Save comparative experiment notes under `/experiments/run-1.md`, `/experiments/run-2.md`, and `/experiments/run-3.md`.

## Versioning Strategy
- Use semantic versioning for the repository: `v1.0.0`, `v1.1.0`, etc.
- Tag major prompt or workflow updates with release notes.
- Keep prompt files and dataset outputs versioned together when making structural changes.

## Folder Structure Explanation
- `/business` – Prompt definitions, templates, and project architecture notes.
- `/datasets` – Outputs from Prompt 1 and raw evidence datasets.
- `/experiments` – Comparison of multiple prompt runs and variant experiments.
- `/validation` – Decision trigger roadmaps and validation plans derived from Prompt 3.
- `/evals` – Structured evaluation reports produced by Prompt 2.
- `/schemas` – JSON/YAML schemas, metadata definitions, and structured data templates.

## Suggested Files
- `/business/prompt-1.md`
- `/business/prompt-2.md`
- `/business/prompt-3.md`
- `/datasets/prompt-1-output-run1.md`
- `/experiments/run-1-comparison.md`
- `/validation/prompt-3-roadmap.md`
- `/evals/prompt-2-scorecard.md`
- `/schemas/prompt-schema.yaml`
