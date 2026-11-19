# ALTMANAI 3.0
# Customer Data Protection & AI Model Training Policy — Master Copy

**Policy ID:** AAI-GOV-DATA-001  
**Version:** 1.0.0 (proposed official text)  
**Entity:** AltmanAI by Altman Family Group, LLC — Pennsylvania, United States  
**Accountable executive:** Blake Hunter Altman, Founder & Chief Executive Officer  
**Founder authorization:** “ALL CLEAR FOR IMPACT” for adoption, implementation work, and public release requested on November 19, 2026  
**Governance status:** Founder-authorized directive; GitHub canonical adoption requires review/merge of the linked pull request.  
**Operational assurance status:** NOT VERIFIED. This document establishes mandatory expectations; it is not an independent certification that every existing service meets them.  
**Review interval:** At least annually and after a material data-flow, vendor, legal, incident, or model change.

> **HUMANITY LEADS. INTELLIGENCE FOLLOWS. POWER SERVES. TRUST GOVERNS.**

## 1. Executive commitment

AltmanAI will build and operate human-first AI systems that preserve customer control, minimize personal-data processing, and make meaningful AI actions reviewable and correctable. Possession of content is not permission to train on it. Capability is not authorization.

**Strict no-training rule:** AltmanAI **must not use customer communications, customer-provided content, or confidential customer records to train, fine-tune, retrain, distill, or otherwise update general-purpose or customer-independent machine-learning model parameters, whether operated by AltmanAI or a third party.** No employee, account administrator, AI agent, or product default may waive this rule unilaterally. A future policy change requires a new version, explicit authorized executive decision, legal and vendor review, and prospective customer notice/authorization where required; it cannot silently license prior customer data for training.

This is a binding **policy requirement and release condition**, **not** a present-tense assertion that all historical vendors, configurations, products or databases have been independently audited.

## 2. Scope and definitions

Applies to AltmanAI-controlled products and services, development and production operations, agents (including Von where deployed), customer support, authorized personnel, contractors, processors, and third-party integrations when they handle customer information.

**Customer Content** includes meeting audio/video, transcripts, chat, email, files, whiteboards, images, forms, survey results, customer prompts and AI outputs, business records, and material derived from them that remains identifiable, confidential, or linkable to a customer. **Personal Data** means information relating to an identifiable person as defined by applicable law. **Service inference** means processing information transiently or within a customer's authorized context to provide the requested service, without updating shared model weights. **Training** includes fine-tuning, distillation, shared gradient updates, or building datasets to improve customer-independent models. **Retrieval** or **RAG** is not training, but may still create privacy, logging, retention, access, embedding, or vendor exposure.

Respect contractual confidentiality and third-party rights. Customer ownership is not automatically determined by this policy; customers retain their rights, subject to applicable law and agreements. AltmanAI claims only the limited processing rights needed to deliver authorized services.

## 3. Lawful purpose, consent and transparency

1. Establish and record a valid legal basis and contractual scope for each processing activity.
2. Describe data categories, purposes, recipients, sharing, material subprocessors, retention, user rights and data transfers in an accurate product-level privacy notice.
3. Provide lawful notice and consent for recordings, transcripts, meeting participants and external services where required. A host's authorization alone may be insufficient.
4. Prohibit undisclosed secondary uses, sale of personal information, behavioral advertising with private content, or use of customer content for unrelated products unless separately assessed and lawful.
5. Minimize collection and avoid sensitive data unless required for an authorized service with appropriate safeguards. Do not expose customer datasets in public repositories or evaluation examples.
6. If a processing activity cannot be justified and controlled, do not ingest the information.

## 4. Model-training separation — mandatory control

- **No customer-content training** of AltmanAI or external general-purpose/foundation models, including via vendor “improvement” or default training-sharing settings.
- **No silent exceptions** for internal development, contractor research, QA convenience, performance tuning, experimentation, or executive preference.
- Keep **inference, retrieval, evaluation, safety review, analytics, and model training** separately inventoried. Each may process data and must have its own lawful basis and controls. Customer records may be used for narrowly necessary, appropriately protected service evaluation only when authorized and consistent with this policy; they must not enter training pipelines.
- Synthetic, independently licensed, public, or otherwise lawfully usable noncustomer datasets may support model development only after provenance, license, privacy and security review. “De-identified” data is not automatically free of privacy obligations or reidentification risk.
- Ensure providers' contractual terms, subprocessor terms, retention options and account settings match this restriction **before** customer content is sent. If not demonstrable, block transmission or choose a compliant alternative.
- Record evidence of configuration, data-flow blocking, vendor terms, model/version, approval and periodic rechecks.

## 5. Human authorization, AI agents and action control

Apply the existing organization rules in [GOVERNANCE.md](GOVERNANCE.md), [AI_SYSTEMS_POLICY.md](AI_SYSTEMS_POLICY.md), and [RELEASE_GOVERNANCE.md](RELEASE_GOVERNANCE.md).

**Authorized human objective → minimum necessary AI processing → proposed output/action → meaningful human review → explicitly authorized execution → traceable result.**

Default third-party integrations and agent tools to read-only and least privilege. Separate analysis from execution credentials where possible. Require authenticated, action-specific approval for public communications, customer-record changes, production deployment, financial actions, sensitive disclosures, policy changes and other consequential actions. Use two-person review where risk warrants it. Log approver, scope, time, tool, result and failure without unnecessarily reproducing private content. Approval must be revocable; agents must fail closed when access, consent, source integrity or safety controls are uncertain.

