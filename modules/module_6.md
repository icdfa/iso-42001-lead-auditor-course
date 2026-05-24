# ISO/IEC 42001 Lead Auditor Training Course: The Complete Guide

## Module 6: Fundamental Audit Concepts and Principles (ISO 19011)

### Learning Objectives
By the end of this module, you will be able to:
1. Understand and apply the seven core principles of auditing as defined by ISO 19011.
2. Clearly differentiate between first-party, second-party, and third-party audits and their purposes.
3. Describe the lifecycle of managing an audit program.
4. Understand the specific roles, responsibilities, and required competencies of a Lead Auditor and audit team members.
5. Explain the critical importance of an evidence-based and risk-based approach to auditing AI systems.

### 6.1 Principles of Auditing: The Auditor's Code
Auditing is not merely a tick-box exercise; it is a professional discipline that relies on a set of fundamental principles. Adherence to these principles is a prerequisite for providing audit conclusions that are relevant, sufficient, and trustworthy. These principles ensure that auditors working independently from one another will reach similar conclusions in similar circumstances. ISO 19011, the international standard for auditing management systems, outlines seven core principles [1].

1. **Integrity:** The foundation of professionalism. Auditors must perform their work ethically, with honesty and responsibility. They must only undertake audit activities if they are competent to do so and must observe and comply with any applicable legal requirements. An auditor must not succumb to pressure to alter findings.
2. **Fair Presentation:** The obligation to report truthfully and accurately. Audit findings, audit conclusions, and audit reports must reflect the audit activities truthfully and accurately. If an auditor encounters significant obstacles (e.g., an auditee refusing to provide records) or if there are unresolved diverging opinions between the audit team and the auditee, these *must* be reported.
3. **Due Professional Care:** The application of diligence and judgment in auditing. Auditors must exercise due care in accordance with the importance of the task they perform and the confidence placed in them by the audit client and other interested parties. This means being thorough, prepared, and analytical.
4. **Confidentiality:** Security of information. Auditors are granted access to highly sensitive information (e.g., proprietary algorithms, trade secrets, sensitive data). Auditors must exercise strict discretion in the use and protection of information acquired in the course of their duties. Audit information must not be used inappropriately for personal gain or in a manner detrimental to the legitimate interests of the auditee.
5. **Independence:** The basis for the impartiality of the audit and objectivity of the audit conclusions. Auditors must be independent of the activity being audited wherever practicable, and must in all cases act in a manner that is free from bias and conflict of interest. (e.g., A consultant who helped build the AIMS cannot be the third-party auditor who certifies it).
6. **Evidence-based Approach:** The rational method for reaching reliable and reproducible audit conclusions in a systematic audit process. Audit evidence must be verifiable. It should generally be based on samples of the information available, since an audit is conducted during a finite period of time and with finite resources. Auditors do not rely on rumors or assumptions; they rely on objective facts.
7. **Risk-based Approach:** An audit approach that considers risks and opportunities. The risk-based approach must substantively influence the planning, conducting, and reporting of audits to ensure that audits are focused on matters that are significant for the audit client and for achieving the audit program objectives. If a specific AI model poses a high risk to human safety, the auditor should spend more time auditing the controls around that model than a low-risk internal chatbot.

### 6.2 Types of Audits
Audits are generally categorized into three types based on the relationship between the auditor and the auditee.

| Audit Type | Also Known As | Description | Primary Purpose |
| :--- | :--- | :--- | :--- |
| **First-Party** | Internal Audit | Conducted by, or on behalf of, the organization itself. | To review management systems, drive internal improvement, and declare conformity prior to external audits. |
| **Second-Party** | Supplier/External Audit | Conducted by parties having an interest in the organization, such as customers or partners. | To evaluate a supplier's capability to meet contractual requirements (e.g., auditing an AI vendor before purchasing their model). |
| **Third-Party** | Certification Audit | Conducted by external, independent auditing organizations (Certification Bodies). | To provide independent certification or registration of conformity to a standard (e.g., issuing an ISO/IEC 42001 certificate). |

### 6.3 Managing an Audit Program
An audit program is a set of one or more audits planned for a specific timeframe and directed towards a specific purpose. Managing an audit program is a PDCA cycle in itself. It involves:
- **Establishing the audit program objectives:** What are we trying to achieve? (e.g., to evaluate the effectiveness of the AIMS across all global offices, to achieve certification).
- **Determining and evaluating audit program risks and opportunities:** What could prevent the audit from being successful? (e.g., lack of competent AI auditors, travel restrictions).
- **Establishing the audit program:** Defining roles, responsibilities, resources, and procedures for the audits.
- **Implementing the audit program:** Scheduling the audits, selecting competent audit teams, and directing the audit activities.
- **Monitoring, reviewing, and improving the audit program:** Are the audits achieving their objectives? Are the auditors performing well?

### 6.4 Roles, Responsibilities, and Competencies
The success of an audit depends heavily on the competence and conduct of the audit team. Auditing an AIMS requires a unique blend of traditional auditing skills and technical AI knowledge.

**The Lead Auditor is responsible for:**
- Managing the entire audit process and representing the audit team.
- Preparing the audit plan and assigning specific tasks to team members based on their expertise.
- Leading the opening and closing meetings.
- Communicating with the auditee management and the audit client.
- Resolving conflicts and reaching conclusions on audit findings.
- Preparing and submitting the final, formal audit report.

**Audit Team Members are responsible for:**
- Planning and carrying out assigned tasks objectively and effectively.
- Collecting and analyzing relevant audit evidence.
- Documenting audit findings clearly.
- Safeguarding the confidentiality of documents and information.

**Competence Requirements:**
To audit ISO/IEC 42001 effectively, the audit team (collectively) must possess knowledge of:
- Audit principles, procedures, and methods (ISO 19011).
- Management system standards (ISO/IEC 42001).
- Organizational context (business management, legal/regulatory frameworks).
- **AI-specific knowledge:** Machine learning concepts, AI lifecycle, AI risk management, data governance, and AI ethics. If the auditors lack deep technical expertise in a specific AI domain, the Lead Auditor may include a **Technical Expert** on the team. The Technical Expert provides knowledge but does not act as an auditor.

### Knowledge Check and Reflection
**Question 1:** Which audit principle requires an auditor to report significant obstacles encountered during the audit, even if it makes the auditee uncomfortable?
A) Confidentiality
B) Fair Presentation
C) Risk-based Approach
D) Independence
*Answer: B*

**Question 2:** An organization wants to achieve formal, globally recognized certification to ISO/IEC 42001. What type of audit must they undergo?
A) First-Party Audit
B) Second-Party Audit
C) Third-Party Audit
D) Internal Audit
*Answer: C*

**Reflection Exercise:** You are a Lead Auditor assembling a team to audit a hospital's AIMS, which includes an AI system that assists in diagnosing diseases from X-rays. You have strong auditing skills but limited medical or AI coding knowledge. Who else should you include on your audit team to ensure due professional care?

### References
[1] ISO. ISO 19011:2018 Guidelines for auditing management systems. https://www.iso.org/standard/70017.html
