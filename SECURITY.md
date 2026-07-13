# AltmanAI Security Policy

AltmanAI treats security, privacy, provenance, and human control as product requirements. This policy applies across the AltmanAI GitHub organization unless a repository publishes a stricter approved policy.

## Report vulnerabilities privately

Do **not** open a public issue, pull request, discussion, or social-media post for an unremediated vulnerability.

**Security contact:** [security@altmanai.tech](mailto:security@altmanai.tech)

Use a clear subject such as: `Security report — repository or product name`

Include, when safely available:

- affected product, repository, component, endpoint, model, agent, or workflow;
- vulnerability description and likely impact;
- minimal reproduction steps or a safe proof of concept;
- affected version, branch, environment, account type, browser, or device;
- logs, screenshots, request/response examples, or relevant code with secrets and personal data removed;
- whether real user data, credentials, production systems, or third-party services may be affected; and
- your preferred contact method and any coordinated-disclosure constraints.

Never send passwords, API keys, private keys, session tokens, access tokens, or unnecessary personal data. If a credential appears exposed, redact it and describe where it was found.

## Scope

This policy covers public repositories in the AltmanAI GitHub organization and the AltmanAI products or services those repositories support, including DailyPilot and organization-level AI, governance, developer, and accountability infrastructure.

Examples of relevant reports include:

- authentication, authorization, session, or account-isolation failures;
- exposed credentials, secrets, private keys, or sensitive configuration;
- injection, code execution, path traversal, insecure deserialization, or dependency compromise;
- personal, customer, financial, legal, or confidential-data exposure;
- cross-user or cross-tenant access;
- supply-chain, build, release, package, or artifact integrity failures;
- prompt injection that causes unauthorized tool use, data disclosure, scope expansion, or policy bypass;
- AI-agent privilege escalation, unsafe external actions, hidden persistence, or ineffective human-confirmation controls;
- material provenance, logging, rollback, or approval-boundary failures; and
- vulnerabilities in public APIs, integrations, web applications, or deployment infrastructure controlled by AltmanAI.

A public repository may contain demonstrations, reference implementations, archived work, or non-production code. Report genuine security concerns, but do not assume public visibility means a component is currently deployed.

## Research boundaries

Good-faith security research is welcome when it minimizes harm.

Please:

- test only accounts, data, and systems you own or are explicitly authorized to use;
- stop when you encounter personal data, confidential information, credentials, or evidence of cross-user access;
- use the minimum access necessary to demonstrate the issue;
- avoid persistence, destructive changes, data modification, or data exfiltration;
- avoid denial-of-service, resource exhaustion, spam, social engineering, phishing, physical-security testing, or attacks against employees, users, vendors, or partners;
- do not introduce malware or attempt to establish long-term access;
- do not publicly disclose exploitable details before AltmanAI has had a reasonable opportunity to investigate and coordinate remediation; and
- follow applicable law and third-party terms.

If testing could affect production availability, real users, money movement, sensitive records, or external services, obtain written authorization first.

## What happens after a report

AltmanAI will make a good-faith effort to:

1. acknowledge a complete report;
2. assess scope, severity, exploitability, and affected systems;
3. request clarification or additional evidence where necessary;
4. contain and remediate verified issues according to risk and available resources;
5. coordinate disclosure timing where appropriate; and
6. preserve an internal or public record proportionate to the incident.

Response and remediation time vary by complexity, impact, dependencies, and whether third parties are involved. Submission does not guarantee a bounty, compensation, public credit, employment, partnership, or other relationship.

## Safe-harbor intent

AltmanAI does not intend to pursue action against researchers who act in good faith, remain within this policy, avoid harm, respect privacy, and promptly report verified issues. This statement is not legal advice, does not bind third parties, and does not authorize activity prohibited by law or by systems AltmanAI does not control.

## Public handling restrictions

Do not place the following in public issues, pull requests, commits, discussions, examples, logs, screenshots, or test fixtures:

- passwords, tokens, credentials, private keys, or session material;
- customer, employee, applicant, or private-user data;
- private financial, legal, health, identity, or account information;
- confidential agreements, proprietary source material, or restricted prompts;
- production database contents or private infrastructure details; or
- exploit details that create unnecessary risk before remediation.

## AI-system incidents

Suspected unauthorized, deceptive, unsafe, or insecure AI behavior should be reported through the same private channel. Include the model or agent identity if known, the prompt or triggering content, available tools and permissions, observed actions, logs, expected behavior, and whether the system affected external services or people.

See [`AI_SYSTEMS_POLICY.md`](AI_SYSTEMS_POLICY.md) for organization-wide controls covering tool-using systems, autonomy, evaluation, human confirmation, rollback, and incident response.

---

© 2026 Altman Family Group LLC. All rights reserved.
