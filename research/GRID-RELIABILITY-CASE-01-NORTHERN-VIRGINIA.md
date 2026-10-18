# Grid Reliability Case Study 01 — Northern Virginia Large-Load Transfer Event

**Research date:** 2026-10-18  
**Case date:** 2026-07-22  
**Status:** Documented event; preliminary operational account; follow-up standards work ongoing.  
**Purpose:** Examine how the electric grid and AI-adjacent infrastructure can be mutually dependent, and distinguish an observed disturbance from claims about systemic failure.

## Executive summary

On July 22, 2026, a mechanical failure removed a 230 kV transmission line from service in Northern Virginia. Data centres in Dominion Energy's service area unexpectedly disconnected from the grid and transferred to on-site backup generation. The resulting load drop produced significant voltage and frequency disturbances. PJM operators adjusted generation and dispatched reactive-power resources; PJM reported recovery of its Balancing Authority Area Control Error limit within nine minutes and no significant overall reliability impact.

PJM described the event as its largest large-load transfer event to date. Approximately 3,800 MW of load disconnected in two waves. Similar, smaller events in the same service area were reported in 2024 and 2025.

This is not evidence of a widespread blackout. It is evidence that the response behavior of large computational loads can itself become a grid-stability issue, even when the initiating transmission fault is correctly cleared and grid operators successfully manage the event.

## Primary source and supporting sources

### Primary operational account

PJM, “PJM, Dominion Review Large Load Transfer Event,” August 11, 2026.  
https://insidelines.pjm.com/pjm-dominion-review-large-load-transfer-event/

The account summarizes preliminary findings from PJM and Dominion, the event timeline, system response, earlier similar events, and standards work being considered.

### Regulatory context: large-load integration

FERC, “FERC Launches Aggressive Targeted Action to Speed Large Load Integration,” June 18, 2026.  
https://www.ferc.gov/news-events/news/ferc-launches-aggressive-targeted-action-speed-large-load-integration

FERC directed six regional grid operators to justify or reform tariffs for data centres and other large energy users. Its stated reform categories include interconnection processes, cost shifting and transparency, co-location and behind-the-meter generation, flexible large loads, and study processes for large loads near generation.

### Regulatory context: data-centre tracking and curtailment debate

Reuters, October 12, 2026.  
https://www.reuters.com/business/energy/us-panel-approves-pjms-registry-data-centers-rejects-plan-curtail-power-them-2026-10-12/

Reuters reports that FERC approved development of a PJM registry to improve information about data-centre locations, service dates, power schedules, and backup resources, while rejecting the core of a proposed temporary-curtailment plan as filed. The regulator left room for a revised proposal and raised questions about why data centres should be curtailed before other large users.

### Potential mitigation: flexible data-centre operation

Pacific Northwest National Laboratory, “Potential of Data Center Controls in Grid Services,” September 22, 2026.  
https://www.pnnl.gov/publications/potential-data-center-controls-grid-services

This study uses modeling and a modified IEEE 24-bus system to examine coordinated data-centre controls, batteries, and on-site generation. It identifies potential benefits for congestion management and stressed-grid conditions. These are modeled results, not proof that every real facility can provide the same service under all operating constraints.

## What happened, according to PJM's preliminary account

1. At 7:56 a.m., a mechanical failure caused a 230 kV line to be automatically removed from service.
2. A first wave of data-centre load—about 2,970 MW—disconnected and transferred to backup power.
3. A second wave of about 1,099 MW followed after voltage disturbances.
4. Total load transfer was approximately 3,800 MW. PJM reported system load dropping from 99,984 MW to 96,205 MW.
5. PJM dispatched generation downward to rebalance supply and demand and dispatched reactive-power resources to lower voltage.
6. PJM reported recovering the Balancing Authority Area Control Error limit within nine minutes, compared with a cited NERC standard of 30 minutes.

These figures are reproduced from PJM's operational account. They should be described as reported operational data, not an independent reconstruction. The source describes preliminary findings; later investigation or final technical reports may revise details.

## Why the event matters

### 1. Resilience is not only about keeping a facility powered

A data centre switching to backup power may protect its own service continuity, but if many facilities do so in a synchronized response, the collective change in grid demand can disturb the wider system. Local continuity and system-wide stability are related but not identical objectives.

### 2. The grid is a coupled system

The causal chain in this case was not simply “grid fails, computers stop.” A transmission fault triggered protective behavior at large loads; that behavior changed system voltage and frequency; grid operators then had to rebalance generation and use reactive-power resources. The response of one class of customer became part of the grid's dynamic behavior.

### 3. Human and AI-related services share some operational dependencies

Electric grids serve homes, hospitals, businesses, communications, and data centres. AI workloads running in data centres depend on electricity and associated physical systems. This supports a narrow operational statement: there are overlapping infrastructure dependencies.

