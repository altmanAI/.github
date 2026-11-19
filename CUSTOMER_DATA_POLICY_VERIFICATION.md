# Customer Data Protection Policy — Verification & Qualification Register

**Policy:** [AAI-GOV-DATA-001](CUSTOMER_DATA_PROTECTION_AND_AI_TRAINING_POLICY.md)  
**Prepared:** November 19, 2026  
**Owner:** Blake Hunter Altman, Founder & CEO  
**Status:** Qualification plan only. **No production data-flow inspection, vendor contract audit, security test, or independent assurance has been completed by this document.**

## Evidence classifications

| Status | Meaning |
|---|---|
| NOT ASSESSED | No current evidence collected or validated |
| GAP IDENTIFIED | Existing fact conflicts with intended policy, remediation required |
| IMPLEMENTED / UNTESTED | Claimed control exists but results not reproduced |
| TESTED / EVIDENCED | Dated reproducible test and scope recorded |
| INDEPENDENTLY REVIEWED | Qualified reviewer, scope and evidence recorded |

**Do not equate approval, 99.99% enthusiasm, or a public commit with compliance.**

## Mandatory qualification questions and evidence required

| ID | Question to prove before a product makes an unqualified claim | Required private evidence / public-safe outcome | Current status |
|---|---|---|---|
| Q01 | Which real products and environments process customer content? | Signed asset, endpoint, environment and owner inventory | NOT ASSESSED |
| Q02 | What customer data categories enter each service or agent? | Collection inventory and sample redacted schema | NOT ASSESSED |
| Q03 | On what lawful basis, contract and notice is each category processed? | Counsel-reviewed basis and exact notice/version | NOT ASSESSED |
| Q04 | Are meeting participants lawfully informed and authorized? | Notice/consent mechanism, regional legal analysis, test | NOT ASSESSED |
| Q05 | Can any customer content enter fine-tuning, training or model-improvement pipelines? | End-to-end lineage review, disabled ingestion routes and tests | NOT ASSESSED |
| Q06 | Are provider training/improvement options configured and contractually restricted? | Dated DPA/terms, console screenshots with secrets redacted, vendor ID | NOT ASSESSED |
| Q07 | Are embeddings, RAG stores, logs and cached AI outputs covered by retention/access controls? | Data-flow graph, TTL, ACL checks, deletion test | NOT ASSESSED |
| Q08 | Is every subprocessor documented with lawful sharing and regional transfer treatment? | Vendor/subprocessor inventory and review date | NOT ASSESSED |
| Q09 | Can users reliably get access, export, correction or deletion as promised? | Support process, identity checks, timed end-to-end test | NOT ASSESSED |
| Q10 | Are backups, legal holds and processor deletion limitations truthfully disclosed? | Retention schedule and restoration/deletion evidence | NOT ASSESSED |
| Q11 | Are tenant boundaries and role-based privileges enforced outside the model prompt? | Code/config inspection, cross-tenant test, IAM evidence | NOT ASSESSED |
| Q12 | Can AI tools cause actions without authenticated, action-specific approval? | Negative tests on sends, writes, purchases, merges and tool calls | NOT ASSESSED |
| Q13 | Does prompt injection in a transcript or webpage cause unauthorized disclosure? | Adversarial evaluation set, redacted results, remediation | NOT ASSESSED |
| Q14 | Can sensitive content leak through public logs, errors, traces, evals or GitHub artifacts? | Data-loss scan, log-sampling results, repo secret scan | NOT ASSESSED |
| Q15 | Are privacy incidents triaged, notified when legally required, and recoverable? | Incident playbook, tabletop record, owners, escalation times | NOT ASSESSED |
| Q16 | Can an administrator secretly override the no-training rule? | Technical gate, change approval control, settings audit | NOT ASSESSED |
| Q17 | Are children and high-stakes scenarios appropriately restricted and reviewed? | Age and use-case assessment, legal review and test | NOT ASSESSED |
| Q18 | Do DailyPilot's public privacy claims reflect actual production behavior? | Feature-to-claim evidence; compare docs/account/privacy.mdx | NOT ASSESSED |
| Q19 | Are the product's current model, SDK, vendor, region and price/version claims evidenced? | Model/vendor register and change record | NOT ASSESSED |
| Q20 | Is there an independently reproducible audit for release claims? | Dated test run/commit and reviewer or external report | NOT ASSESSED |

## Publicly identified prior claims requiring reconciliation

- [DailyPilot privacy documentation](https://github.com/altmanAI/docs/blob/main/account/privacy.mdx) makes specific non-training, non-sharing, control and deletion assurances. They are **public statements**, not evidence from a live production audit.
- [AltmanAI AI Systems Policy](AI_SYSTEMS_POLICY.md) requires bounded authority, provenance and evaluation.
- [Release Governance](RELEASE_GOVERNANCE.md) blocks release if privacy/legal controls are unresolved.
- The July 2026 [Credibility Scorecard](CREDIBILITY_SCORECARD.md) itself flags inconsistent repository-level proof/enforcement; it is a historical baseline, not a current verified score.
- [Canon Charter](https://github.com/altmanAI/canon-charter-v1) is a historical integrity-bound artifact; do not silently rewrite it.

## Go / no-go rule for any actual customer-data integration

**GO** only with a named product owner; mapped purposes, data and recipients; valid legal/notice basis; verified vendor no-training handling; minimum API scopes; tested human confirmation; documented retention/deletion; access tests; incident response; rollback and explicit founder or delegated decision.

**NO-GO** if third-party model-training restrictions cannot be verified, if user notice is missing, if authorization can be bypassed, if sensitive data leaks to public fixtures, or if a critical legal/security requirement remains unresolved.

**Do not enter passwords, API keys, contracts with personal data, raw customer records or vulnerability exploits into this public register.** Keep evidence in an access-controlled company system; list only sanitized result links and dates in public updates.

## 30/60/90-day evidence milestones (proposed, not completed)

- **30 days:** complete asset/data/vender inventory, reconcile existing public claims and product notices; identify blockers.
- **60 days:** implement or disable nonconforming data flows; complete vendor contractual checks and automated permission/retention/training-isolation tests.
- **90 days:** independent or qualified privacy review, incident exercise, system-card updates and a truthful public compliance-status summary. Escalate failures; do not launch affected processing on timeline alone.

**Acceptance metrics (targets, NOT measured results):** 100% inventoried customer-content data flows, 100% customer-data vendors with reviewed terms, 100% consequential write-action tests requiring authorization, zero known customer-content model-training routes, and zero unresolved critical data-handling defects at launch.

**P.A.I.H.I.** Proof: reproduce tests; Alignment: match purpose; Integrity: publish gaps; Humanity: preserve privacy, agency and recourse; Impact: measure useful outcomes and harms.

© 2026 Altman Family Group, LLC. All rights reserved.
