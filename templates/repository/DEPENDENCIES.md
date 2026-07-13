# Dependency and Supply-Chain Record

> Public-safe inventory for major runtime, build, release and security-sensitive dependencies. Do not expose private infrastructure, credentials or exploitable details.

## Repository

- **Repository:** `[owner/repository]`
- **Primary ecosystems:** `[npm | Python | Go | Rust | other]`
- **Dependency owner:** `[maintainer]`
- **Last reviewed:** `[YYYY-MM-DD]`
- **Lockfile present:** `[yes/no/not applicable]`
- **Automated updates:** `[Dependabot/Renovate/other/not configured]`

## Major dependency matrix

| Dependency | Version / constraint | Type | Purpose | Risk level | Update source | Latest review | Notes |
|---|---|---|---|---|---|---|---|
| `[name]` | `[version]` | `[runtime | development | build | action | service]` | `[purpose]` | `[low | medium | high | critical]` | `[registry/release source]` | `[date]` | `[limitations or controls]` |

Risk should consider:

- privilege and data access;
- runtime or release criticality;
- maintainer and project health;
- transitive dependency exposure;
- native code or install scripts;
- network access and telemetry;
- package integrity and provenance;
- known vulnerabilities and patch availability;
- replacement difficulty and blast radius.

## Scan posture

| Control | Tool / provider | Trigger | Last run | Result | Evidence |
|---|---|---|---|---|---|
| Vulnerability scan | `[npm audit / pip-audit / osv-scanner / other]` | `[PR/push/schedule/manual]` | `[date]` | `[summary or unverified]` | `[workflow/report link]` |
| Dependency review | `[GitHub Dependency Review / other]` | `[PR]` | `[date]` | `[summary]` | `[link]` |
| Automated updates | `[Dependabot/Renovate]` | `[schedule]` | `[date]` | `[summary]` | `[link]` |
| Secret scan | `[GitHub native / gitleaks / trufflehog / other]` | `[trigger]` | `[date]` | `[public-safe summary]` | `[link]` |
| Action pinning | `[policy/tool]` | `[trigger]` | `[date]` | `[summary]` | `[link]` |

## Current vulnerability status

- **Critical unresolved:** `[count or unverified]`
- **High unresolved:** `[count or unverified]`
- **Accepted risk records:** `[links or none]`
- **Next required review:** `[date or release trigger]`

Do not state zero vulnerabilities unless the applicable ecosystems and lockfiles were scanned and the evidence is linked.

## GitHub Actions and release dependencies

| Action / service | Reference | Pinning | Permissions | Purpose | Risk / mitigation |
|---|---|---|---|---|---|
| `[action]` | `[tag or SHA]` | `[tag/SHA]` | `[permissions]` | `[purpose]` | `[risk and control]` |

Workflows should use minimum required permissions. Third-party actions should be pinned to a reviewed commit SHA where practical for security-sensitive or release workflows.

## External services

| Service | Data shared | Authentication | Failure mode | Exit / fallback | Owner |
|---|---|---|---|---|---|
| `[service]` | `[data categories]` | `[method]` | `[failure impact]` | `[fallback]` | `[owner]` |

## Exception and risk acceptance

A high or critical dependency risk may be accepted only through a traceable decision record that includes:

- business or technical justification;
- affected versions and scope;
- compensating controls;
- expiration or review date;
- accountable human approver;
- rollback or replacement plan;
- security-sensitive handling where applicable.

Governance-critical or material exceptions require Founder authorization under repository governance.

## Change log

| Date | Change | Reason | Evidence | Approver |
|---|---|---|---|---|
| `[date]` | `[dependency or policy change]` | `[reason]` | `[PR/scan link]` | `[human]` |
