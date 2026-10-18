# Benefit Assessment 01 — What Grid Flexibility Has Actually Established

**Research date:** 2026-10-18  
**Status:** Evidence synthesis; benefit claims separated by evidence type  
**Question:** What benefits of flexible AI/data-centre demand are established, what remains modeled, and what counterevidence must constrain the claim?

## Executive conclusion

The evidence now supports a limited but meaningful claim: **selected AI workloads can be deliberately modulated to reduce a participating compute cluster's power draw during defined grid events while meeting specified workload-service constraints.** A peer-reviewed Phoenix field demonstration reports a 25% reduction for three hours on a 256-GPU cluster. Public experimental artifacts include time-series power data, performance data, and control code.

The evidence is less mature at the next levels. Grid-wide cost savings and avoided capacity build-out are supported by system modeling, not by the Phoenix demonstration alone. A 2026 PJM case study estimates that, under its modeled assumptions and a relatively mild-weather 2023 baseline, the system could accommodate up to 32 GW of additional flexible load with curtailment of 0.1% of annual energy consumption, concentrated in 1.2% of hours. This is a scenario result, not a guarantee that 32 GW can be connected safely under current conditions or during extreme weather.

A critical counterweight: a 2026 multi-region power-system modeling study finds that temporal flexibility lowers modeled system costs but does **not** always reduce emissions. In its modeled Mid-Atlantic and Western Interconnection cases, emissions can rise by up to 3%, depending on generation mix and investment assumptions; Texas with higher renewable penetration shows reductions up to 40%. Thus, cost benefits and emissions benefits must be assessed separately.

**Current judgment:** Technical feasibility is supported; grid-level benefits are plausible and supported by models; realized public savings and reliability improvements remain to be independently measured at operating-system scale. Environmental benefits are conditional, not inherent.

## Evidence base

### E-BEN-01 — Phoenix field demonstration

**Source:** Colangelo et al., “AI data centres as grid-interactive assets,” *Nature Energy* 11, 254–261 (2026; first published online 5 December 2025). https://doi.org/10.1038/s41560-025-01927-1

The study reports software-based power orchestration on a 256-GPU cluster running representative AI workloads at a hyperscale cloud facility in Phoenix, coordinated with Arizona Public Service and Salt River Project. The cluster reduced power use by 25% for three hours during peak demand while maintaining AI quality-of-service guarantees. The demonstrated approach did not require hardware modifications or energy storage.

**Public artifacts:** https://github.com/ai-emerald/emerald-ai-demo-may-2025  
The repository describes data files including SRP total power time series, experiment workload-performance data, DVFS sweeps, and figures' source data. The article reports the field result, while the artifact repository allows further inspection of the measurements and implementation.

**Evidence classification:** Field-demonstrated, but site/cluster-specific. The paper's collaboration and declared competing interests should be kept in mind; authors include employees of organizations involved in the work. Peer review is a strength, not a substitute for replication.

**Established:** The participating cluster's power draw could be reduced during the tested events under the study's service constraints.

**Not established by this result alone:** Whole-data-centre demand reduction of 25%; regional price reduction; avoided outages; lower consumer bills; deferred power plants or transmission; repeatability at other facilities.

### E-BEN-02 — PJM curtailment-enabled headroom analysis

**Source:** Higgins et al., “Estimating headroom and demand flexibility requirements for fast large-load integration: A PJM case study” (2026). Duke Scholars record and abstract: https://scholars.duke.edu/publication/1917768 ; preprint DOI: https://doi.org/10.2139/ssrn.7416921

The authors define curtailment-enabled headroom as additional peak consumption a system can reliably serve without adding capacity, if new loads commit to reducing net withdrawals during critical periods. In their 2023 PJM case, they estimate up to 32 GW of additional flexible load, with curtailment affecting 0.1% of annual energy consumption (293 GWh) during 1.2% of hours.

**Evidence classification:** System-modeling/case-study result. The authors explicitly note that data availability limited the analysis to a relatively mild weather year.

