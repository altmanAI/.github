# AltmanAI AI System Card

> Use this template for models, agents, AI-assisted features, automated decision workflows, and systems that can invoke tools or affect users. Replace all instructional text before release.

## 1. System identity

- **System name:**
- **Repository or product:**
- **Version:**
- **Lifecycle status:** Proposed / Experimental / Internal / Beta / Production / Deprecated / Archived
- **Accountable human owner:**
- **Technical owner:**
- **Last reviewed:**
- **Next required review:**

## 2. Authorized purpose

### Intended objective

Describe the human-authorized problem this system addresses and the useful outcome it is designed to produce.

### Intended users

Identify users, operators, reviewers, and affected stakeholders.

### Explicit non-goals

State what the system is not designed, authorized, or validated to do.

### Prohibited uses

List disallowed domains, decisions, actions, data uses, or deployment contexts.

## 3. System description

- **Models or providers used:**
- **Prompts, policies, or routing logic:**
- **Tools and external services:**
- **Human inputs and approvals:**
- **Outputs and actions:**
- **Persistence, memory, or state:**
- **Deployment environment:**

Include a data-flow or architecture diagram when the system is material, multi-component, tool-using, or production-facing.

## 4. Capability boundaries

### Supported capabilities

List only capabilities supported by reproducible evidence.

### Unsupported capabilities

Identify functions the system may appear able to perform but is not authorized, reliable, or validated to perform.

### Known limitations

Describe uncertainty, hallucination risk, non-determinism, coverage gaps, language or accessibility limitations, model/provider dependencies, and foreseeable failure modes.

## 5. Human authority and recourse

- **Who defines objectives?**
- **Who can authorize consequential actions?**
- **What requires confirmation before execution?**
- **How can a user challenge, correct, or appeal an output?**
- **How can an operator pause, disable, or roll back the system?**
- **What decisions must never be delegated solely to the AI system?**

Meaningful human control must be operational, not ceremonial. Reviewers must have sufficient information, time, authority, and practical ability to intervene.

## 6. Data governance and privacy

- **Data sources:**
- **Personal or sensitive data involved:**
- **Legal or consent basis where applicable:**
- **Data minimization controls:**
- **Retention and deletion:**
- **Access controls:**
- **Logging and observability:**
- **Training or provider data-use settings:**
- **Cross-border or third-party processing:**

Do not include secrets, credentials, private personal data, or exploit details in a public system card.

## 7. Security and misuse resistance

Address, where applicable:

- least-privilege permissions;
- credential and secret handling;
- prompt injection and indirect prompt injection;
- data exfiltration;
- unsafe or unauthorized tool invocation;
- identity, authentication, and authorization failures;
- dependency and supply-chain risk;
- malicious inputs and adversarial use;
- rate limits, abuse controls, and anomaly detection;
- sandboxing, isolation, and environment boundaries;
- incident response and kill-switch procedures.

## 8. Evaluation record

### Evaluation objectives

Define the claims being tested and why they matter.

### Test sets and scenarios

Document representative, edge-case, adversarial, accessibility, privacy, and failure-recovery tests.

### Baselines and thresholds

State comparison baselines, acceptance thresholds, and release-blocking conditions.

### Results

Provide dated, versioned, reproducible evidence. Distinguish measured results from estimates or qualitative judgment.

### Independent or human review

Identify reviewers, review scope, unresolved disagreements, and any domain-specific expertise required.

## 9. Human-impact review

Consider:

- dignity and respectful treatment;
- autonomy and informed choice;
- accessibility and inclusive use;
- privacy and contextual integrity;
- fairness and disparate impact;
- overreliance, dependency, and deskilling;
- emotional or psychological effects;
- recourse and error correction;
- effects on workers, communities, and vulnerable users.

## 10. P.A.I.H.I. assessment

- **Proof:** What evidence supports the system's claims and release status?
- **Alignment:** How does the system match the authorized objective and AltmanAI mission?
- **Integrity:** What uncertainty, limitations, assistance, conflicts, or unresolved risks are disclosed?
- **Humanity:** How are dignity, agency, privacy, accessibility, safety, and meaningful review preserved?
- **Impact:** What useful outcome occurred or is expected, and how will it be measured?

## 11. Monitoring and change control

- **Operational metrics:**
- **Safety and quality indicators:**
- **Drift detection:**
- **User feedback and complaint channels:**
- **Incident thresholds:**
- **Review cadence:**
- **Material-change triggers:**
- **Rollback procedure:**

A material change to the model, provider, prompt architecture, data flow, permissions, tools, intended use, or risk profile requires renewed review.

## 12. Release decision

- **Decision class:** Routine / Material / Governance-critical / Regulated or high-stakes
- **Release decision:** Approved / Conditionally approved / Rejected / Retired
- **Conditions or restrictions:**
- **Accountable approver:**
- **Approval date:**
- **Authorization record or Master Ledger reference:**
- **Rollback owner:**

### AI assistance disclosure

Identify material AI assistance used to design, implement, test, document, or review this system. Human reviewers remain accountable for verification and release decisions.
