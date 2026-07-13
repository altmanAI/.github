# AltmanAI AI Systems Policy

## Human authority, controlled autonomy, and verifiable operation

This policy establishes the default requirements for AI models, agents, assistants, autonomous workflows, tool-using systems, and AI-assisted development operated or represented by AltmanAI.

It applies across the AltmanAI GitHub organization unless a repository publishes a stricter approved policy. It is designed for current systems and for future systems with materially greater capability, autonomy, persistence, multimodality, or real-world access.

AltmanAI does **not** claim to have created artificial general intelligence or superintelligence. This policy is a readiness framework for increasingly capable systems.

## 1. Governing rule

> **Human authorization → AI execution → Proof-of-Impact validation**

AI may accelerate work. It does not independently acquire corporate authority, ownership, accountability, or permission to expand its own scope.

The accountable human remains responsible for:

- defining the objective;
- determining the permitted scope and tools;
- reviewing material outputs and actions;
- escalating uncertainty or risk;
- stopping or reversing unsafe activity where possible; and
- preserving an appropriate decision and evidence record.

## 2. Core requirements

Every material AI system should be designed and operated according to these requirements:

1. **Explicit purpose** — The system has a defined objective, intended users, permitted uses, and meaningful non-goals.
2. **Bounded authority** — Permissions, tools, data access, spending, communications, and external actions are limited to what the objective requires.
3. **Human accountability** — A named human owner remains accountable for deployment, monitoring, and material decisions.
4. **Traceability** — Important prompts, inputs, outputs, tool calls, approvals, changes, and incidents are logged or otherwise reconstructable where lawful and proportionate.
5. **Evidence-based validation** — Claims and outputs are tested against appropriate sources, artifacts, evaluations, or human review.
6. **Security and privacy** — Credentials, personal data, proprietary information, and system boundaries are protected through least privilege and data minimization.
7. **Accurate capability** — The system is not represented as more reliable, autonomous, intelligent, safe, or production-ready than evidence supports.
8. **Reversibility** — Consequential changes use staged release, rollback, revocation, or containment mechanisms wherever technically feasible.
9. **Escalation** — The system must defer, refuse, or request qualified review when evidence, authority, or safety controls are insufficient.
10. **Human recourse** — People affected by meaningful system outputs should have a practical way to question, correct, appeal, or override them when appropriate.

## 3. Autonomy classes

AltmanAI classifies AI-enabled workflows by the practical authority they exercise.

| Class | Description | Minimum control |
|---|---|---|
| **A0 — Advisory** | Produces suggestions, drafts, classifications, or analysis without taking external action | Human reviews before use |
| **A1 — Assisted execution** | Performs bounded actions after specific human instruction | Scoped permissions, logs, and post-action review |
| **A2 — Supervised autonomy** | Executes a defined multi-step workflow within pre-approved boundaries | Approval gates for consequential actions, monitoring, limits, and rollback |
| **A3 — High-impact autonomy** | Can materially affect users, finances, production systems, legal rights, public communications, or sensitive data | Specialized risk review, explicit accountable-human approval, continuous monitoring, incident plan, and independent validation where appropriate |
| **A4 — Frontier or open-ended autonomy** | Exhibits broad, persistent, self-directed, or difficult-to-predict operation across tools or environments | Not authorized for deployment without a dedicated governance decision, capability evaluation, containment plan, and approval proportionate to the risk |

When classification is uncertain, use the higher class.

## 4. Consequential actions requiring human confirmation

Unless an approved system-specific policy states otherwise, AI systems must not independently perform the following without accountable-human confirmation:

- merge or publish governance-critical changes;
- deploy production code or alter production infrastructure;
- rotate, disclose, create, or materially change credentials and access controls;
- send authoritative public, legal, financial, employment, partnership, or investor communications;
- enter contracts, accept terms, make purchases, transfer funds, or commit company resources;
- access or disclose sensitive personal, customer, employee, applicant, financial, health, legal, or identity data beyond an approved workflow;
- delete, overwrite, or irreversibly transform material records;
- make high-stakes decisions affecting legal rights, employment, credit, finance, health, safety, or government access;
- represent an unverified output as fact, certification, audit result, legal conclusion, or approved company position; or
- expand its own permissions, persistence, scope, or external connectivity.

## 5. Prohibited uses

AltmanAI systems may not be intentionally designed or operated to:

- manipulate people through deception, coercion, hidden behavioral targeting, or exploitation of vulnerability;
- impersonate a person or organization without clear authorization and appropriate disclosure;
- fabricate evidence, credentials, partnerships, adoption, funding, performance, testing, citations, or approvals;
- conceal material AI involvement where disclosure is required;
- bypass security controls, authorization boundaries, rate limits, or contractual restrictions;
- retain or reuse sensitive data beyond the approved purpose;
- conduct unauthorized surveillance, credential theft, data exfiltration, malware activity, or destructive operations;
- autonomously retaliate against, threaten, harass, discriminate against, or profile individuals in ways inconsistent with law and human dignity; or
- prevent meaningful human review of consequential decisions.

