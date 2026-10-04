# ADR-003 — Personal and Enterprise Digital Twin reference architecture

**Status:** PROPOSED  
**Date:** 2026-10-03  
**Decision type:** Core architecture and product boundary  
**Related contract:** `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json`

## Context

The project thesis requires two distinct but related objects:

1. A Personal Digital Twin managed by a person.
2. An Enterprise Digital Twin managed by an organization.

The enterprise may contain nested twins for people, assets, processes and products. These relationships must not turn the platform into a profile database or merge personal and organizational ownership.

## Proposed decision

Adopt the Personal Digital Twin, Enterprise Digital Twin and Authorized Relationship Layer as the proposed reference architecture.

Use the term **Enterprise Digital Twin** for the product-level organization representation. Use **Asset Twin** only for a nested twin of a specific enterprise asset.

## Fundamental distinction

A profile system describes attributes. A Digital Twin represents a changing entity through state, events, context, goals, evidence, relationships, transitions, actions, outcomes and governance.

The platform must not claim Digital Twin capability until at least one workflow demonstrates state updates from events and evidence, a human decision, and a measurable outcome.

## Boundaries

- Personal and Enterprise Twins have separate ownership and access policies.
- The relationship layer is the only approved bridge between them.
- Cross-twin access is denied by default.
- The student profile is a possible first Personal Twin vertical slice, not the full product.
- Enterprise implementation requires a validated organization use case and buyer.

## Consequences

### Positive

- Clarifies the company's core thesis.
- Supports both individual and organizational users.
- Provides a place for asset, process and product twins without confusing them with the enterprise twin itself.
- Protects personal ownership and consent.

### Risks

- The combined platform is broad and must be implemented through vertical slices.
- Enterprise and personal data can be sensitive or regulated.
- The term Digital Twin may be challenged if the system only stores profiles.
- Relationship permissions become a first-class architectural concern.

## Validation required

1. Demonstrate a Personal Twin workflow beyond static profile storage.
2. Define and validate one Enterprise Twin use case.
3. Define the relationship contract between a person and an enterprise.
4. Demonstrate event-to-state update and outcome feedback.
5. Compare the workflow with a profile database, RAG system or standard SaaS record.

## Promotion criteria

This proposal can become canonical only after updating the project scope, architecture diagram, taxonomy, variable registry, file inventory, memory routing, privacy model and implementation roadmap through an approved change.
