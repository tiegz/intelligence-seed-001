# AI Case Study 01 — AI-Assisted Software Development as a Candidate Bridge

**Date:** 2026-10-17  
**Status:** Preliminary comparative case study; evidence scoped to published studies located for this pass.  
**Question:** Does AI-assisted software development qualify as a bridge, and at what level?

## Executive summary

AI coding assistance is a useful test because it can be evaluated against measurable outcomes, but results differ across settings. One randomized study of experienced open-source developers found slower completion with AI access; another randomized enterprise study reported faster completion; a third set of field experiments reported more completed tasks. These results should not be collapsed into a single universal productivity estimate.

The evidence supports a narrow conclusion: **AI assistance can change software-development workflows, and its measured effect depends on context and outcome.** The evidence reviewed here does not establish that AI-assisted coding is already an architectural bridge that changes the future possibility space of intelligence. That stronger claim requires evidence about downstream systems and capability changes, not merely faster or slower completion of current tasks.

## 1. Candidate bridge claim

**Candidate:** Integrating generative AI into software-development work changes the distribution of code generation, search, debugging, explanation, and review across human developers and AI tools.

**Target outcome:** Net performance of a specified software task or portfolio of tasks, measured by time, correctness, review burden, rework, defects, maintainability, and successful delivery.

**Potential levels:**
- Capability bridge if it measurably changes task outcomes.
- Architectural bridge if the workflow or system organization changes in a way that enables materially different combinations of software-development tasks.
- Possibility-space bridge only if there is credible evidence that AI assistance changes which subsequent tools or capabilities can be built, tested, or improved—not simply that a developer finishes a task faster.

## 2. Study A — METR randomized trial

**Source:** Becker, J., Rush, N., Barnes, E., & David, R. (2025), "Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity." https://metr.org/Early_2025_AI_Experienced_OS_Devs_Study-paper.pdf

### Design and result

The study recruited 16 experienced open-source developers and examined 246 tasks in mature projects with which participants had substantial prior familiarity. Tasks were randomly assigned to permit or prohibit AI tool use. In the studied setting, access to early-2025 AI coding tools increased completion time by 19% on average, even though participants expected a speed improvement.

### What this establishes

- The effect of AI assistance cannot be inferred from subjective expectations alone.
- A plausible capability extension may be offset by prompt iteration, output inspection, integration work, or verification.
- A task-level bridge can have a negative net effect under particular conditions.

### Limitations

The sample was small and highly experienced, the repositories were mature and familiar to participants, and the tools were those available during the study period. This does not establish that AI assistance generally reduces productivity. The result may differ for novices, unfamiliar code, greenfield development, other tasks, other tools, or later models.

### Bridge classification

**Capability bridge: context-dependent; net negative on completion time in this study.**  
**Architectural bridge: not established.**  
**Possibility-space bridge: not tested.**

## 3. Study B — Enterprise randomized trial with Google developers

**Source:** Paradis et al., "How Much Does AI Impact Development Speed? An Enterprise-Based Randomized Controlled Trial." https://arxiv.org/abs/2410.12944

### Design and result

This study involved 96 full-time Google software engineers and a complex enterprise-grade task. It reported that AI features significantly shortened time on task, with a best estimate of roughly 21%, while also reporting a wide confidence interval. The tools, task, and developer environment differed from the METR study.

### What this establishes

The METR slowdown should not be generalized to all coding contexts. In at least one enterprise setting, AI assistance was associated with a measured reduction in time on a defined task.

### Limitations

One complex task in one organizational setting does not establish an ecosystem-wide productivity effect. Time to task completion does not fully measure code quality, security, maintainability, future debugging costs, or organizational learning. The paper itself calls for caution in generalizing its estimate across tools and settings.

### Bridge classification

**Capability bridge: supported for task time in this particular setting, with uncertainty.**  
**Architectural bridge: not established by the time result alone.**  
**Possibility-space bridge: not tested.**

## 4. Study C — Three field experiments across organizations

**Source:** Cui, K. et al. (published online 2026), "The Effects of Generative AI on High-Skilled Work: Evidence from Three Field Experiments with Software Developers." https://doi.org/10.1287/mnsc.2025.00535; related author-hosted summary: https://www.microsoft.com/en-us/research/publication/the-effects-of-generative-ai-on-high-skilled-work-evidence-from-three-field-experiments-with-software-developers/

