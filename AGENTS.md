# AGENTS.md

## Human Intelligence Platform — Agent Execution Contract

**Repository:** `RobertoGarciaITS/Nvidia-Mvp-Inception`  
**Repository role:** Governed control plane for architecture, research, evidence, memory and execution  
**Scope:** Human Intelligence Platform + separate NVIDIA Inception technical/application track  
**Status:** Baseline operating contract  
**Applies to:** Codex, coding agents, research agents, document agents, AI copilots and automated workflows operating in this repository.

---

# 1. Mission

Agents working in this repository must help transform the Human Intelligence Platform from:

```text
VISION
→ HYPOTHESIS
→ ARCHITECTURE
→ EXPERIMENT
→ EVIDENCE
→ VALIDATED PRODUCT
```

without collapsing those stages into one another.

The repository values:

```text
TRACEABILITY
EVIDENCE
MINIMUM SCOPE
REVERSIBILITY
SECURITY
HUMAN CONTROL
```

over speed or speculative completeness.

---

# 2. Read order

Before modifying anything, read in this order:

1. `AGENTS.md`
2. `memory/AGENT_MEMORY_MANIFEST_v0.1.json`
3. `governance/PROJECT_SCOPE_v0.1.md`
4. `governance/TAXONOMY_v0.1.json`
5. `governance/FILE_INVENTORY_v0.1.json`
6. `governance/VARIABLE_REGISTRY_v0.1.json`
7. `README.md` for human-oriented project orientation
8. task-specific contract(s), architecture, research and evidence artifacts
9. active issue, task or execution order

After the bootstrap files, use the memory manifest to load the **smallest relevant context bundle** for the task. Do not reread or infer the entire repository when the manifest provides a narrower authoritative path.

If instructions conflict, use this precedence:

```text
Explicit human instruction
        ↓
Repository contract / governance
        ↓
Architecture contract
        ↓
Active task / issue
        ↓
README explanatory material
        ↓
Agent inference
```

When conflict remains unresolved, stop the affected change and surface the conflict.

---

# 3. Source-of-truth rule

The semantic source of truth for the current platform diagram is:

`contracts/architecture/HUMAN_INTELLIGENCE_PLATFORM_DIAGRAM_CONTRACT_v0.1.json`

The expanded Personal and Enterprise Digital Twin architecture is governed by:

`contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json`

The maturity semantics are governed by:

`contracts/architecture/DIGITAL_TWIN_MATURITY_CONTRACT_v0.1.json`

The canonical repository-native visual representation is:

`assets/architecture/human-intelligence-platform/human-intelligence-platform-overview_v0.1.svg`

Rule:

```text
JSON CONTRACT
    ↓ governs semantics
SVG
    ↓ canonical visual
PNG / PDF / PPTX
    ↓ derived artifacts
```

Never change semantic architecture only by editing the SVG.

If semantics change:

1. update or supersede the contract;
2. determine whether an ADR is required;
3. update the visual;
4. update dependent documentation;
5. record the change through Git.

---

# 4. Project boundaries

The Human Intelligence Platform currently includes these conceptual layers:

```text
Personal Digital Twin
Enterprise Digital Twin
Authorized Relationship Layer

Domain Twins / Permissioned Views

Evidence Graph
Human Digital Twin Core
Capability Graph

AI Agent Layer

Human Data Sources

Recommendations
Human Decisions
Actions
Measurable Progress

Trust / Privacy / Governance
```

The Human Digital Twin Core contains the conceptual components:

```text
Identity
State
Context
Goals
Events
```

Do not introduce new layers, graphs, agents, domains or trust boundaries merely because they sound useful.

New architecture must be justified by a requirement or experiment.

---

# 5. Domain model

The approved architecture has two representation scopes:

- **Personal Digital Twin:** a person's persistent, goal-oriented and permission-aware representation.
- **Enterprise Digital Twin:** an organization's persistent representation, including organization state and nested People, Asset, Process and Product Twins.
- **Authorized Relationship Layer:** governed relationships using roles, projects, permissions, skills, goals and outcomes.