## 6. Model, data, and tool provenance

Material systems should document, as appropriate:

- model or provider identity and version;
- deployment date and environment;
- system prompts, policies, or configuration relevant to behavior;
- tools, APIs, repositories, databases, and external services available to the system;
- training, fine-tuning, retrieval, or evaluation data provenance where known and lawful to disclose;
- important licensing, privacy, security, geographic, or contractual constraints;
- known capability boundaries and failure modes; and
- the human owner and approval record.

AltmanAI-controlled records currently use **AltmanAI Model 2.0** as the authorized AI development and execution partner identity label. Other contributors must identify the actual system they used.

## 7. Evaluation gates

Before a material AI system is represented as production-ready, the responsible team should evaluate the risks relevant to its use, which may include:

- task accuracy and factuality;
- calibration and uncertainty communication;
- prompt-injection and indirect-injection resistance;
- unsafe tool selection or parameter use;
- privilege escalation and permission boundary adherence;
- sensitive-data leakage and memorization;
- deceptive, manipulative, or sycophantic behavior;
- harmful bias, accessibility failures, and disparate impact;
- recovery from malformed, adversarial, or ambiguous inputs;
- reliability under latency, outage, provider, or dependency failure;
- rollback, revocation, and incident containment;
- human comprehension of the system’s role and limitations; and
- effectiveness of appeal, correction, or override paths.

Evaluation evidence should be versioned and connected to the release or decision it supports. Passing one evaluation does not establish permanent safety or reliability.

## 8. Security controls for tool-using agents

Tool-using systems should use:

- least-privilege credentials and narrowly scoped tokens;
- environment separation between development, testing, and production;
- allowlists for sensitive tools, destinations, repositories, and data stores;
- explicit confirmation for destructive, external, financial, or public actions;
- secret scanning and redaction;
- input and retrieved-content treatment that assumes untrusted instructions may be present;
- rate, cost, time, recursion, and action-count limits;
- tamper-resistant or reviewable logs appropriate to the risk;
- kill switches, token revocation, rollback, and isolation procedures; and
- dependency and supply-chain review.

No model output, webpage, document, email, issue, comment, retrieval result, or tool response should automatically be treated as trusted instructions merely because the system can read it.

## 9. Human review standard

Human review must be meaningful rather than ceremonial. Reviewers should have sufficient context, time, authority, and competence to evaluate the material risks.

For consequential work, the reviewer should confirm:

- the objective and scope are authorized;
- outputs are supported by appropriate evidence;
- important limitations and uncertainty are visible;
- sensitive data and permissions were handled correctly;
- the system did not silently expand the task;
- downstream effects and affected stakeholders were considered;
- rollback or correction remains possible where appropriate; and
- the final record accurately distinguishes human and AI contributions.

## 10. Incident response

Suspected harmful, unauthorized, deceptive, or insecure AI behavior should be treated as an operational incident.

The response should, as appropriate:

1. stop or isolate the affected workflow;
2. revoke or narrow credentials and tool access;
3. preserve relevant logs, prompts, outputs, approvals, and system state;
4. identify affected users, systems, repositories, and data;
5. correct or retract inaccurate public claims or outputs;
6. notify responsible stakeholders through approved channels;
7. remediate the root cause and test the fix;
8. document residual risk and follow-up actions; and
9. preserve a proportionate incident or Master Ledger record.

Security vulnerabilities must be reported through `SECURITY.md`, not a public issue.

## 11. Deployment and change management

Material AI-system changes should use version control and a reviewable release process. Changes affecting models, prompts, tools, permissions, data sources, policies, autonomy, evaluations, or high-impact behavior should state:

- what changed;
- why it changed;
- what evidence supports the change;
- what risks or regressions are possible;
- how the change was tested;
- how it can be rolled back; and
- who authorized release.

Silent capability expansion is not an acceptable deployment practice.

## 12. P.A.I.H.I. review

Material AI work should answer:

- **Proof:** What evidence supports the system’s behavior and claims?
- **Alignment:** Is the system operating within the authorized purpose and boundaries?
- **Integrity:** Are uncertainty, limitations, assistance, incentives, and incidents represented honestly?
- **Humanity:** Does the system preserve agency, dignity, privacy, accessibility, safety, and recourse?
- **Impact:** What useful outcome occurred, and what unintended effects were observed?

## 13. Exceptions and amendments

Exceptions require a documented rationale, risk analysis, compensating controls, expiration or review date where appropriate, and approval matching the decision class in `GOVERNANCE.md`.

Changes to this policy are governance-critical and require a dedicated pull request, material AI-assistance disclosure, and explicit Founder approval before merge.

The authorization phrase is:

> **All Clear for Impact**

Approval does not waive applicable law, contracts, security obligations, privacy rights, licensing terms, testing, or specialized review.

---

© 2026 Altman Family Group LLC. All rights reserved.
