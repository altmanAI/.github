# AltmanAI Credibility Scorecard

**Baseline audit date:** July 13, 2026  
**Scope:** 14 public repositories currently visible under `github.com/altmanAI`  
**Active compliance denominator:** 13 repositories  
**Archived/historical:** 1 repository (`PAIHI-Portables`)  
**Status:** Baseline assessment — not a certification or external audit

> Credibility is not claimed. It is supported by inspectable evidence, limitations, decision records, and accountable human approval.

## Executive finding

AltmanAI's organization-level policy layer is materially stronger than its repository-level enforcement layer.

The organization already publishes governance, security, contribution, conduct, AI-assistance, P.A.I.H.I., rollback, and founder-approval expectations. The primary credibility gap is that evidence remains distributed across README files, tests, manifests, pull requests, and registry artifacts instead of being indexed through consistent `GOVERNANCE.md`, `PROOF.md`, and `DECISION_LOG.md` files in each strategic repository.

The active-portfolio baseline is **62.4/100** under the methodology below. This means the organization has a meaningful governance foundation, but it has not yet demonstrated consistent, automated, repo-level enforcement.

## Scoring method

| Dimension | Weight | What earns credit |
|---|---:|---|
| Governance adherence | 20 | Organization baseline, repo-specific authority, change classes, escalation and rollback rules |
| Proof density | 25 | Tests, CI, reproducible commands, artifacts, citations, limitations and claim-to-evidence mapping |
| P.A.I.H.I. implementation | 25 | Proof, Alignment, Integrity, Humanity and Impact demonstrated in the repository |
| AI-assistance disclosure | 15 | Material PRs identify the system, assistance type, human verification and limitations |
| Founder approval trail | 15 | Attributable approval record containing `All Clear for Impact` for material or governance-critical changes |

Ratings:

- **Strong:** 80–100
- **Substantial:** 70–79
- **Developing:** 50–69
- **Foundational:** below 50
- **Archived:** excluded from active compliance calculations

Scores are conservative. Anything not directly verified during this baseline is treated as unverified rather than compliant.

## Public repository scorecard

| Repository | Positioning | Score | Rating | Verified evidence | Primary gap |
|---|---|---:|---|---|---|
| `.github` | Active governance layer | 86 | Strong | Organization governance, security, contribution rules, conduct rules, PR template, recent AI disclosures and founder approvals | Approval rules are not yet enforced automatically |
| `canon-charter-v1` | Frozen canonical artifact | 82 | Strong | Repo governance, manifest, P.A.I.H.I. record, verification script, CI, changelog, version and approval phrase | No root `PROOF.md`; legacy AI label remains in a minted record |
| `human-first-ai` | Working reference implementation | 79 | Substantial | Runnable architecture, tests, P.A.I.H.I. scorer, explicit limitations and founder approval | Material PR omitted explicit AI-system identity; no root `PROOF.md` |
| `AltmanAI-Impact-Explorer` | Early full-stack implementation | 76 | Substantial | FastAPI/React structure, basic tests, public-data boundary and a disclosed correction PR | Dependency and deployment evidence not fully indexed; no root `PROOF.md` |
| `altmanai-sdk` | Initial public foundation | 63 | Developing | Cross-language structure, schemas, hashing/verification utilities, test commands and status labels | Production adoption and parity are not independently demonstrated; no root `PROOF.md` |
| `altmanai-master-ledger` | Active proof layer | 62 | Developing | Public ledger/registry structure, schemas, receipts and selected approval records | Evidence is partly self-attested and lacks one claim-to-artifact index |
| `DailyPilot-Engine` | Working reference implementation | 62 | Developing | Runnable Python CLI, named modules, test command and explicit production limitation | CI/coverage/privacy/accessibility evidence is not indexed; no root `PROOF.md` |
| `altmanai-masterplan` | Active execution map | 61 | Developing | Portfolio maturity labels, priorities, evidence-over-roadmap rule and founder approval requirement | No repo-specific governance, proof or decision log verified |
| `altmanai-alt-seal` | Governance and verification asset | 57 | Developing | Published hashes, Save-Receipt artifacts, local verifier and scope limitations | Internally defined trust standard lacks independent validation and decision log |
| `releaseshield-by-altmanai` | v0.1 product development | 50 | Developing | Clear scope, preliminary detection limitations, human review and proof-report design | Feature descriptions precede demonstrated working CLI/Action evidence |
| `docs` | Active documentation | 45 | Foundational | Structured docs source, preview command and organization contribution routing | Published-site parity, accessibility and product-feature accuracy are not evidenced |
| `paihi-framework` | Active development | 45 | Foundational | Development status, framework dimensions, human-authorization principles and reference implementation link | Organization-wide enforcement claims exceed currently demonstrated controls |
| `altmanai-public-hub` | Active public entry point | 43 | Foundational | Clear company purpose, product direction, contacts and current/developing labels | Product and impact claims are weakly linked to code, tests and measurable outcomes |
| `PAIHI-Portables` | Archived and consolidated | 40 | Archived | Honest archive notice states there was no working code and routes users to the SDK | Historical repository; excluded from active compliance denominator |

## Governance adherence

The `.github` repository supplies organization-level defaults for security reporting, contribution rules and conduct. It also declares its governance policy as the baseline for repositories without an approved local policy.

However, GitHub community-health inheritance is not equivalent to a repo-specific authority map. Strategic repositories still need local rules for:

- what counts as routine, material, security-sensitive and governance-critical;
- who may approve each change class;
- which files and release actions trigger founder approval;
- incident escalation and rollback criteria;
- the objective or masterplan record served by the repository.