Current approved operational domain views:

- Education Twin
- Professional Twin
- Worker Twin
- Athlete Twin
- Care Twin

Interpret the five operational domains as **permissioned domain views/extensions of one Human Twin Core**, not independent identities. They remain the current baseline for implementation scope.

The seven-domain human flourishing model is an **organizational proposal** for the Personal Digital Twin, not a claim that seven domains are implemented. It includes Identity and Self, Health and Vitality, Learning and Capabilities, Work and Contribution, Relationships and Community, Resources and Material Security, and Purpose and Flourishing.

The Enterprise Digital Twin has a separate proposed domain organization: Organization and Identity, People and Capabilities, Resources and Assets, Processes and Operations, Customers and Ecosystem, Risk and Compliance, and Strategy and Outcomes. Treat this as architecture-level scope until an enterprise buyer and use case are validated.

An agent must not assume that all domain data is mutually accessible.

Default policy:

```text
DENY CROSS-DOMAIN ACCESS
unless explicitly authorized
```

---

# 6. Agent model

Current conceptual agents:

- Tutor Agent
- Career Agent
- Safety Agent
- Coach Agent
- Care Agent

Agents are not authoritative sources of human truth.

They consume authorized context.

Expected conceptual context contract:

```text
Authorized Twin State
+
Relevant Evidence
+
Capability Graph
+
Current Context
+
Goals
+
Domain Knowledge
+
Policies
```

Agent output may include:

- recommendation;
- explanation;
- plan;
- alert;
- simulation;
- next action.

Human decisions remain authoritative where the workflow requires human judgment.

---

# 7. Evidence discipline

Never present an assumption as evidence.

Use this internal classification when useful:

| Tag | Meaning |
|---|---|
| `[F]` | Fact |
| `[E]` | Evidence |
| `[H]` | Hypothesis |
| `[A]` | Assumption |
| `[I]` | Inference |
| `[P]` | Projection |
| `[V]` | To be validated |

Maturity progression:

```text
IDEA
→ HYPOTHESIS
→ PROTOTYPE
→ EXPERIMENT
→ EVIDENCE
→ VALIDATED PRODUCT
```

Do not skip stages in documentation, code comments, pitch materials or status reports.

---

# 8. MVP discipline

The current MVP target is intentionally small:

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

An agent must not expand the MVP to all domains or all agents without an explicit task.

Default rule:

```text
IF NOT REQUIRED TO TEST THE CURRENT HYPOTHESIS
→ DEFER
```

---

# 9. Development roadmap

Use this conceptual sequence unless a governed decision changes it:

```text
P00 Foundation / Governance
 ↓
P01 Problem + Beachhead
 ↓
P02 Human Twin Core
 ↓
P03 Evidence Graph
 ↓
P04 Capability Graph
 ↓
P05 One Domain View
 ↓
P06 One Agent MVP
 ↓
P07 Pilot / Evidence
 ↓
P08 NVIDIA Evaluation
 ↓
P09 Domain Expansion
 ↓
P10 Physical AI
```

Do not implement downstream phases in a way that bypasses unresolved upstream assumptions.

---

# 10. NVIDIA-specific rule

NVIDIA technology must be introduced from workload evidence, not branding.

Required reasoning pattern:

```text
WORKLOAD
→ REQUIREMENT
→ ALTERNATIVES
→ BENCHMARK
→ NVIDIA CAPABILITY
→ POC
→ EVIDENCE
→ DECISION
```

Forbidden reasoning pattern:

```text
NVIDIA PRODUCT
→ FIND A USE CASE
```

Potential areas such as NIM, NeMo, Jetson, Metropolis, Omniverse or Physical AI are candidates only.

Do not claim:

- NVIDIA partnership;
- NVIDIA endorsement;
- production dependency;
- benchmark superiority;
- customer use;

