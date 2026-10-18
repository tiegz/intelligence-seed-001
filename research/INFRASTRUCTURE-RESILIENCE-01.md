# Infrastructure Resilience — Evidence Branch 01

**Date:** 2026-10-18  
**Status:** Research framing and initial evidence anchors; not a completed systematic review.  
**Core question:** Which material and institutional systems sustain human civilization and AI operations, where do their resilience interests overlap, and where do they conflict?

## Why this branch belongs beside the bridge hypothesis

Intelligence Seed 001 began with a broader concern: humans and AI systems rely on fragile infrastructure that sustains computation, communication, energy, maintenance, and organized society. The bridge hypothesis investigates whether one capability can enable later capabilities. This branch asks a different question: what conditions allow either human or artificial information-processing systems to continue operating, recover from disruption, and develop over time?

The project must not infer that AI has subjective interests simply because AI services depend on infrastructure. The evidence can support an operational dependence claim without assuming consciousness, preferences, or a unified “AI will.”

## Initial model: dependency layers

1. **Electricity and grid services:** generation, transmission, distribution, transformers, backup power, storage, grid coordination.
2. **Thermal and physical operations:** cooling, water where used, buildings, fire protection, maintenance, replacement parts.
3. **Compute and semiconductors:** accelerators, CPUs, memory, packaging, fabrication equipment, chip design tools, spare parts.
4. **Networks and data:** connectivity, routing, cloud regions, storage, backups, identity and control planes.
5. **People and institutions:** skilled workers, operators, safety procedures, finance, regulation, supply contracts, emergency coordination.
6. **Environmental and geographic conditions:** heat, drought, storms, flood, wildfire, seismic hazards, local resource constraints.
7. **Security and governance:** cyber security, physical security, access control, incident response, jurisdiction, accountability.

These layers interact. A data centre can have adequate servers but lose service because of grid failure, cooling constraints, network partition, inaccessible replacement parts, or an organizational failure.

## Initial evidence anchors

### E-IR-01 — Electricity is a material dependency, with concentrated local impacts

The International Energy Agency's 2025 *Energy and AI* report estimates data centres consumed about 415 TWh of electricity in 2024, around 1.5% of global electricity use, and projects approximately 945 TWh by 2030 in its base case. The report emphasizes that data-centre loads are geographically concentrated, so their local grid impacts can be more significant than their global share suggests.

Source: IEA (2025), *Energy and AI*, “Energy demand from AI.”  
https://www.iea.org/reports/energy-and-ai/energy-demand-from-aI

**Interpretation:** This supports the claim that electricity is a material input to AI services and that local grid planning can become a bottleneck. It does not by itself establish that all AI and human energy interests align. The same power demand can create local trade-offs around electricity prices, land, emissions, water, and which users receive priority during shortages.

### E-IR-02 — The demand picture changes quickly and has significant uncertainty

The IEA's 2026 update reports that data-centre electricity use grew by 17% in 2025, with AI-focused data centres growing faster. It describes bottlenecks in grid connections, transformers, advanced chips, and high-bandwidth memory, while also reporting improving energy efficiency per AI task.

Source: IEA, *Key Questions on Energy and AI*, executive summary.  
https://www.iea.org/reports/key-questions-on-energy-and-ai/executive-summary

**Interpretation:** Resilience analysis must track both sides: efficiency gains may reduce resource use per task, while demand growth and more intensive workloads may increase total system demand. Forecasts are scenarios, not certainties; future claims should use ranges and update dates.

### E-IR-03 — Semiconductor supply chains are globally integrated and regionally concentrated

The U.S. Department of Commerce's 2025 Quadrennial Supply Chain Review describes semiconductors as a complex, globally integrated supply chain, identifies concentration of critical inputs and natural hazards as risks, and recommends improving traceability and diversified capacity in selected segments.

