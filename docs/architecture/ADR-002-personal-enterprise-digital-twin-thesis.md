# ADR-002 — Personal and Enterprise Digital Twin thesis

**Status:** PROPOSED  
**Date:** 2026-10-03  
**Decision type:** Core product and architecture thesis  
**Related contract:** `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_CONTRACT_v0.1.json`

## Context

The project needs to distinguish a true Digital Twin from a database of profiles and users. It also needs a clear separation between the representation of a person and the representation of an organization.

The proposed product thesis is:

> Human Intelligence Platform is a governed Human-in-the-Loop Digital Twin platform where people manage a Personal Digital Twin and organizations manage Enterprise Digital Twins. Authorized relationships connect them without merging their identities or data.

## Decision proposal

Define two top-level twin types:

### Personal Digital Twin

Represents the person's evolving identity, state, context, goals, evidence, capabilities, relationships and outcomes.

### Enterprise Digital Twin

Represents the organization's structure, people and capabilities, resources, processes, customers, risks, strategy and outcomes.

### Relationship layer

Represents governed interactions between a person and an enterprise, such as a role, project, authorization, skill requirement, learning objective or work outcome.

## Minimum distinction from a profile database

A profile database can answer:

> What attributes are stored for this user?

A Digital Twin must additionally answer:

> What is true now, how did it change, why do we believe it, what is the entity trying to achieve, what can happen next, what action was taken, and what outcome followed?

The minimum twin requires identity, state, events, context, goals, evidence, relationships, transition rules, feedback, governance and time/versioning.

## Consequences

### Positive

- Clarifies the product category and technical thesis.
- Prevents the student profile from being mistaken for the complete platform.
- Creates a clean boundary between person-owned and organization-owned representations.
- Enables future workforce, learning, enterprise and ecosystem workflows.

### Risks

- The concept is materially broader than the first MVP.
- Enterprise and personal data create significant privacy and governance obligations.
- “Digital Twin” can be misused as marketing language without event, state and feedback evidence.
- Cross-twin flows may create employment, health or financial risks.

## Required validation

1. Validate one Personal Twin use case with real users.
2. Define one Enterprise Twin use case and buyer.
3. Model the relationship and permission boundary between them.
4. Demonstrate state updates from events and evidence.
5. Demonstrate a human decision and measurable outcome.
6. Test whether the twin provides value beyond a profile database plus search or RAG.

## Promotion criteria

This thesis should become canonical only after the contract, architecture diagram, project scope, taxonomy, variable registry and privacy model are updated through an approved architectural decision.
