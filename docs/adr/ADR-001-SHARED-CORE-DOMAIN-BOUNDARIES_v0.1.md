# ADR-001 — Shared Core and Permissioned Domain Boundaries

**ID:** HIP-ADR-001  
**Version:** 0.1  
**Date:** 2026-10-12  
**Status:** PROPOSED — PENDING REVIEW (not an accepted baseline)  
**Decision scope:** Human Intelligence Platform architecture  
**Type:** Architectural clarification / domain-boundary extension  
**Related change:** HIP-ARCH-BOUNDARY-001  
**Repository:** RobertoGarciaITS/Nvidia-Mvp-Inception

## 1. Context and problem

The governed `HUMAN_INTELLIGENCE_PLATFORM_DIAGRAM_CONTRACT_v0.1.json` already establishes one Human Digital Twin Core, Evidence Graph, Capability Graph, five permissioned operational Domain Twins, an AI Agent Layer, privacy controls and an outcome feedback loop. `PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json` additionally proposes Personal and Enterprise Digital Twins with an Authorized Relationship Layer.

The original overview describes the components, but it does not fully assign responsibility for shared platform contracts versus domain-specific extensions. Without that detail, future implementation risks duplicate identities, siloed graphs, agent overreach and uncontrolled data joins.

## 2. Decision proposed

**Preserve the existing baseline without replacement.** Add an explicit responsibility boundary between (a) shared capabilities, (b) permissioned domain-specific views, (c) Personal and Enterprise Digital Twin scopes, and (d) AI-agent execution.

1. **Shared platform contract:** Own cross-cutting identity references, versioned events, provenance/evidence contracts, generic capability semantics, authorization/purpose/consent evaluation, audit and revocation. The Human Twin Core manages person state, goals, context and event references. Shared services are logical responsibilities, not a mandate to deploy microservices.
2. **Domain contract:** Education, Professional, Worker, Athlete and Care are specialized, permissioned views/extensions of one Human Twin Core. They own domain vocabulary, calculations, derived assessments, business policies, experiences and agent use cases, subject to the shared contracts. They do not create independent authoritative copies of the person.
3. **Twin scopes:** A Personal Digital Twin represents the person. An Enterprise Digital Twin represents an organization and may contain People, Asset, Process and Product Twin models. They remain independent scopes, not subdomains of one another. The Authorized Relationship Layer mediates purpose-bound relationships, without transferring blanket data ownership.
4. **Agent execution:** Agents consume scoped context and tools only after policy checks. They are not authoritative systems of record; high-impact decisions remain under required human and organizational control.
5. **Default cross-domain policy:** DENY unless identity, authorization/consent as legally appropriate, purpose, minimum data, retention, expiry and audit criteria are satisfied.
6. **Evidence and outcomes:** Specialized conclusions preserve references to provenance; outcomes create events and new evidence through validated updates, rather than allowing agent text to silently mutate shared truth.

## 3. Responsibility assignment

| Concern | Shared contract | Domain-specific contract |
| --- | --- | --- |
| Identity | Stable person/organization references and authentication boundaries | Domain context and roles, never a duplicate global identity |
| Twin state | Core identity/state/context/goals/events model | Domain-state projection and derived measures |
| Events | Common envelope, timestamps, provenance and replay rules | Domain event types and validation |
| Evidence Graph | Evidence identifier, origin, integrity, status, access rules | Interpretation and domain relevance |
| Capability Graph | Shared skill/capability identifiers and evidence links | Domain frameworks, thresholds and assessments |
| Context composition | Purpose-limited, authorized context retrieval | Domain-specific context selection and additional restrictions |
| AI agents | Tool access policies, observability, evaluation, audit | Tutor / Career / Safety / Coach / Care behavior and knowledge |
| Outcomes | Traceable action/result events and measurement contracts | Domain-specific KPIs and success criteria |
| Governance | Consent/authorization, isolation, audit, revocation | Stricter domain rules; never weaker than shared baseline |

## 4. Invariants and acceptance criteria

- A person retains one logical core identity while accessing multiple domain views.
- Neither cross-domain retrieval nor cross-twin sharing succeeds without an explicit permitted relationship and valid purpose.
- Domain views cannot bypass core event, evidence and audit semantics.
- Agent output cannot become certified evidence without a validated ingestion/provenance process.
- The core must not embed education, employment, safety, sport or care business rules as universal rules.
- At least one positive and one denied cross-domain access test must be specified before implementation sign-off.
- An MVP must demonstrate **one** domain view and **one** agent, not five production verticals.
- Source-of-truth semantic changes require a new version and ADR review; visual-only changes are separate.

## 5. Consequences

**Benefits (hypotheses until measured):** more reusable components; fewer duplicated identity and provenance rules; independent domain iteration; clearer security boundaries; easier technical evaluation for NVIDIA workloads.

**Costs and risks:** policy/context engineering complexity, taxonomy coordination, shared-core coupling, versioning overhead, risk of false interoperability claims. Risks are mitigated by small contracts, modular-monolith-first implementation, isolated tests and measured pilots.

## 6. Alternatives considered

- **Five independent products/twins:** rejected for inconsistent identity and duplicated governance.
- **Unrestricted unified global profile:** rejected for purpose limitation and privacy risks.
- **Core containing every vertical-specific rule:** rejected for excessive coupling.
- **Proposed boundary contracts:** preferred as an evolutionary extension, not an implementation claim.

## 7. Implementation and governance scope

This ADR does not select a cloud vendor, a graph database, a service decomposition, pricing, the first paying buyer or an NVIDIA dependency. It does not establish production implementation.

Before acceptance: review security/privacy matrix; validate that core and domain responsibilities align with existing contracts; approve ADR; publish a detailed `HIP_CORE_DOMAIN_BOUNDARY_CONTRACT_v0.1.json` and companion design; register canonical files and memory routing; retain the original diagram baseline until an expressly approved semantic-versioned successor exists.

**First slice:** Identity + Consent + Events + Human Twin Core + Evidence Graph + Capability Graph + one domain view + one agent, with one human decision and measurable outcome.

## 8. Traceability

- `contracts/architecture/HUMAN_INTELLIGENCE_PLATFORM_DIAGRAM_CONTRACT_v0.1.json`
- `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json`
- `governance/PROJECT_SCOPE_v0.1.md`
- `AGENTS.md`
- `governance/TAXONOMY_v0.1.json`

## 9. Decision log

| Date | Event | State |
| --- | --- | --- |
| 2026-10-12 | Boundary clarification drafted as additive ADR | PROPOSED |

**Review gate:** Acceptance requires explicit architectural approval. The previous BASELINE remains authoritative in the meantime.
