# Bridge Rubric Test — Round 1

**Date:** 2026-10-17  
**Status:** Desk test of the rubric; not an independent inter-rater study.

## Purpose

Test whether the provisional bridge rubric distinguishes ordinary task assistance from changes in system organization and from stronger claims about future capability. This is a conceptual stress test using published literature leads and well-known examples, not a systematic review or a new empirical experiment.

## Rubric used

Each case is scored 0–2 on six dimensions:

- **B — Baseline clarity:** 0 unclear; 1 partially defined; 2 well-defined comparison.
- **M — Mechanism:** 0 speculative; 1 plausible but incomplete; 2 explicit and supported.
- **D — Demonstrated difference:** 0 asserted only; 1 some evidence; 2 directly demonstrated for the specified outcome.
- **A — Architectural change:** 0 none shown; 1 possible or limited; 2 system organization/representation changes materially.
- **F — Future capability space:** 0 no evidence; 1 plausible downstream implication; 2 credible evidence of new subsequent capability classes.
- **T — Trade-offs and failure modes:** 0 ignored; 1 partly covered; 2 explicit and material to the analysis.

The scores are qualitative prompts, not validated measurements. A high total must not be interpreted as a scientific quality score. F is intentionally hard to score highly: it requires evidence beyond immediate task improvement.

## Desk-test results

| Case | B | M | D | A | F | T | Interpretation |
|---|---:|---:|---:|---:|---:|---:|---|
| Calculator for arithmetic | 2 | 2 | 2 | 1 | 0 | 1 | Clear capability bridge; no basis here for a strong architectural or future-space claim. |
| Writing and durable records | 1 | 2 | 2 | 2 | 1 | 2 | Strong representational and sociotechnical bridge; historical effects are contingent and uneven. |
| Team navigation with instruments and procedures | 1 | 2 | 2 | 2 | 1 | 2 | Strong distributed-task description; does not by itself prove a unified group mind. |
| Major transition in cognitive architecture | 1 | 1 | 1 | 2 | 1 | 2 | Best fit for the architectural hypothesis, but historical reconstruction and possibility-space claims remain difficult. |
| AI-assisted coding in experienced developers' existing projects (METR 2025 study) | 2 | 2 | 2 | 1 | 0 | 2 | A tool-enabled task intervention with a measured negative time effect in this setting; no evidence here of a future-space bridge. |

## Why these cases receive these ratings

### 1. Calculator

For a defined arithmetic task, the comparison can be clear and the mechanism is straightforward: the device performs operations rapidly and consistently. This supports a task-level bridge. The example exposes a problem with any single "bridge score": if task assistance and architectural transitions receive the same label without subtypes, the framework overstates what a calculator demonstrates.

### 2. Writing

Writing changes how information can be represented, preserved, retrieved, copied, and circulated. But claims that literacy universally or profoundly changes cognition have been criticized; effects depend on scripts, institutions, educational practices, and cultural context. A 2023 chapter reviewing the literacy thesis notes that ethnographic and experimental evidence has not supported some broad claims of specific, widespread cognitive effects. Rebecca Emigh's 2024 review warns against framing literacy and digitality as a simple ladder of superiority.

Sources:
- https://academic.oup.com/edited-volume/45648/chapter-abstract/396358327
- https://doi.org/10.1146/annurev-soc-033022-035644

**Rubric implication:** the existence of a mechanism (durable external records) is easier to establish than a broad claim about the net cognitive effects of writing across cultures.

### 3. Distributed navigation

Hutchins's *Cognition in the Wild* documents how navigation work is distributed across people, artifacts, representations, and routines. This strongly motivates a system-level description of task performance. It does not, without additional argument, settle whether the system is literally a single cognitive agent.

Source: https://doi.org/10.7551/mitpress/1881.001.0001

**Rubric implication:** system boundaries should be selected for a specified task and explanatory purpose, not treated as a universal answer to the question "where is the mind?"

### 4. Cognitive architecture transitions

Barron, Halina, and Klein (2023) discuss transitions that may alter which cognitive architectures can evolve. This is close to the possibility-space claim but also means the seed must explain what its cross-domain framework contributes beyond existing scholarship.

Source: https://doi.org/10.1098/rspb.2023.0671

**Rubric implication:** F must be scored separately from A. A changed architecture is not by itself proof of specific downstream possibilities.

### 5. AI-assisted coding

METR's randomized study involved 16 experienced open-source developers and 246 tasks in mature projects. For the AI tools and task setting studied in February–June 2025, participants took 19% longer with AI access on average, despite expecting a speedup. This result is not a universal estimate for all developers or newer tools; other randomized studies report benefits in different contexts.

Source: https://metr.org/Early_2025_AI_Experienced_OS_Devs_Study-paper.pdf

**Rubric implication:** tool access cannot be treated as proof of increased capability. The outcome depends on task type, developer experience, codebase familiarity, tool quality, review overhead, and measurement method. Even when task speed improves, that would not establish an architectural or future-space bridge.

## What this desk test shows

1. **The three-level distinction is necessary.** Capability, architecture, and future possibility-space claims should not be collapsed into one category.
2. **The rubric needs an explicit outcome vector.** Time alone is insufficient. Track correctness, quality, cost, robustness, verification burden, dependence, recovery, and distribution of benefits and harms.
3. **Historical and biological cases have weaker counterfactuals.** A mechanism may be plausible even where controlled baselines are impossible. The evidence rating should state this limitation rather than disguise it with a numeric score.
4. **The rubric is not yet inter-rater validated.** This document is a single analyst's desk test. A real inter-rater test requires independent reviewers who classify cases before seeing these ratings.
5. **F should remain conservative.** Claims that a bridge changes future capability space should need downstream evidence, a credible mechanism, or comparative modelling—not just a story about what happened afterward.

## Revised rubric requirements

For each case, future ledger entries should include:

- the exact target task or capability;
- the system boundary and why it is appropriate;
- a counterfactual or best available baseline;
- separate outcomes for performance, cost, quality, and robustness;
- the causal mechanism and alternative explanations;
- short- and long-term effects distinguished;
- at least one failure, null, or adverse effect;
- a statement of what evidence would downgrade or reject the claim.

## Conclusion

The rubric is useful as a checklist that forces explicit baselines, mechanisms, outcomes, and trade-offs. It is not yet a validated scale, and the current desk test cannot establish inter-rater reliability. Its strongest function is to prevent a narrow task improvement from being mistaken for a transformation in the future possibilities of cognition.
