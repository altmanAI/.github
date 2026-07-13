# AltmanAI Organization Governance & Standards

### Humanity leads. Intelligence follows.

This repository is the organization-level governance, trust, documentation, and community-health hub for **AltmanAI**, by Altman Family Group LLC.

It defines the default operating standards applied across AltmanAI repositories unless a repository publishes a more specific policy. Its purpose is straightforward: make human accountability, AI-assisted work, contribution expectations, security reporting, and public claims easier to inspect.

## What this repository controls

| Area | Organization-level standard |
|---|---|
| **Public identity** | The organization profile and approved company positioning. |
| **Governance** | Decision authority, review paths, approval gates, and source-of-truth rules. |
| **Contributions** | How creators propose, document, disclose, and validate changes. |
| **Security** | Responsible disclosure expectations and prohibited handling of secrets or private data. |
| **Community health** | Default issue templates, pull request requirements, conduct, and support routes. |
| **AI transparency** | Disclosure and human-review requirements for materially AI-assisted work. |

## Operating model: founder-led human accountability

AltmanAI uses a **founder-led human accountability** model.

- **Blake Hunter Altman, Founder & CEO**, holds final accountable authority for organization-level governance, public positioning, and material approval decisions.
- Maintainers and contributors may research, propose, implement, test, and review changes within their authorized scope.
- AI systems may assist with analysis, drafting, code, testing, documentation, and workflow execution, but they do not hold corporate authority and may not independently approve, merge, publish, contract, or represent AltmanAI.
- Significant public, governance, security, or organization-standard changes require explicit human approval before they become authoritative.

The approval phrase used for governance-level authorization is:

> **All Clear for Impact**

This is an approval control, not a substitute for evidence, testing, security review, or legal judgment where those are required.

## P.A.I.H.I. in practice

AltmanAI's P.A.I.H.I. framework turns its human-first philosophy into reviewable operating questions:

| Dimension | Review question |
|---|---|
| **Proof** | What evidence, artifact, test, or source supports this change? |
| **Alignment** | Does it match the authorized objective, repository scope, and company mission? |
| **Integrity** | Are capabilities, limitations, risks, and AI assistance represented honestly? |
| **Humanity** | Does it preserve human agency, dignity, privacy, safety, and meaningful control? |
| **Impact** | What useful outcome does it create, and how will that outcome be reviewed? |

Signature process:

> **Human authorization → AI execution → Proof-of-Impact validation**

## Canonical documentation

| File | Purpose |
|---|---|
| [`profile/README.md`](profile/README.md) | Public face of the AltmanAI GitHub organization |
| [`GOVERNANCE.md`](GOVERNANCE.md) | Authority, decision classes, review process, and approval model |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Contributor paths, quality standards, and AI-assisted-work disclosure |
| [`SECURITY.md`](SECURITY.md) | Responsible vulnerability disclosure and sensitive-data rules |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Community conduct standard |
| [`SUPPORT.md`](SUPPORT.md) | Support and contact routes |
| [`.github/pull_request_template.md`](.github/pull_request_template.md) | Pull request evidence, risk, review, and approval checklist |
| [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE/) | Structured bug, feature, research, and documentation proposals |
| [`GITHUB_AUDIT.md`](GITHUB_AUDIT.md) | Account-wide repository audit and prioritization record |
| [`REPO_SCORECARD.md`](REPO_SCORECARD.md) | Directional portfolio scorecard for repository stewardship |

## Change lifecycle

1. **Define the problem.** State the user, business, research, governance, or security need.
2. **Establish evidence.** Link relevant issues, sources, tests, artifacts, or existing decisions.
3. **Propose a bounded change.** Keep scope clear and distinguish live capability from future intent.
4. **Disclose AI assistance.** Identify material AI involvement in the pull request.
5. **Review risk and impact.** Apply P.A.I.H.I., security, privacy, and repository-specific checks.
6. **Obtain human authorization.** Secure the approval required for the change class.
7. **Preserve the record.** Merge through GitHub so the decision and resulting artifact remain inspectable.

## Source of truth

AltmanAI separates public positioning from verifiable records:

- This repository is the canonical source for organization-level GitHub governance and standards.
- The **[AltmanAI Master Ledger](https://github.com/altmanAI/altmanai-master-ledger)** is the public source for selected records, reusable standards, and Proof-of-Impact artifacts.
- Product repositories remain authoritative for their own code, tests, releases, and repository-specific documentation.
- When documents conflict, the more specific approved record governs unless an explicit organization-level decision supersedes it.

## Trust boundaries

Public repositories must not contain credentials, private keys, customer data, private financial information, confidential business records, proprietary prompts not approved for release, or security-sensitive implementation details.

Public visibility does not automatically grant an open-source license, create a partnership, establish employment, confer equity, or authorize someone to represent AltmanAI. Each repository's license and approved written agreements control.

## Company context

AltmanAI is a Pittsburgh-rooted human-first AI company building practical products and accountability infrastructure for responsible human–AI collaboration.

- **Website:** [altmanai.tech](https://www.altmanai.tech)
- **Public organization profile:** [`profile/README.md`](profile/README.md)
- **Master Ledger:** [altmanAI/altmanai-master-ledger](https://github.com/altmanAI/altmanai-master-ledger)

---

© 2026 Altman Family Group LLC. AltmanAI, DailyPilot, P.A.I.H.I., and related proprietary systems are protected intellectual property. All rights reserved.