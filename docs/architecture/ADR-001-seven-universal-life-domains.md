# ADR-001 — Seven universal human-life domains

**Status:** PROPOSED  
**Date:** 2026-10-03  
**Decision type:** Architecture ontology  
**Related contract:** `contracts/architecture/HUMAN_INTELLIGENCE_PLATFORM_LIFE_DOMAINS_CONTRACT_v0.1.json`

## Context

The current canonical architecture defines five practical domain twins: Education, Professional, Worker, Athlete and Care. A broader human-flourishing model is needed to represent the areas of life that a person may manage through one Human Digital Twin.

The project must avoid creating several disconnected identities or implementing all domains at once.

## Proposal

Use the following seven areas as a parallel strategic ontology:

1. Identity and Self
2. Health and Vitality
3. Learning and Capabilities
4. Work and Contribution
5. Relationships and Community
6. Resources and Material Security
7. Purpose and Flourishing

The seven domains are permissioned views of one Human Digital Twin Core. They are not seven independent twins with unrestricted data exchange.

## Mapping

| Current practical view | Seven-domain area |
|---|---|
| Education Twin | Learning and Capabilities |
| Professional Twin | Work and Contribution |
| Worker Twin | Work and Contribution |
| Athlete Twin | Health and Vitality |
| Care Twin | Health and Vitality / Relationships and Community |

## Decision

Adopt the seven-domain model as a **parallel design hypothesis** for strategic product exploration. Keep the five-domain architecture contract as the current canonical baseline until the proposal passes research, privacy review, domain-boundary review and an explicit architecture promotion decision.

## Consequences

### Positive

- Gives the platform a coherent human-flourishing ontology.
- Separates universal life areas from specialized products or workflows.
- Makes the student experience one domain view instead of the full platform.
- Provides a stable place for future financial, relational, identity and purpose use cases.

### Risks

- The domains are conceptual and may not match customer language.
- Health, care, finance and relationships involve sensitive data and stronger controls.
- Overly broad ontology could encourage premature implementation.
- Some outcomes may span multiple domains and require careful provenance.

## Required next validation

1. Review human-flourishing frameworks and competing ontologies.
2. Interview users about how they organize goals and life progress.
3. Define domain boundaries and cross-domain references.
4. Produce a permission matrix and data-sensitivity model.
5. Select one beachhead and one domain view for the MVP.

## Promotion criteria

The proposal may replace or supersede the canonical five-domain model only after a new architecture contract version, updated SVG, updated scope contract, taxonomy changes, variable-registry changes and explicit approval.