**Potential benefit:** A credible framework for quantifying how flexibility commitments might enable more large-load interconnection using existing system headroom.

**Limits:** This does not show that 32 GW is available today under all conditions, nor that the modeled curtailment burden is acceptable to every workload or customer. Extreme weather, future load, zonal constraints, operational rules, and real participation rates may change the result. The estimate should not be quoted without its year and assumptions.

### E-BEN-03 — Multi-region cost and emissions model

**Source:** “Flexible data centers reduce power system costs but can increase emissions,” *iScience* (2026), open-access article. https://doi.org/10.1016/j.isci.2026.116497

The study models temporal data-centre flexibility in Texas, the Mid-Atlantic, and the Western Interconnection. Its results indicate lower total system costs across the modeled regions and scenarios, but emissions outcomes vary with the generation mix. The paper reports emissions reductions of up to 40% in Texas under high renewable availability, while modeled emissions can increase by up to 3% in the Mid-Atlantic and Western Interconnection settings as flexibility shifts demand toward existing carbon-intensive baseload generation. In sensitivity analysis, the emissions advantage can disappear when renewable investment becomes less economical.

**Evidence classification:** End-to-end power-system modeling, not a measured real-world savings audit.

**Potential benefit:** Flexibility can flatten net load, change dispatch and investment choices, and lower modeled system cost.

**Counterweight:** Flexible demand is not automatically low-carbon. The result depends on which generators respond, the timing of renewable availability, and investment economics. A cost reduction is not proof of an emissions reduction.

### E-BEN-04 — Duke/Nicholas Institute load-flexibility analysis

**Source context:** Duke University describes its February 2025 analysis as a first-of-its-kind assessment of how load flexibility could help the U.S. power system absorb new demand and mitigate costly grid-capacity expansion. https://climate.duke.edu/annual-report/items/rethinking-load-growth/

A 2026 report by WRAL summarizes the analysis as estimating that shifting a portion of large data-centre demand could avoid up to $150 billion in power-plant, fuel, and transmission costs over a decade. https://www.wral.com/news/state/duke-study-data-center-load-flexibility-us-150b-savings-feb-2026/

**Evidence classification:** National-scale modeled scenario, reported here through Duke's summary and secondary reporting. The headline maximum is a scenario estimate, not realized savings or a guaranteed forecast.

**Next verification needed:** Retrieve the full technical paper, identify the low/high scenario assumptions, determine whether the $40–150 billion range refers to capital expenditure, system cost, or a specific combination, and check whether later independent analyses reproduce the estimate. Do not treat this range as a proven customer-bill saving.

### E-BEN-05 — PNNL grid-services model

**Source:** Bharati et al., *Potential of Data Center Controls in Grid Services*, PNNL-39553 (22 September 2026). https://www.pnnl.gov/publications/potential-data-center-controls-grid-services

PNNL models data-centre controls, thermal-management loads, batteries, and on-site generation on a modified IEEE 24-bus transmission system. It reports modeled potential for mitigating congestion on a weak grid and helping grid operation during stressed conditions or contingencies.

**Evidence classification:** Simulation/modeling. Useful for mechanism and scenario exploration; not a real-grid outcome measurement.

## Benefit ladder: evidence status

| Proposed benefit | Current status | Evidence needed to strengthen it |
|---|---|---|
| Reduce participating cluster power during a defined event | **Demonstrated in one field setup** | Independent replication, multiple workload types and sites |
| Preserve service constraints while reducing power | **Demonstrated under tested constraints** | Publish detailed workload-level performance and latency distributions |
| Make additional load connectable with limited curtailment | **Supported by modeled PJM case** | Updated weather/load scenarios, independent validation, real tariff and interconnection pilots |
| Reduce congestion or improve contingency operation | **Supported by models; plausible mechanism** | Utility/ISO event records, nodal constraints, dispatch/reserve data and counterfactual |
| Reduce total power-system costs | **Supported by multiple models, not yet a realized savings audit** | Measured cost accounting and transparent counterfactual; separate avoided costs from transferred costs |
| Reduce consumer bills | **Not established** | Tariff and rate-case analysis showing how savings/costs flow to different customer classes |
| Avoid blackouts or improve reliability indices | **Not established by the field demonstration** | Repeated event studies and reliability metrics against a credible counterfactual |
| Reduce greenhouse-gas emissions | **Conditional and region-dependent** | Hourly marginal emissions, dispatch response, renewable curtailment and long-run investment analysis |
| Benefit both AI operators and other grid users | **Potentially aligned, not universal** | Distributional accounting of costs, compensation, service impacts, and reliability gains |