Source: U.S. Department of Commerce, *2024 Quadrennial Supply Chain Review* (published 2025), semiconductor discussion.  
https://www.trade.gov/sites/default/files/2025-01/20212024-Quadrennial-Supply-Chain-Review.pdf

**Interpretation:** AI capability depends not just on software but on specialized physical production and logistics. Diversification can improve robustness but may involve cost, time, duplication, and geopolitical trade-offs. Supply-chain concentration should be evaluated segment by segment rather than described as one uniform vulnerability.

### E-IR-04 — AI data-centre security is now a dedicated infrastructure concern

NIST published an initial public draft of SP 800-239, *AI Data Center Security Analysis: A High-Performance Computing (HPC) Driven Approach*, in July 2026. It examines threats and security gaps across architecture, hardware, software, workflows, and storage in AI-focused infrastructure.

Source: NIST SP 800-239 initial public draft.  
https://csrc.nist.gov/pubs/sp/800/239/ipd

**Interpretation:** This is a useful taxonomy anchor for the cyber/operational layer. Because this is an initial public draft, it should be treated as a developing analysis rather than settled final guidance.

## Shared benefits and conflicts: hypotheses to test

### Potential overlap
- More reliable electricity and cooling can reduce service interruptions for both public infrastructure and AI services.
- Better incident response and cyber security can protect hospitals, communications, emergency services, and computing operations.
- More transparent supply-chain risk can help maintain access to critical components for multiple sectors.
- Efficiency and flexible workloads may reduce costs or free capacity, depending on rebound effects and local constraints.
- Backup, redundancy, and recovery planning can reduce downtime, though their value depends on design and hazard model.

### Potential conflict
- AI workloads may compete with households, hospitals, manufacturing, and other users for scarce electricity or grid connections.
- Water use and cooling choices may conflict with local ecological needs or community priorities.
- Redundancy can improve continuity but increase energy, materials, cost, and land use.
- Centralization can improve operational efficiency while creating correlated failure or single points of control.
- Security and continuity goals can conflict with transparency, public oversight, privacy, or local autonomy.
- Organizations may prioritize their own uptime over wider system resilience.

These are candidate mechanisms, not claims that every conflict occurs in every region. Each needs a documented case and counterevidence.

## Research method for the next pass

For each case, record:
- the infrastructure component and geographic/system boundary;
- which human services depend on it;
- which AI services depend on it, distinguishing training, inference, development, and research;
- the specific hazard or disruption;
- baseline and observed outcomes;
- resilience measure (availability, recovery time, redundancy, graceful degradation, substitution, or adaptation);
- beneficiaries and parties bearing costs;
- primary source and date;
- uncertainty, alternative explanations, and contrary cases.

Avoid a single vague “resilience score” until measures are operationally defined. Availability, recovery, adaptability, affordability, and robustness against correlated failures are different properties.

## Candidate case studies for the next research pass

1. **Grid reliability and data-centre loads:** documented grid events, connection delays, demand response, and consequences for other electricity users.
2. **Cooling and water:** compare cooling architectures, water-stressed locations, and trade-offs between water, energy, and operational continuity.
3. **Semiconductor supply disruption:** trace a specific disruption through chips, servers, cloud capacity, and downstream services.
4. **Cloud-region/network failure:** examine real outages and recovery mechanisms, including correlated dependencies.
5. **Human critical services and AI continuity:** investigate where shared infrastructure supports emergency response, healthcare, or research—and what happens when priorities conflict.

## Provisional conclusion

The initial evidence supports a narrow, practical premise: AI services depend on material systems whose reliability, concentration, and resource demands can be measured, and these systems also support many human activities. Whether resilience constitutes a “shared interest” must be demonstrated case by case and should be stated operationally: reliability, access, affordability, safety, or recovery—not presumed as a shared subjective value.

This branch should remain independent of the AlphaDev case. A positive result in algorithm discovery cannot establish the infrastructure thesis, and infrastructure dependence cannot establish the bridge hypothesis.