It does **not** establish that human society and AI have identical interests, that every AI service is equally dependent, or that AI has subjective interests. The case is about systems and service dependencies.

### 4. Governance is part of resilience

The subsequent debate concerns who must provide information, who pays for new grid capacity, whether large loads should be flexible or curtailable, and how rules should treat different users. These are not purely technical questions. The design of tariffs, interconnection rules, emergency procedures, and accountability influences whether reliability costs are shared fairly.

## Shared benefits and conflicts visible in this case

### Possible shared benefits
- Better coordination between grid operators and large computational facilities.
- More accurate forecasts of facility demand, ramping, and backup-power behavior.
- Ride-through behavior designed to avoid unnecessary synchronized disconnection during disturbances.
- Carefully tested flexibility, storage, and backup resources that can help rather than destabilize grid operations.
- Clear interconnection requirements before facilities are energized.

### Potential conflicts
- Curtailing data centres can preserve supply for other users but interrupt computational services and raise questions about fair treatment.
- Building extra generation, transmission, and storage may improve reliability but impose financial, land-use, environmental, and construction costs.
- On-site backup can protect an individual facility while creating other concerns around emissions, fuel, noise, or synchronized switching.
- Rules that prioritize one class of large customer may disadvantage other industrial users or households.
- Centralized data-centre growth can bring economic benefits while concentrating grid risk in particular regions.

These are plausible trade-offs identified by the event and regulatory debate; the source material does not quantify every effect or establish that every conflict occurred during the July 22 event.

## Counterevidence and limits

- **No major reliability impact was reported.** This is evidence that the system response and operator actions contained the disturbance, not evidence of inevitable grid collapse.
- **The initiating fault was reportedly cleared correctly.** The unexpected large-load disconnection behavior, not simply a failure to clear the line fault, was central to the issue discussed by PJM.
- **The event does not isolate AI workloads.** “Data-centre load” includes computational infrastructure, but the public account does not establish that every affected workload was AI-specific.
- **The event does not prove a causal effect of AI growth on this incident.** It demonstrates a large computational-load response; wider claims about demand growth and future adequacy need separate evidence.
- **Preliminary findings can change.** The account is an operational summary, not a full independent forensic report.
- **A single event is not a prevalence estimate.** It cannot tell us how frequently similar events occur across all grids or facilities.
- **Mitigation is possible.** PJM, Dominion, FERC, NERC, and facilities can change standards, controls, and operating procedures. The case should be used to test solutions as well as document risk.

## Evidence assessment

| Claim | Assessment | Reason |
|---|---|---|
| Large computational loads can disconnect in a way that affects grid dynamics | Strong for this documented event | PJM reports an approximately 3,800 MW load transfer and voltage/frequency disturbance |
| Operators can contain a major load disturbance without a widespread outage | Strong for this event | PJM reports recovery of the control-error limit within nine minutes and no significant overall reliability impact |
| Data-centre behavior should be included in grid planning and reliability standards | Strongly motivated; standards work ongoing | PJM identifies ride-through concerns; FERC/NERC processes address computational loads |
| Data centres can always act as beneficial flexible grid resources | Not established | PNNL study is modeling; real capability depends on workload, controls, contracts, and operational constraints |
| AI and human society have a unified shared interest | Not established | Shared infrastructure dependence does not imply identical interests or subjective preferences |
| AI load growth will necessarily cause blackouts | Not established | One event cannot establish this, and the grid response in this case avoided a major reliability impact |

## Research questions for the next pass

1. What did Dominion's later technical investigation conclude, if a final public report is available?
2. What standards or interconnection changes did PJM and NERC subsequently propose, and what is their current status?
3. How do data-centre ride-through settings compare with those of other large loads and inverter-based resources?
4. What evidence shows whether flexible computing workloads can shift or reduce demand during grid stress without unacceptable service or safety consequences?
5. How are costs of new generation, transmission, and reliability services allocated between large data centres and other ratepayers?
6. Can we find a contrasting case in which large-load flexibility measurably improved grid operation, rather than only a case where load behavior created a disturbance?

## Provisional conclusion

The July 22, 2026 PJM/Dominion event is a strong initial case for the infrastructure-resilience branch because it reveals a two-way coupling: grid conditions affected data-centre power behavior, and the response of those facilities affected grid voltage and frequency. The system's successful recovery is as important as the disturbance.

The defensible takeaway is not that AI threatens the grid or that AI and humans share one interest. It is that large computational infrastructure is becoming a material participant in a coupled power system, so its behavior, flexibility, backup arrangements, and costs must be considered alongside the needs of other grid users. Whether particular resilience measures produce net shared benefits is an empirical question for further cases.