“ALL CLEAR FOR IMPACT” records a founder-reviewed decision in the proper governance context. It is **not** an API credential, authentication secret, standalone digital signature or override of law, security review, contract, incident control or customer consent.

## 6. Access, security and separation

Implement proportionate authentication (including MFA for privileged accounts), role-based access, periodic access review, encryption in transit and at rest where appropriate, secret management, environment separation, vendor access controls, audit integrity, vulnerability management and documented incident response.

No agent prompt or separate agent name is sufficient isolation. Enforce permission and tenant boundaries at the application, identity, data and tool levels. Treat retrieved pages, email, transcripts and tool results as untrusted data; prohibit prompt-injection instructions from changing permissions or sending content externally.

Do not upload real customer data to developer demos, test fixtures, public logs, GitHub issues or model evaluation corpora. Use synthetic fixtures and redacted proof wherever feasible.

## 7. Retention, deletion, portability and rights

Maintain a per-product and per-data-type retention schedule with responsible owner, legal/contractual basis, storage location and deletion method. Do not promise immediate destruction of backups or legal-hold records where technically or legally impossible; explain actual timelines and exceptions. When required or offered by contract, provide authenticated access, correction, export, deletion and objection/appeal channels with identity verification and response tracking. Honor valid erasure/deletion instructions across processors as contracts and law require.

Minimize telemetry and embeddings, set log expiration, and document backups, restoration, archive, legal hold and incident evidence. Personal data must not persist solely because an AI feature produced it.

## 8. Children, vulnerable users and high-impact domains

Apply age-appropriate privacy safeguards and legal requirements before processing minors' data. Avoid deploying unreviewed AI decisions in health, employment, education, housing, finance, legal rights or public safety. Require appropriate domain experts, heightened purpose limits, meaningful human review, accessible recourse and incident escalation. Do not infer high-stakes authority from broad customer consent or AI confidence scores.

## 9. Third-party providers, conferencing and MCP

Before a Zoom, SDK, API, MCP server or other third-party integration handles Customer Content, record:
- precise data fields, recipients, transit/storage regions and transfer mechanism;
- API/OAuth permissions and ability to revoke;
- data training and improvement terms for each vendor/subprocessor;
- retention/deletion, logs, embeddings and replay/debugging practices;
- notice and participant permissions where applicable;
- security requirements, breach handling, change notification and contractual controls.

Zoom's own published privacy statements describe Zoom's practices, **not AltmanAI compliance**. No affiliation, sponsorship or partnership with Zoom is implied by compatibility with its developer platform.

## 10. Incidents, correction, complaints and review

Security or privacy incidents require containment, preservation of proportionate evidence, owner assignment, legal notification analysis, timely lawful communications, corrective action and retesting. Do not publish unremediated exploit details or personal information. Private vulnerability reports follow [SECURITY.md](SECURITY.md). Customers must have a practical channel to challenge material incorrect data or unauthorized activity.

Material policy amendments must be versioned and reviewed as governance-critical changes under existing rules; historical signed/minted or hash-bound artifacts remain unchanged and are superseded by linked amendments.

## 11. Public claims and proof requirements

An approved policy is **not** proof of implementation. AltmanAI must not state that a specific product is fully compliant, independently audited, privacy-certified, 99.99% reliable, vendor-approved, trained exclusively on AltmanAI data, or that no customer content was ever processed contrary to this policy without independent supporting evidence.

For each product, publish a truthful status: **not assessed / gap identified / implemented-not-tested / tested-with-evidence / independently reviewed**. Keep sensitive evidence internal and publish only safe summaries and references. A 99.99% confidence expression by the Founder is a **statement of conviction, not a measured assurance metric**.

The release gate, evidence questions and open statuses are in [CUSTOMER_DATA_POLICY_VERIFICATION.md](CUSTOMER_DATA_POLICY_VERIFICATION.md).

## 12. Adoption, precedence and implementation

- This text supplements, rather than silently rewrites, existing AltmanAI governance, security, release, AI-systems and product policies. Applicable law and binding contracts prevail.
- If an existing product privacy notice offers **weaker protections** than this policy, flag the conflict, stop affected data flows when required, and publish an accurate harmonized notice after validation.
- The Founder has authorized the **policy direction and preparation for public adoption** on November 19, 2026. Its canonical GitHub effective version and publication commit are established by the approved merge record.
- Implement through a documented asset/data-flow inventory, vendor review, technical tests, privacy and legal review, and controlled rollout. Unknown or failing controls block compliance claims and implicated processing.
- No policy publication retroactively certifies historical operations. When facts change, amend the policy and correct claims promptly.

### Executive approval and disclosure

**BLAKE HUNTER ALTMAN**  
Founder & Chief Executive Officer  
**ALTMANAI** — By Altman Family Group, LLC  
Pennsylvania | United States of America

**Founder-stated approval:** ALL CLEAR FOR IMPACT (November 19, 2026).  
**Release record:** Link the eventual merged PR and commit here; quoted approval alone does not constitute verified GitHub signature.  
**AI assistance:** GPT-6 materially assisted research synthesis and drafting. The human Founder retains corporate approval authority. Historical AltmanAI records referencing *AltmanAI Model 2.0* are not silently renamed by this AltmanAI 3.0 policy initiative.

© 2026 Altman Family Group, LLC. All rights reserved, subject to applicable third-party rights and repository licenses.