## How to establish benefits rather than merely predict them

For each real demand-response event, record the following with timestamps and a common interval (ideally one to five minutes where available):

1. **Baseline:** Expected load absent the event, with the baseline method disclosed.
2. **Actual load:** Metered site demand before, during, and after the event.
3. **Delivered response:** Absolute MW reduced, percentage of site load, ramp rate, duration, response latency, and reliability of delivery.
4. **Rebound:** Additional demand after the event, the time needed to return to baseline, and whether the rebound creates a new peak.
5. **Locational usefulness:** Whether the site is behind the constrained line or in the relevant congestion/voltage area. A reduction elsewhere may not resolve a local bottleneck.
6. **Grid outcome:** Congestion, reserve deployment, dispatch costs, prices, emergency alerts, voltage/frequency metrics, or reliability indicators. Record which of these were actually available.
7. **Compute outcome:** Job completion, throughput, latency, SLA violations, backlog, dropped work, and effects on downstream users.
8. **Counterfactual:** What the grid and facility would likely have done without the intervention. Use matched days, dispatch models, or a pre-registered evaluation design where feasible.
9. **Cost allocation:** Operator compensation, program costs, deferred infrastructure expenditure, fuel costs, tariff effects, and which customer groups gain or pay.
10. **Emissions:** Hourly or marginal generation response, renewable curtailment, storage charging/discharging, and longer-run capacity effects.
11. **Repeatability and uncertainty:** Number of events, sites, weather regimes, confidence intervals or ranges, and exclusions.
12. **Governance:** Who can request curtailment, what services are protected, how conflicts are resolved, and who is liable if a promised response is not delivered.

A reported load reduction counts as a **facility-level outcome**. A measured change in grid operation counts as a **grid-level outcome**. A lower total cost or risk for other users counts as a **public benefit** only after the counterfactual and distribution of costs are addressed.

## Counterexamples and failure conditions to actively test

- Flexibility can increase emissions in a grid with a carbon-intensive generation mix.
- A workload shifted to another location can transfer rather than eliminate grid stress.
- A synchronized rebound after curtailment can create a secondary peak.
- Curtailment may make compute service worse or transfer delay to customers who were not part of the agreement.
- Modeled capacity savings may not materialize if transmission, local distribution, or other constraints remain binding.
- Cost reductions for the system may not lower household bills if tariff design allocates savings elsewhere.
- Voluntary flexibility may be unavailable precisely during the most severe event unless contracts, telemetry, and control systems are robust.
- Benefits can be double-counted if the same MW reduction is credited to several programs or used simultaneously to justify multiple capacity claims.

## Provisional conclusion

The strongest established benefit is currently **controlled reduction of power demand at a participating AI compute cluster under tested service constraints**. The next layer—reliability, cost, and capacity benefits—is supported by credible modeling and has a plausible physical mechanism, but needs event-level verification and transparent counterfactuals. Emissions benefits are conditional and may reverse.

This evidence supports a practical, testable research hypothesis: well-designed workload flexibility can be a useful grid resource in some settings, provided that it is measured, locationally appropriate, reliable, fairly compensated, and evaluated for rebound, emissions, and distributional effects.

It does not yet establish universal net benefits or a general human–AI shared-interest thesis. The defensible claim is narrower: human services and computational services share power-system dependencies, and carefully governed flexibility may create overlapping practical benefits under identifiable conditions.
