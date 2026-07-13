# AltmanAI Q3 2026 Credibility Report — Baseline

**Report date:** July 13, 2026  
**Reporting period:** Q3 2026 baseline  
**Scope:** Current public AltmanAI GitHub portfolio  
**Status:** Proposed; pending Founder approval before merge

## Executive summary

AltmanAI has established a substantive organization-level governance framework, but repo-level evidence and automated enforcement remain inconsistent.

The current public portfolio contains **14 repositories**: **13 active** and **1 archived**. The active baseline averages **62.4/100** under the public credibility methodology in [`CREDIBILITY_SCORECARD.md`](../CREDIBILITY_SCORECARD.md).

This score is not an external certification. It measures the currently inspectable presence of governance, proof, P.A.I.H.I. implementation, AI-assistance disclosure, and founder approval records.

## Portfolio status

| Metric | Baseline |
|---|---:|
| Public repositories inventoried | 14 |
| Active repositories in compliance denominator | 13 |
| Archived repositories | 1 |
| Active average credibility score | 62.4/100 |
| Repositories scoring 70 or higher | 4 |
| Sampled strategic repositories with root `PROOF.md` | 0 of 9 |
| Confirmed material AI-disclosure gaps | 1 |
| Current dependency vulnerability status | Unverified |
| Current dedicated secret-scan status | Unverified |
| External audit completed | No |

## Strongest current evidence

### `.github`

Organization-level governance, security policy, contribution rules, conduct policy, AI-system policy, issue forms, and a detailed pull-request template are published. Recent material governance PRs generally contain explicit AI-assistance disclosure and founder authorization.

### `canon-charter-v1`

The repository includes local governance, a manifest, a P.A.I.H.I. record, verification tooling, CI, versioning, a changelog, and a visible approval statement. It is the most complete artifact-integrity repository in the current portfolio.

### `human-first-ai`

The repository presents a runnable P.A.I.H.I. reference architecture with tests and a reproducible scoring demonstration. The implementation is explicitly labeled early and minimal rather than production-complete.

### `AltmanAI-Impact-Explorer`

The repository describes a concrete full-stack implementation and basic tests. Its material metadata-correction PR preserved the integrity trail while explicitly disclosing AltmanAI Model 2.0 assistance and founder authorization.

## Confirmed gaps

1. **Evidence is scattered.** Nine sampled strategic repositories lacked a root-level `PROOF.md` even when tests, manifests, schemas, or PR evidence existed elsewhere.
2. **Approval is manual.** `All Clear for Impact` is a documented convention, but no required status check currently verifies that an attributable founder comment exists for governed paths.
3. **AI disclosure is not universal.** The material `human-first-ai` PR reviewed in this baseline included test evidence and founder approval but did not name the assisting AI system.
4. **Dependency posture is unverified.** No current ecosystem-specific dependency scans were executed in this connector-based baseline.
5. **Secret posture is provisional.** A prior code-search sweep reported no hits, but code search is not a substitute for native or dedicated secret scanning.
6. **Outcome metrics are weak.** Product and public-facing repositories often describe intended value without defining measurable success or observed post-release impact.
7. **Framework language exceeds enforcement.** `paihi-framework` contains target-state language that implies organization-wide assurance before conformance checks and repo-level evidence are consistently deployed.

## Corrections and integrity actions

### Required public correction

Create a correction issue or decision-log entry for the missing AI-system identity in the material `human-first-ai` PR. Preserve the original PR history; do not rewrite it to create the appearance that disclosure was present at merge time.

### Required language correction

Revise P.A.I.H.I. target-state claims so they distinguish:

- the framework's intended standard;
- controls currently implemented in code;
- controls adopted by specific repositories;
- controls not yet enforced organization-wide.

## Foundational work proposed in this change set

- publish `CREDIBILITY_SCORECARD.md`;
- publish this Q3 2026 baseline report;
- add a path-sensitive founder approval workflow;
- open a reviewable PR rather than merging directly;
- preserve the exact human approval phrase as a manual founder decision.

## Next reporting targets

The next credibility report should measure:

- top-10 adoption of `GOVERNANCE.md`, `PROOF.md`, and `DECISION_LOG.md`;
- material PR AI-disclosure compliance over the prior 90 days;
- test and coverage evidence for active code repositories;
- dependency and secret-scanning results at a public-safe level;
- corrected or removed public claims;
- open critical issues and remediation status;
- accessibility, privacy, recourse, and human-impact evidence;
- external validation progress.

## Success-criteria status

| Criterion | Q3 baseline status |
|---|---|
| Top 10 have governance + proof + decision log | Not met |
| Material PRs in prior 90 days have AI disclosure | Not met; one confirmed gap |
| P.A.I.H.I. score at least 70% across top repos | Not established under a conformance audit |
| Zero unpatched critical production dependencies | Unverified |
| Founder approval recorded per material change | Partial; visible in several material PRs |
| External audit completed and published | Not met |
| Quarterly report published and verifiable | Proposed in this branch |

## Approval record

**Required before merge:** an attributable Founder comment containing the exact standalone phrase:

> **All Clear for Impact**

No AI system or workflow may generate, infer, or substitute this approval.

---

**Audit execution:** AltmanAI Model 2.0  
**Accountable human authority:** Blake Hunter Altman, Founder & CEO  
**Organization:** AltmanAI by Altman Family Group LLC