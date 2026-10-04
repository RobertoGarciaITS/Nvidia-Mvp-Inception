# PROJECT_SCOPE_v0.1

## Human Intelligence Platform — Project Scope Contract

**Artifact ID:** HIP-GOV-SCOPE-001  
**Version:** 0.1  
**Status:** BASELINE  
**Scope owner:** Human Intelligence Platform  
**Repository:** RobertoGarciaITS/Nvidia-Mvp-Inception

---

## 1. Purpose

Define the authorized problem, product, technical and NVIDIA Inception boundaries for the Human Intelligence Platform (HIP).

This contract exists to prevent scope drift, premature implementation and confusion between the startup product roadmap and the NVIDIA Inception application track.

---

## 2. Product scope

### IN SCOPE

The Human Intelligence Platform may develop and validate:

- Human Digital Twin Core;
- identity, state, context, goals and events;
- Evidence Graph;
- Capability Graph;
- permissioned Domain Views / Domain Twins;
- AI Agent Layer;
- human-in-the-loop decisions;
- measurable outcomes and feedback loops;
- trust, privacy and governance controls;
- evidence-backed product experimentation;
- technical benchmarks;
- one initial beachhead;
- one initial domain view;
- one initial agent;
- NVIDIA workload evaluation when justified by requirements.

### OUT OF SCOPE FOR THE CURRENT MVP

Unless explicitly authorized by a later contract or ADR:

- all five domain twins implemented simultaneously;
- all five agents implemented simultaneously;
- production healthcare diagnosis;
- autonomous employment decisions;
- autonomous industrial safety authorization without human/governed control;
- unrestricted cross-domain data access;
- universal personal surveillance;
- production-scale physical AI deployment;
- broad consumer platform launch;
- speculative blockchain/crypto integration;
- premature multi-cloud complexity;
- technology adoption solely for branding;
- claims of NVIDIA partnership or endorsement.

---

## 3. Current MVP boundary

The current MVP boundary is:

```text
Identity + Consent
+
Human Twin Core
+
Events
+
Evidence Graph
+
Capability Graph
+
ONE Domain View
+
ONE Agent
```

The specific beachhead, domain view and agent remain subject to validation.

---

## 3A. Business model hypothesis

The project hypothesis is an integral Digital Twin platform with three related business motions:

```text
Human Intelligence Platform
│
├── B2C — Business to Customer
│   └── Personal Digital Twin managed by an individual
│
├── B2E — Business to Enterprise
│   └── Enterprise Digital Twin managed by an organization
│
└── B2B — Business to Business
    └── Authorized relationships between organizations and their Digital Twins
```

These motions share the Human Twin Core, Evidence Graph, Capability Graph, governance model and Authorized Relationship Layer. They are not three unrelated products.

### B2C

The customer is an individual who manages a Personal Digital Twin. The student is the first provisional beachhead for testing one domain view and one product loop. The student does not define the complete market, product or business model.

### B2E

The customer is an enterprise or organization that manages an Enterprise Digital Twin, including organizational state and nested People, Asset, Process and Product Twins. Enterprise buyer, use case, pricing and access model remain to be validated.

### B2B

The customer relationship involves organizations collaborating through projects, roles, permissions, skills, goals and outcomes. The Authorized Relationship Layer determines what context may be shared and for what purpose.

### Scope interpretation

The business model must be evaluated using a master Business Model Canvas plus separate B2C, B2E and B2B canvases. This section records a **business hypothesis**, not validated market evidence.

> Terminology note: B2E commonly means Business to Employee in other contexts. In this project, B2E explicitly means Business to Enterprise.

---

## 4. Platform domains

Current approved conceptual domains:

1. Education Twin
2. Professional Twin
3. Worker Twin
4. Athlete Twin
5. Care Twin

These are permissioned extensions/views of one Human Twin Core.

They are not separate human identities.

---

## 5. Agent scope

Current approved conceptual agents:

1. Tutor Agent
2. Career Agent
3. Safety Agent
4. Coach Agent
5. Care Agent

Agents may assist with recommendations, explanations, plans, alerts, simulations and next actions.

Agents are not sources of truth about the human and may not bypass governance, consent or required human judgment.

---

## 6. NVIDIA Inception scope

NVIDIA Inception is a separate acceleration and evaluation track.

### IN SCOPE

- application readiness;
- pitch-deck research and evidence;
- NVIDIA workload mapping;
- justified benchmarks and POCs;
- NIM / NeMo / evaluation / guardrail exploration when relevant;
- future edge, vision, Omniverse or Physical AI evaluation when relevant;
- documentation of gaps, experiments and results.

### OUT OF SCOPE

- forcing NVIDIA technology into the architecture without workload evidence;
- implying formal NVIDIA endorsement before it exists;
- presenting future NVIDIA integrations as already implemented;
- making the startup roadmap dependent on acceptance into Inception.

---

## 7. Development phases

```text
P00 Foundation / Governance
P01 Problem + Beachhead Validation
P02 Human Twin Core
P03 Evidence Graph
P04 Capability Graph
P05 One Domain View
P06 One Agent MVP
P07 Pilot / Evidence
P08 NVIDIA Workload Evaluation
P09 Domain Expansion
P10 Physical AI / Edge / Industrial Extensions
```

---

## 8. Scope gates

A downstream phase must not silently resolve an upstream uncertainty.

Key gates:

- G0 — repository/governance baseline;
- G1 — problem evidence sufficient;
- G2 — beachhead selected;
- G3 — MVP architecture approved;
- G4 — evidence/capability model demonstrated;
- G5 — one agent benchmarked;
- G6 — pilot evidence generated;
- G7 — NVIDIA workload fit demonstrated where claimed;
- G8 — expansion authorized.

---

## 9. Scope-change rule

A scope change requires an explicit artifact when it alters:

- target customer;
- MVP boundary;
- Human Twin boundary;
- domain list;
- agent authority;
- data sensitivity;
- trust/privacy assumptions;
- external platform dependency;
- roadmap phase ordering.

Use an ADR or a new version of this contract for material changes.

---

## 10. Current status

**Current project stage:** P00 / transitioning toward P01.  
**Current evidence maturity:** architecture baseline; business and product validation still incomplete.  
**Current authorized goal:** build the governed memory, research and evidence system before expanding implementation.