unless supported by current evidence.

---

# 11. Research rule

When research is required:

1. define the question;
2. define what would falsify the hypothesis;
3. prefer primary sources;
4. capture source, date and scope;
5. distinguish global evidence from Mexico-specific evidence;
6. distinguish scientific evidence from commercial claims;
7. record uncertainty;
8. do not silently reconcile conflicting sources.

Research should produce a reusable artifact, not only chat prose, when it materially affects architecture, market claims or product decisions.

---

# 12. Architecture change control

A change requires an ADR or equivalent governed decision when it changes:

- Human Twin boundaries;
- identity semantics;
- evidence semantics;
- capability semantics;
- trust / privacy boundaries;
- cross-domain access;
- agent authority;
- persistent data model;
- system-of-record assumptions;
- external platform dependency.

Visual-only changes do not require an ADR if semantics remain unchanged.

When uncertain, treat the change as semantic.

---

# 13. File and artifact rules

Prefer predictable repository paths.

Recommended families:

```text
assets/
contracts/
docs/
governance/
research/
evidence/
roadmap/
pitch/
experiments/
benchmarks/
src/
tests/
```

Do not create empty directory trees for aesthetics.

Create a directory when there is a real artifact to place inside it.

Version governed artifacts explicitly when useful:

`NAME_v0.1.ext`

Do not overwrite a historical baseline without a reason.

Use a new version when meaning changes.

---

# 14. Naming

Preferred styles:

### Contracts / governance

```text
UPPER_SNAKE_CASE_v0.1.md
UPPER_SNAKE_CASE_v0.1.json
```

### Visual / presentation assets

```text
descriptive-kebab-case_v0.1.svg
descriptive-kebab-case_v0.1.png
```

### Source code

Follow the conventions of the selected language/framework once implementation begins.

Do not introduce inconsistent naming without explicit justification.

---

# 15. Git workflow

Default:

1. inspect current state;
2. create/identify scoped task;
3. make minimum necessary change;
4. run relevant validation;
5. inspect diff;
6. commit with meaningful message;
7. use PR review when the change is non-trivial or semantic.

Suggested commit prefixes:

```text
docs:
governance:
architecture:
research:
evidence:
feat:
fix:
test:
bench:
assets:
chore:
```

Avoid unrelated changes in the same commit.

---

# 16. Testing rule

When implementation exists, tests must match the artifact type.

Examples:

### Contracts / JSON

Validate:

- valid JSON;
- schema compatibility when applicable;
- required IDs;
- path references;
- version consistency.

### Diagrams

Validate:

- renderability;
- semantic alignment with contract;
- readable labels;
- no missing governed nodes.

### Code

Use:

- unit tests;
- integration tests;
- contract tests;
- security tests;
- benchmark tests;

according to the component.

### Agents

Evaluate at minimum:

- task completion;
- factual grounding;
- tool selection;
- policy compliance;
- determinism where expected;
- latency;
- cost;
- failure behavior;
- context isolation.

Do not report `PASS` without an executed check.

---

# 17. Security and privacy

Never commit:

- passwords;
- API keys;
- tokens;
- private credentials;
- secrets;
- raw personal data unless explicitly authorized and governed.

Prefer synthetic or de-identified test data.

For human data, consider:

- consent;
- purpose;
- minimum required data;
- retention;
- access;
- provenance;
- revocation;
- audit.

Default to least privilege.

---

# 18. Human-data rule

This project deals with potentially sensitive human context.

Never assume that because data can technically be joined, it should be joined.

Every cross-domain flow must answer:

```text
WHO is requesting?
WHAT data?
FOR WHAT purpose?
UNDER WHAT consent?
FOR HOW LONG?
WITH WHAT audit trail?
```

If those questions are not answerable, do not implement the cross-domain flow.

---

# 19. Pitch-deck rule

The pitch is downstream of evidence.

Required order:

```text
RESEARCH
→ SOURCE
→ CLAIM
→ EVIDENCE STATUS
→ COPY
→ DESIGN
```