## Proof density

Concrete proof is strongest in:

1. `canon-charter-v1` — manifests, verification tooling and CI;
2. `human-first-ai` — runnable reference code, tests and reproducible P.A.I.H.I. scoring;
3. `altmanai-sdk` — schemas, cross-language foundations and deterministic artifact tooling;
4. `DailyPilot-Engine` — working CLI, scoring modules and tests;
5. `AltmanAI-Impact-Explorer` — full-stack structure and basic API tests.

A root-level `PROOF.md` was not found in nine sampled strategic repositories: `altmanai-masterplan`, `altmanai-master-ledger`, `DailyPilot-Engine`, `altmanai-sdk`, `human-first-ai`, `releaseshield-by-altmanai`, `AltmanAI-Impact-Explorer`, `paihi-framework`, and `canon-charter-v1`.

This does not mean those repositories have no evidence. It means the evidence is not yet normalized into a claim-to-proof index.

## P.A.I.H.I. findings

### Proof

Tests, manifests, hashes and verification scripts exist in several repositories, but there is no organization-wide evidence threshold or conformance suite.

### Alignment

The current masterplan provides a clear portfolio map. Repo-specific links to formal objectives remain inconsistent.

### Integrity

Recent cleanup work has improved maturity labels and removed or corrected unsupported positioning. Remaining target-state language must stay distinguishable from shipped capability.

### Humanity

Human authorization is a documented principle. Accessibility, privacy, recourse and user-impact audits are not yet consistently evidenced per repository.

### Impact

Several repositories describe intended outcomes, but measurable success metrics and post-release observations are not consistently defined.

## AI-assistance disclosure spot check

The three-repository recent-PR spot check covered `.github`, `AltmanAI-Impact-Explorer`, and `human-first-ai`.

| Repository | Material PRs reviewed | Result |
|---|---:|---|
| `.github` | 5 founder-authored material/governance PRs | Recent material PRs consistently identify AltmanAI Model 2.0 and human authorization; one cleanup PR requested approval but did not contain an explicit AI-system disclosure |
| `AltmanAI-Impact-Explorer` | 1 material human-authored correction PR | AI assistance and `All Clear for Impact` are explicit |
| `human-first-ai` | 1 material code/governance PR | Tests and founder approval are explicit; the assisting AI system is not named |

**Confirmed correction item:** create a public correction record for the `human-first-ai` disclosure gap rather than rewriting history silently.

Dependabot or automated dependency PRs should identify the automation source through GitHub metadata and are evaluated separately from human/AI-authored material changes.

## Founder approval trail

Visible approval records exist in recent governance, identity, canonical and material code changes. The phrase is currently a manual convention, not an enforced merge requirement.

This baseline proposes a path-sensitive GitHub Action that requires an attributable comment containing exactly:

> **All Clear for Impact**

The workflow must not manufacture or automate founder approval.

## Security and dependency posture

### Public-safe finding

A July 5, 2026 code-search sweep reported no exposed-secret hits, with an explicit warning that code-search indexing can lag.

### Current limitation

No new package-manager dependency audit, native GitHub secret-scanning verification, dependency-review run or third-party secret scan was completed as part of this connector-based baseline. Therefore:

- this report does **not** claim zero vulnerabilities;
- this report does **not** certify that no secret has ever been committed;
- production repositories require live ecosystem-specific scans before the security success criteria can be checked.

Sensitive findings, if discovered, must be reported privately under `SECURITY.md` and must not be added to this public scorecard before remediation.

## Top 10 hardening scope

The current strategic top 10 for the credibility initiative are:

1. `.github`
2. `altmanai-masterplan`
3. `altmanai-master-ledger`
4. `paihi-framework`
5. `human-first-ai`
6. `altmanai-sdk`
7. `DailyPilot-Engine`
8. `releaseshield-by-altmanai`
9. `AltmanAI-Impact-Explorer`
10. `canon-charter-v1`

`PAIHI-Portables` is archived and is not treated as an active strategic implementation target.

## Mandatory repository deliverables

Each top-10 repository must add or explicitly link:

- `GOVERNANCE.md`
- `PROOF.md` or `EVIDENCE.md`
- `DECISION_LOG.md`
- dependency and supply-chain posture
- secret-scanning posture
- AI-assistance disclosure requirements
- explicit success metrics and limitations
- rollback and incident-escalation rules

## Immediate correction queue

1. Add founder-approval enforcement to the organization workflow.
2. Create the `human-first-ai` AI-disclosure correction record.
3. Add `PROOF.md` to the first implementation wave: `human-first-ai`, `altmanai-sdk`, `DailyPilot-Engine`, `ReleaseShield`, and `Impact-Explorer`.
4. Recast target-state enforcement language in `paihi-framework` until conformance checks exist.
5. Run dependency and secret scans and publish only remediated, public-safe summaries.
6. Add measurable outcome definitions to product and public-facing repositories.

## Monthly publication standard

Future revisions should publish:

- audit date and exact repository denominator;
- score changes and methodology changes;
- new evidence and validation links;
- corrected or removed claims;
- unresolved high-risk gaps;
- dependency/security status at a public-safe level;
- material PR disclosure compliance;
- founder approvals for governance-critical changes.

## Approval status

This scorecard is proposed on a review branch.

**Merge status:** Pending explicit Founder approval.  
**Required phrase:** `All Clear for Impact`

---

**Owner:** AltmanAI Model 2.0 — audit execution and evidence scaffolding  
**Accountable human authority:** Blake Hunter Altman, Founder & CEO  
**Company:** AltmanAI by Altman Family Group LLC, Pittsburgh, Pennsylvania