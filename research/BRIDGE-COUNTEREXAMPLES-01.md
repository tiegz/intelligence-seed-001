# Counterexample Search — Bridge Hypothesis Round 1

**Date:** 2026-10-17  
**Status:** Preliminary counterexample map based on a scoped literature search; not a systematic review.

## Purpose

A useful framework must survive more than examples selected because they look like progress. This document collects cases that limit, complicate, or potentially contradict strong interpretations of the bridge hypothesis.

A counterexample need not show that no capability changed. It may instead refute a stronger claim—for example, that a change reliably improves cognition overall, that all users benefit, or that new capability necessarily produces a broader future possibility space.

## Counterexample 1 — Literacy does not produce a uniform cognitive transformation

**Strong claim challenged:** Writing or literacy reliably transforms cognition in a universal, predictable way.

The literature on the "literacy thesis" includes influential claims that literacy produces broad cognitive changes. A 2023 review chapter notes that ethnographic and experimental studies have not supported some claims of specific, widespread, profound cognitive effects, leading researchers to qualify or narrow the thesis. Emigh's 2024 review shows how narratives that rank literacy above orality can embed Eurocentric assumptions and overlook reciprocal, historically contingent relationships among oral, literate, and digital practices.

Sources:
- https://academic.oup.com/edited-volume/45648/chapter-abstract/396358327
- https://doi.org/10.1146/annurev-soc-033022-035644

**What it refutes:** A simple story in which one representational technology automatically makes people more intelligent or makes one culture cognitively superior.

**What it does not refute:** That durable records support particular capabilities, such as preserving and revisiting information.

**Rubric update:** Record the target outcome and social context. Do not infer a global increase in intelligence from the presence of writing.

## Counterexample 2 — Distributed systems can fail through coordination errors

**Strong claim challenged:** Distributing cognition across people, tools, and procedures necessarily improves task performance.

Busby's analysis of 75 design-error cases in complex process-plant design examined failures in interactions among designers, design tools, formal organizations, and the wider environment. Errors often involved absent or unattended cues.

Source: https://doi.org/10.1016/S0142-694X(00)00028-4

**What it refutes:** The assumption that adding components, communication channels, or distributed expertise automatically improves the whole system.

**What it does not refute:** That distributed systems can perform tasks through coordinated representations and operations.

**Rubric update:** Explicitly test interface failures, missing signals, responsibility gaps, communication overhead, and whether the combined system is more reliable than its best available alternative.

## Counterexample 3 — AI assistance can slow down skilled work

**Strong claim challenged:** Adding AI to a cognitive workflow necessarily expands effective capability.

METR's randomized controlled trial studied 16 experienced open-source developers performing 246 tasks in mature repositories. For the early-2025 tools and tasks tested, AI access increased task completion time by 19% on average, despite developers expecting it to help.

Source: https://metr.org/Early_2025_AI_Experienced_OS_Devs_Study-paper.pdf

**Important qualification:** This is a context-specific result, not proof that AI always slows coding. A separate randomized trial involving 96 Google software engineers reported faster completion of a complex enterprise-grade task, with a best estimate around 21% faster but a wide confidence interval. Another set of three field experiments across 4,867 developers reported increased completed tasks with AI assistance. Different tasks, tools, populations, and outcome measures can produce different results.

Sources:
- https://arxiv.org/abs/2410.12944
- https://www.microsoft.com/en-us/research/publication/the-effects-of-generative-ai-on-high-skilled-work-evidence-from-three-field-experiments-with-software-developers/

**What it refutes:** Treating tool availability, user enthusiasm, benchmark performance, or a plausible mechanism as sufficient evidence of net productivity gains.

**What it does not refute:** That AI can improve performance in some workflows or may contribute to the development of later systems.

**Rubric update:** Measure net outcomes including verification, rework, defect rates, time to understand unfamiliar code, and long-run maintainability—not only generation speed or subjective impressions.

## Counterexample 4 — Integration can improve coordination while increasing systemic vulnerability

**Strong claim challenged:** More integration is always a net improvement.

Systems engineering and critical-infrastructure research distinguish benefits from interdependence from risks such as cascading failure, common-mode failure, and dependence on shared components. The OECD's critical-infrastructure resilience work treats interdependencies as a source of both system-level coordination and systemic risk.

Source: https://doi.org/10.1787/02f0e5a0-en

**What it refutes:** A scalar "more connected = more intelligent = better" model.

**What it does not refute:** That integration can create new system-level capabilities.

**Rubric update:** Assess capabilities as a vector and include failure containment, redundancy, recoverability, and who bears the risk. The same architectural change can be beneficial for normal operations and harmful under disruption.

## Counterexample 5 — Later success does not prove an earlier change was aimed at it

**Strong claim challenged:** Because a later capability emerged, the earlier change should be understood as a step toward that capability.

Evolutionary theory distinguishes selection acting on current effects from later consequences that were not anticipated. Cognitive-transition research explicitly cautions against retrospective, teleological interpretations.

Source: https://doi.org/10.1098/rspb.2023.0671

**What it refutes:** Reading a future outcome backward as the purpose or inevitable result of an earlier transition.

**What it does not refute:** That earlier structures can alter which later developments become feasible.

**Rubric update:** Separate the mechanism and selective/developmental pathway at the time from later consequences. The fact that a later capability became possible is not proof that it was inevitable or that the transition was beneficial overall.

## Provisional result

These cases do not invalidate the narrow bridge concept. They do invalidate several easy but unjustified expansions of it:

- bridges are not necessarily beneficial;
- capability changes are not necessarily global intelligence gains;
- integration is not always an improvement;
- a successful outcome does not prove inevitability or purpose;
- tool availability does not prove net benefit;
- a broad analogy across domains does not establish a common causal mechanism.

The concept remains viable only if it records baseline, target capability, mechanism, context, trade-offs, and counterfactuals. A bridge can be local, costly, reversible, or net harmful. The framework should describe those outcomes rather than defining them away.

## Remaining counterexample work

This is a first map, not an exhaustive search. Next rounds should look specifically for:
1. external-memory tools that reduce unaided recall or create brittle dependence;
2. communication systems where additional information lowers decision quality through overload;
3. biological changes that improve one function while imposing major costs elsewhere;
4. automation that raises local throughput but degrades system-level safety or skill retention;
5. technical systems whose capabilities collapse when a shared infrastructure component fails.

A future version should add direct primary studies for each category and distinguish evidence of a trade-off from evidence of a net negative outcome.