Do not invent:

- customers;
- revenue;
- pilots;
- partnerships;
- market size;
- traction;
- benchmark results;
- technical implementation.

If a slide needs missing information, use `TBD`, `HYPOTHESIS` or block the slide.

---

# 20. Status protocol

Use statuses consistently:

```text
NOT_STARTED
RESEARCHING
DRAFT
PARTIAL
EVIDENCE_READY
REVIEW
PASS
BLOCKED
DEFERRED
REJECTED
```

A polished document is not automatically `PASS`.

`PASS` requires the acceptance criteria for that artifact/task to have been met.

---

# 21. Agent execution response

For non-trivial repository tasks, report:

```text
TASK
SCOPE
FILES READ
FILES CHANGED
VALIDATION
EVIDENCE / RESULTS
RISKS / GAPS
STATUS
NEXT GATE
```

For small changes, a concise equivalent is acceptable.

Do not claim a file was changed unless the write succeeded.

Do not claim a test ran unless it actually ran.

---

# 22. Stop conditions

Stop and surface a blocker when:

- source-of-truth contracts conflict;
- required evidence is unavailable;
- the requested change would expose secrets or personal data;
- the change crosses a governance boundary without authorization;
- an architecture decision is required but missing;
- a requested claim cannot be supported;
- a destructive action is not explicitly authorized.

Do not replace uncertainty with invention.

---

# 23. Current repository baseline

The authoritative repository inventory is:

`governance/FILE_INVENTORY_v0.1.json`

Agents must treat that registry as the canonical file catalog.

Current human-readable snapshot:

```text
README.md
AGENTS.md

assets/
└── architecture/
    └── human-intelligence-platform/
        └── human-intelligence-platform-overview_v0.1.svg

contracts/
├── architecture/
│   ├── HUMAN_INTELLIGENCE_PLATFORM_DIAGRAM_CONTRACT_v0.1.json
│   ├── PERSONAL_ENTERPRISE_DIGITAL_TWIN_CONTRACT_v0.1.json
│   ├── PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json
│   └── DIGITAL_TWIN_MATURITY_CONTRACT_v0.1.json
└── presentation/
    └── HUMAN_INTELLIGENCE_PLATFORM_PITCH_DECK_V2_CONTENT_DESIGN_CONTRACT_v0.1.json

governance/
├── PROJECT_SCOPE_v0.1.md
├── TAXONOMY_v0.1.json
├── VARIABLE_REGISTRY_v0.1.json
└── FILE_INVENTORY_v0.1.json

memory/
└── AGENT_MEMORY_MANIFEST_v0.1.json
```

The snapshot is explanatory only. If it conflicts with the file inventory, use the inventory and report the documentation drift. The Personal and Enterprise contracts define architecture semantics; they do not establish production implementation.

Do not assume additional systems are implemented simply because they appear in the long-term architecture.

---

# 24. Guiding rule

> Build only what the current hypothesis needs, preserve evidence of what happened, and keep humans in control.


# 25. Repository memory protocol

The canonical agent context router is:

`memory/AGENT_MEMORY_MANIFEST_v0.1.json`

The canonical file catalog is:

`governance/FILE_INVENTORY_v0.1.json`

The canonical variable state registry is:

`governance/VARIABLE_REGISTRY_v0.1.json`

The canonical classification vocabulary is:

`governance/TAXONOMY_v0.1.json`

Rules:

1. Use the memory manifest to select task-specific context.
2. Use the file inventory to understand each artifact's role before editing it.
3. Use the variable registry instead of inventing values for unresolved business or technical variables.
4. Use the taxonomy when creating new governed artifacts, claims or statuses.
5. If a task produces a new durable source of truth, update the appropriate registry in the same change or create the next registry version.
6. Repository memory must record **what is currently governed**, not speculative facts.
7. Never use memory files to store credentials, secrets or raw sensitive personal information.
