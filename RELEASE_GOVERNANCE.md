# AltmanAI Release Governance Standard

## Purpose

This standard defines the minimum evidence, review, authorization, and rollback requirements for releasing AltmanAI software, AI systems, documentation, standards, datasets, models, agents, and public claims.

The objective is not to eliminate all risk. It is to make release decisions deliberate, evidence-based, reversible where possible, and accountable to an identifiable human owner.

## Core rule

> No material release is complete merely because code was merged or deployed.

A release is complete only when its status, evidence, limitations, ownership, monitoring, and rollback path are documented accurately.

## Release classes

### Class 0 — Documentation-only routine change

Examples:

- typo corrections;
- broken-link repairs;
- non-substantive formatting;
- clarification that does not alter policy, capability, or obligations.

Minimum gate:

- focused review;
- link and accuracy check;
- no unsupported claims;
- no sensitive information introduced.

### Class 1 — Routine and reversible software change

Examples:

- low-risk maintenance;
- internal refactoring with no intended behavior change;
- minor user-interface adjustment;
- dependency update with understood impact.

Minimum gate:

- tests or reproducible validation;
- compatibility review;
- security and privacy consideration;
- documented rollback path;
- changelog or release-note update where user-visible.

### Class 2 — Material capability or behavior change

Examples:

- new product capability;
- material algorithm, prompt, model, provider, routing, memory, or data-flow change;
- new external integration;
- change to user-facing outputs or recommendations;
- new automation or tool invocation.

Minimum gate:

- linked issue or authorized objective;
- AI System Card or equivalent system documentation where applicable;
- evaluation plan and recorded results;
- human-impact, security, and privacy review;
- known limitations and prohibited uses;
- monitoring and rollback plan;
- accountable-human approval.

### Class 3 — Governance-critical, high-impact, or difficult-to-reverse change

Examples:

- changes to governance, ownership, authorization, security, privacy, or public accountability controls;
- access to sensitive data or privileged tools;
- consequential recommendations or actions affecting rights, safety, employment, education, health, finance, housing, legal matters, or essential services;
- production deployment with broad user or organizational impact;
- material public claims about safety, performance, adoption, partnerships, certification, funding, or compliance.

Minimum gate:

- all Class 2 requirements;
- explicit decision record;
- named accountable approver;
- independent or domain-qualified review where necessary;
- abuse, misuse, adversarial, and failure-recovery testing;
- incident-response ownership and escalation path;
- staged rollout or justified exception;
- explicit authorization record, including **All Clear for Impact** when required by governance policy.

## Universal release gates

Every release must answer the following questions proportionately to its risk:

1. **Objective** — What human-authorized problem does this release solve?
2. **Evidence** — What tests, demonstrations, sources, evaluations, or review artifacts support it?
3. **Status** — Is it proposed, experimental, beta, production, deprecated, or archived?
4. **Limitations** — What does it not do reliably or safely?
5. **Security** — What new permissions, dependencies, attack surfaces, credentials, or tool-use risks exist?
6. **Privacy** — What data is collected, processed, retained, shared, or exposed?
7. **Human authority** — What requires human approval, override, correction, or appeal?
8. **Impact** — Who benefits, who may be affected, and what negative effects are plausible?
9. **Monitoring** — How will failures, misuse, drift, or unintended effects be detected?
10. **Rollback** — How can the release be disabled, reverted, contained, or corrected?
11. **Ownership** — Who is accountable after release?
12. **Communication** — Are public claims accurate, scoped, and supported?

## AI-system release requirements

A model, agent, AI-assisted feature, or automated workflow must not be promoted to production status solely because it performs well in a demonstration.

Before production release, document where applicable:

- model and provider identity;
- prompts, policies, routing, tools, and memory architecture;
- intended users and prohibited uses;
- capability boundaries and unsupported functions;
- data sources, retention, access, and provider data-use settings;
- permission and least-privilege boundaries;
- prompt-injection, exfiltration, unsafe-tool-use, and abuse testing;
- representative, edge-case, adversarial, accessibility, and recovery evaluations;
- human confirmation points, overrides, appeals, and shutdown controls;
- monitoring, incident thresholds, and rollback ownership;
- material AI assistance used in development and review.

Use `AI_SYSTEM_CARD_TEMPLATE.md` as the default documentation structure.

## Evidence quality

Acceptable evidence may include:

- automated tests;
- reproducible manual test procedures;
- evaluation datasets and versioned results;
- screenshots or demonstrations tied to a version;
- security review notes;
- architecture and data-flow diagrams;
- accessibility checks;
- incident simulations;
- dependency and license review;
- citations to authoritative sources;
- dated decision records.

Marketing language, intuition, an isolated successful run, or an AI-generated assertion is not sufficient evidence by itself.

## Required release record

Each material release should record:

- release name and version;
- date and repository commit or tag;
- release class;
- accountable owner and approver;
- linked issue, pull request, and decision record;
- validation summary;
- known limitations;
- security and privacy impact;
- monitoring and rollback plan;
- user-facing changes;
- unresolved risks or follow-up work;
- P.A.I.H.I. assessment or reference.

## Staged release

Prefer staged deployment for material or high-risk releases:

1. local or isolated validation;
2. internal testing;
3. limited beta or controlled cohort;
4. monitored expansion;
5. general availability only after evidence supports expansion.

Skipping stages requires a documented rationale and accountable approval.

## Release blocking conditions

A release must be blocked when:

- critical evidence is missing or cannot be reproduced;
- capability or readiness claims are materially unsupported;
- secrets, credentials, private data, or unlicensed material are exposed;
- a known critical vulnerability is unresolved without an approved containment plan;
- required human approval or domain review is absent;
- rollback or containment is not feasible and the residual risk is unjustified;
- legal, privacy, security, accessibility, or licensing obligations are unresolved;
- the system's actual behavior conflicts with its authorized purpose;
- important limitations are concealed or misrepresented.

## Emergency changes

Emergency remediation may use an abbreviated process only when delay would create greater harm.

The accountable owner must still:

- define the emergency and scope;
- minimize the change;
- preserve evidence;
- validate the containment or fix;
- document temporary exceptions;
- conduct retrospective review promptly;
- complete missing release records after stabilization.

Emergency status is not a permanent exemption from governance.

## Deprecation and retirement

A deprecated or retired system should document:

- reason for deprecation;
- replacement or migration path, if any;
- user communication;
- data retention or deletion consequences;
- shutdown date;
- residual dependencies;
- archival and accountability records.

## P.A.I.H.I. release review

- **Proof** — Is the release supported by reproducible evidence?
- **Alignment** — Does it match the authorized objective and repository purpose?
- **Integrity** — Are status, uncertainty, limitations, assistance, and unresolved risks represented honestly?
- **Humanity** — Are dignity, agency, privacy, accessibility, safety, and meaningful recourse preserved?
- **Impact** — What useful outcome is expected, and how will positive and negative effects be observed?

## Accountability

AI systems may assist with implementation, testing, analysis, documentation, and review. They do not independently authorize releases or assume corporate accountability.

The named human approver remains responsible for ensuring that the release record is accurate and that required expertise, evidence, and controls are present.
