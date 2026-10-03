# Requirements Traceability v0.1

**Product:** Human Intelligence Platform  
**Current phase:** Concept definition and MVP requirements  
**Working roles:** Product Manager, UX/UI analyst, requirements analyst, and technical delivery coordinator

## How answers feed the project

Each answer is converted into:

1. A requirement, decision, assumption, or open question.
2. A priority and owner for validation.
3. A UX/UI implication.
4. A technical impact, including screens, data, API, permissions, or components.
5. An acceptance criterion.
6. A regression test once code exists.

No regression can run yet because the repository currently contains architecture and governance artifacts, but no application code.

## Initial requirements

| ID | Requirement / decision | Type | Priority | UX/UI impact | Acceptance criterion | Regression test |
|---|---|---|---|---|---|---|
| REQ-001 | The first user is a student. | Product hypothesis | P0 | Language and onboarding must address students. | A student can understand the purpose of the product during onboarding. | Verify the onboarding text and persona-specific flow. |
| REQ-002 | The student is the initial buyer. | Business hypothesis | P0 | Avoid institution-first purchase flows in the MVP. | MVP pricing and account assumptions identify the student as the buyer. | Verify buyer and account model remain consistent in product copy. |
| REQ-003 | The student creates a talent profile. | Functional requirement | P0 | Primary CTA and first flow create a profile. | A student can start and save a profile. | Create profile from a new session and verify persistence. |
| REQ-004 | Minimum profile fields are name, degree, degree progress, graduation date, completed projects, and projects in progress. | Data requirement | P0 | Form sections and field labels must be clear. | All required fields can be entered, validated, saved, and displayed. | Submit valid and invalid values for every field. |
| REQ-005 | The MVP profile is private and visible only to the student. | Privacy requirement | P0 | No public profile or search exposure in MVP. | An unauthenticated or different user cannot view the profile. | Test authorization with owner, anonymous, and second-user sessions. |
| REQ-006 | External visibility is a future feature. | Roadmap decision | P1 | Do not expose sharing controls in the MVP unless marked future. | MVP contains no accidental public sharing path. | Scan routes and UI actions for unauthorized profile exposure. |
| REQ-007 | After saving, the student can view the complete profile. | Acceptance criterion | P0 | Confirmation leads directly to a complete profile view. | Saved data appears accurately in the profile view. | Save, reload, and compare all fields with the submitted values. |
| REQ-008 | The repository is the development location for the demo. | Delivery decision | P0 | Product artifacts and implementation must remain traceable in the repo. | Demo code, tests, and requirements are committed to the repository. | Run repository checks and verify required files are present. |
| REQ-009 | The conceptual architecture is documented by the canonical SVG and JSON contract. | Architecture evidence | P1 | UX flows should not contradict the Human Twin, evidence, or governance model. | Product requirements reference the architecture without claiming functional implementation. | Compare implementation terminology and permissions against the contract. |

## Open questions that must become requirements

- Authentication and account creation
- Exact student segment and geography
- Whether “career progress” is self-reported or calculated
- Project fields and evidence model
- Edit, draft, and delete behavior
- Data retention and export
- Future consent flow for external visibility
- Success metric for the first student profile

## Change-control rule

When a new answer changes an existing requirement, update this file, the progress log, and the affected design or test artifact. Do not add a new button, screen, field, or data source without recording its purpose and acceptance criterion.