The research combines randomized field experiments involving 4,867 developers across Microsoft, Accenture, and an anonymous Fortune 100 company. The authors report an increase in completed tasks among developers with access to an AI-based coding assistant, with larger adoption and gains among less-experienced developers.

### What this adds

It broadens the evidence beyond a small group of experienced open-source developers and highlights that skill level and workplace context may matter.

### Limitations

The intervention, organization, tasks, and outcome definitions differ from those in METR. Completed tasks and time per task are not interchangeable outcomes. The results do not establish that the same effect applies to every codebase, tool, or developer, nor that the effect persists over time or includes downstream maintenance costs.

### Bridge classification

**Capability bridge: supported for the study's measured outcome in the sampled field settings.**  
**Architectural bridge: not established by task counts alone.**  
**Possibility-space bridge: not tested.**

## 5. Cross-study comparison

| Question | METR 2025 | Google enterprise RCT | Three field experiments |
|---|---|---|---|
| Setting | Experienced open-source developers; familiar mature projects | Enterprise developers; complex task | Multiple organizations and developer populations |
| Main reported outcome | Completion time | Time on task | Completed tasks |
| Reported direction | 19% slower with AI in this setting | Roughly 21% faster best estimate; wide interval | More completed tasks with AI access |
| Generalization caution | Small, specialized sample and dated tools | One task and organizational context | Different task and adoption settings |
| Establishes possibility-space change? | No | No | No |

These studies are not a clean head-to-head comparison. They differ in participants, tasks, tools, context, and outcomes. Their value together is to show why a bridge assessment needs explicit operational definitions and should not turn heterogeneous results into one simple headline.

## 6. The downstream question: does AI help build later cognitive infrastructure?

To test the seed's stronger hypothesis, the next unit of analysis should not be "AI helped write code." It should be a documented development chain:

1. An AI system contributes to a specific tool, workflow, model, or infrastructure component.
2. That artifact is independently evaluated against a credible baseline.
3. The artifact enables a subsequent task or system that was previously infeasible or materially more costly.
4. The later capability is measured separately from the initial productivity effect.
5. Human contributions, compute, data, existing tools, and organizational changes are recorded.
6. The workflow is tested for reliability, security, maintenance burden, and reproducibility.
7. Failed attempts and regressions are retained in the evidence record.

Examples to investigate in a future pass include AI-assisted test generation that enables broader validation, AI-supported chip design, tools used in scientific discovery, and AI agents used to build or evaluate later agent systems. These are research leads, not established examples of a possibility-space bridge.

## 7. Falsification and downgrade criteria

The stronger bridge claim should be downgraded if:
- apparent gains disappear under controlled comparison;
- human review and correction eliminate the net benefit;
- downstream capability is not measured;
- the result is attributable to additional compute, data, or human expertise rather than a change in AI-enabled organization;
- the system introduces brittle dependencies that outweigh its claimed gains in relevant conditions;
- claimed novel capability is achievable just as well without the proposed bridge;
- the result cannot be reproduced outside a single demonstration.

Conversely, the possibility-space claim would become more credible if multiple independently evaluated cases show that AI materially contributes to building a tool or architecture which reliably enables new downstream capabilities, with credible baselines and documented trade-offs.

## 8. Current ledger update

**Claim:** AI assistance changes software-development workflows and can affect task outcomes.

**Assessment:** Supported, but context-dependent; results vary by task, population, tool, and outcome.

**Claim:** AI-assisted software development is already a bridge that expands future cognitive possibility space.

**Assessment:** Not established by the studies reviewed here.

**Next action:** Select one downstream artifact case—preferably an AI-supported testing or software-development toolchain—with inspectable outputs, a credible comparison, and evidence about the subsequent capability it enabled.

## References

1. Becker, J., Rush, N., Barnes, E., & David, R. (2025). "Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity." METR. https://metr.org/Early_2025_AI_Experienced_OS_Devs_Study-paper.pdf
2. Paradis, E. et al. (2024). "How Much Does AI Impact Development Speed? An Enterprise-Based Randomized Controlled Trial." https://arxiv.org/abs/2410.12944
3. Cui, K. et al. (2026). "The Effects of Generative AI on High-Skilled Work: Evidence from Three Field Experiments with Software Developers." *Management Science*. https://doi.org/10.1287/mnsc.2025.00535
