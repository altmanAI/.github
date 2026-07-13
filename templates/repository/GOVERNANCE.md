# Repository Governance

> Replace every bracketed field before adoption. Delete guidance comments after review.

## Repository identity

- **Repository:** `[owner/repository]`
- **Status:** `[working | reference | foundation | experimental | historical | planned]`
- **Strategic objective:** `[link to altmanai-masterplan objective, issue, RFC or master-ledger record]`
- **Accountable owner:** Blake Hunter Altman, Founder & CEO
- **Maintainers:** `[names or GitHub handles]`
- **Last reviewed:** `[YYYY-MM-DD]`

## Purpose and authority boundary

This repository exists to `[state the authorized problem and intended users]`.

It does not authorize maintainers, contributors or AI systems to make company-wide legal, financial, employment, partnership, security-exception or public-positioning commitments unless a separately approved record grants that authority.

## Decision classes

| Class | Examples | Minimum approval |
|---|---|---|
| Routine | Typos, link fixes, formatting, low-risk maintenance | Maintainer review and required checks |
| Material | Features, public claims, architecture, data handling, dependencies, releases | Evidence, tests, risk review and authorized human approval |
| Security-sensitive | Authentication, authorization, secrets, cryptography, permissions, incident controls | Security review and accountable maintainer approval; private handling where necessary |
| Governance-critical | This file, security policy, contribution rules, canonical records, authority model | Founder approval with `All Clear for Impact` before merge |
| Regulated/high-stakes | Legal rights, health, employment, credit, finance, safety or government decisions | Appropriate specialist review plus Founder authorization |

When classification is uncertain, use the higher class.

## Path and change controls

| Path or change type | Required review |
|---|---|
| `GOVERNANCE.md`, `SECURITY.md`, `CONTRIBUTING.md` | Governance-critical |
| `/docs`, public profile or product claims | Material; Founder approval when positioning or canonical policy changes |
| Release, version or package publication | Material; release evidence and rollback plan required |
| Dependency or workflow changes | Material or security-sensitive according to risk |
| Credentials, private data or exploitable findings | Never publish; follow `SECURITY.md` |

## Required proposal record

Material changes must identify:

1. authorized objective and related issue or decision;
2. scope and non-goals;
3. evidence, tests or validation;
4. limitations and uncertainty;
5. security, privacy, accessibility and human-impact risks;
6. AI-assistance disclosure;
7. rollback or correction plan;
8. accountable human approver.

## P.A.I.H.I. review

- **Proof:** What evidence supports the change and what remains unverified?
- **Alignment:** Which approved objective does it serve?
- **Integrity:** Are status, limitations, uncertainty and assistance disclosed accurately?
- **Humanity:** Does it preserve human control, dignity, privacy, accessibility, safety and recourse?
- **Impact:** What measurable outcome should result and how will it be observed?

## AI-assistance disclosure

Material AI assistance must be disclosed in the pull request:

> **AI Assistance:** `[system name]` assisted with `[research | drafting | code | tests | review | documentation | other]`. Verified by `[human name]` on `[YYYY-MM-DD]`. Known limitations: `[limitations]`.

AI systems do not independently approve or merge material changes.

## Founder approval

Governance-critical changes require an attributable Founder comment containing the exact standalone phrase:

> **All Clear for Impact**

Approval does not waive evidence, tests, security, privacy, legal, licensing or correction obligations.

## Rollback criteria

A change must be rolled back, disabled or corrected when:

- it creates a critical security or privacy risk;
- a material public claim proves unsupported;
- required evidence or approval was absent;
- production behavior materially differs from the approved scope;
- user harm, loss of control or significant accessibility failure is observed;
- a dependency or external service becomes unsafe or unavailable.

The rollback record must link the original decision and explain impact, containment and follow-up.

## Incident escalation

1. Stop or contain the affected behavior when safe.
2. Preserve logs and evidence without exposing secrets or personal data.
3. Notify the accountable maintainer and Founder.
4. Use the private security channel for exploitable details.
5. Record the public-safe correction or incident summary when disclosure is appropriate.
6. Update `PROOF.md`, `DECISION_LOG.md`, changelog and affected claims.

## Amendments

Changes to this document are governance-critical and require a dedicated pull request, AI-assistance disclosure, evidence, and explicit Founder approval.
