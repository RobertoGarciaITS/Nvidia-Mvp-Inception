# Digital Twin essence, requirements and maturity v0.1

**Status:** PROPOSED FRAMEWORK  
**Contract:** `contracts/architecture/DIGITAL_TWIN_MATURITY_CONTRACT_v0.1.json`

## What the repository already defined

The existing architecture contracts define a twin as a persistent, time-aware, evidence-linked representation with state, context, goals, relationships, actions, outcomes and governance.

They also define the general product progression:

```text
IDEA → HYPOTHESIS → PROTOTYPE → EXPERIMENT → EVIDENCE → VALIDATED PRODUCT
```

## What was missing

The repository did not yet define:

- the boundary between a profile, model, digital shadow and Digital Twin;
- explicit synchronization requirements;
- a use-case-specific maturity scale;
- evidence required to claim prediction, action or cross-twin interoperability;
- a maturity assessment for the current project.

## Essence of a Digital Twin

The Digital Twin Consortium defines a digital twin as a virtual representation of a real-world entity or process synchronized at a specified frequency and fidelity. It emphasizes current and historical data, predicted futures and outcome-driven use cases. [Digital Twin Consortium](https://www.digitaltwinconsortium.org/2020/12/digital-twin-consortium-defines-digital-twin/)

NIST describes digital twins as models that can support monitoring, diagnosis, prediction, optimization and decision support, and treats them as capable of interoperating in systems of systems. [NIST Digital Twins](https://www.nist.gov/digital-twins)

For this project:

> A Digital Twin is a persistent, time-aware, evidence-linked computational representation of an entity's state, context, goals, relationships, behavior and outcomes, updated by events and used to support governed human decisions and actions.

## Fundamental requirements

1. **Entity and ownership:** identify what the twin represents and who controls or governs it.
2. **State and time:** represent current state and preserve how it changes over time.
3. **Events and synchronization:** define what updates the twin, update frequency, required fidelity and stale-data handling.
4. **Evidence and provenance:** link claims about state or capability to source, timestamp, confidence or validation status.
5. **Context and goals:** interpret state in a situation and compare it with goals or desired outcomes.
6. **Relationships:** represent relevant dependencies, roles, resources, projects, processes or other entities.
7. **Behavior and transitions:** define how events or actions can change state.
8. **Human decision and action:** support a decision, action, simulation or operational workflow; consequential decisions keep the person in the loop.
9. **Feedback and outcomes:** record what happened after an action and use the result to update the twin or evidence.
10. **Governance:** make identity, purpose, consent or authorization, minimum data, access, retention, revocation and audit explicit.
11. **Validation and uncertainty:** expose uncertainty and validate predictions, recommendations or inferred capabilities for the specific use case.

## Proposed maturity levels

| Level | Name | Meaning | Project interpretation |
|---|---|---|---|
| M0 | Concept or Profile | Static records or concept | Student profile idea alone |
| M1 | Structured Digital Representation | State schema, ownership, access and time metadata | Current architecture contracts and proposed profile |
| M2 | Event-Linked or Observed Twin | Events update state with evidence and timestamps | First technical experiment |
| M3 | Contextual Human-in-the-Loop Twin | Context, goals, decision and audit | Minimum product-level target |
| M4 | Predictive or Scenario Twin | Validated forecasts or what-if analysis | Future capability |
| M5 | Prescriptive or Closed-Loop Twin | Authorized action, outcome and feedback | Advanced governed capability |
| M6 | Federated System of Twins | Personal, enterprise, asset, process or product twins interoperate | Long-term platform target |

These levels are a project-specific framework, not a universal industry standard. Digital Twin Consortium publishes maturity frameworks for particular business or infrastructure contexts, while its broader maturity work considers lifecycle, readiness, architecture, digital thread and sustainability. [DTC maturity assessment](https://www.digitaltwinconsortium.org/working-groups/digital-engineering/digital-twin-maturity-assessment-framework/) [DTC business maturity model](https://www.digitaltwinconsortium.org/wp-content/uploads/sites/3/2024/11/Digital_Twin_Business_Maturity_Model_20241120.pdf)

## Current project assessment

```text
Repository architecture: M1 proposed
Student profile alone: M1, not yet a full Digital Twin
Minimum project target: M3
Long-term Personal + Enterprise platform: M6
Current validated implementation: none
```

The project may not claim a validated Digital Twin until one vertical slice demonstrates:

```text
Identity + State + Event update + Evidence / provenance
+ Goal + Human decision + Measured outcome + Feedback update
```

## Research caveat

There is no single maturity scale that governs every Digital Twin domain. A manufacturing asset twin, a person-centered twin and an organizational twin may require different update frequencies, fidelity, evidence standards, safety controls and outcome measures. Maturity must therefore be assessed per use case and per twin type.
