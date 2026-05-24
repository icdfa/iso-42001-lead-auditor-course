# ISO/IEC 42001 Lead Auditor Training Course: The Complete Guide

## Module 8: Conducting an ISO/IEC 42001 Audit

### Learning Objectives
By the end of this module, you will be able to:
1. Conduct an effective, professional opening meeting that sets the right tone.
2. Apply various methods for gathering robust audit evidence (interviews, observation, document review).
3. Evaluate audit evidence objectively against ISO/IEC 42001 criteria.
4. Generate accurate and objective audit findings (Conformities, Nonconformities, Opportunities for Improvement).
5. Identify, structure, and write clear, undeniable nonconformity reports using the PLO structure.

### 8.1 Conducting the Opening Meeting: Setting the Stage
The on-site audit (Stage 2) officially begins with the opening meeting. This is a formal meeting chaired by the Lead Auditor and attended by the auditee's management and, where appropriate, those responsible for the functions or processes to be audited. First impressions matter; the Lead Auditor must project professionalism, competence, and a collaborative (yet independent) attitude.

**The primary purposes of the opening meeting are to:**
- Introduce the audit team and outline their specific roles.
- Confirm the agreement of all parties to the audit plan (including objectives, scope, and criteria). This ensures everyone is on the same page and prevents "scope creep."
- Ensure that all planned audit activities can be performed (e.g., confirming access to secure server rooms or specific personnel).
- Provide a short summary of how the audit activities will be undertaken (explaining the sampling process).
- Confirm communication channels between the audit team and the auditee (e.g., end-of-day debriefs).
- Confirm matters relating to confidentiality, information security, and occupational health and safety.
- Confirm the time and location for the closing meeting.

### 8.2 Gathering Audit Evidence: The Auditor's Investigation
During the audit, information relevant to the audit objectives, scope, and criteria must be collected by appropriate sampling and must be verified. Only verifiable information may be accepted as audit evidence. Hearsay or assumptions are not evidence.

Auditors use three primary methods to gather evidence, often triangulating them to confirm a finding:

#### 8.2.1 Interviews
Interviews are a vital source of information. Auditors should interview personnel from various levels--from top management (Clause 5) to frontline data scientists and operational staff.
- **Best Practices:**
 - Put the interviewee at ease; an audit is an investigation, not an interrogation.
 - Ask open-ended questions (who, what, where, when, why, how) to encourage detailed responses. (e.g., "Can you explain how you select training data?" rather than "Do you select training data?").
 - Listen actively and do not interrupt. Allow silence; people often fill it with valuable information.
 - Verify the information obtained during interviews against other sources (e.g., if a developer says they run bias checks, ask to see the report).

#### 8.2.2 Observation
Observation involves watching a process or procedure being performed in real-time. In the context of an AIMS, this might involve observing how data scientists label data, how an AI model is deployed to the production environment, or how the system's real-time performance dashboard is monitored by operations staff.
- **Best Practices:** Ensure the observation is conducted under normal operating conditions. Note any deviations from documented procedures. Ask the person to explain what they are doing as they do it.

#### 8.2.3 Review of Documented Information
This involves examining documents (policies, procedures, manuals) and records (evidence of activities performed, such as risk assessment reports, training logs, incident reports, or model performance metrics).
- **Best Practices:** Use the sampling plan to select records. Check for completeness, accuracy, and appropriate authorization (e.g., did the risk owner actually sign off on accepting the residual risk?). For ISO/IEC 42001, pay special attention to the Statement of Applicability and records of AI impact assessments [1].

### 8.3 Evaluating Evidence and Generating Audit Findings
Once evidence is gathered, it must be evaluated against the audit criteria to determine the audit findings. Audit findings can indicate conformity or nonconformity.

**The evaluation process involves:**
1. Comparing the collected objective evidence against the specific requirements of ISO/IEC 42001, the organization's own AIMS policies, or applicable laws.
2. Determining if the requirement has been met (**Conformity**) or not met (**Nonconformity**).
3. Identifying **Opportunities for Improvement (OFI)**. An OFI is issued when the system currently meets the requirement, but the auditor identifies a risk that it might fail in the future, or sees a way the process could be made more efficient or robust. (Note: Auditors must be careful not to provide consulting advice when issuing OFIs).

### 8.4 Identifying and Writing Nonconformities
A nonconformity is the non-fulfillment of a requirement. When a nonconformity is identified, the auditor must document it clearly, accurately, and undeniably so that the auditee understands the exact issue and can take appropriate corrective action.

**A well-written nonconformity report must include three elements (often referred to as the PLO or Requirement-Evidence-Finding structure):**

1. **The Requirement (The "Rule"):** The specific clause of ISO/IEC 42001, the internal policy, or the legal requirement that has not been met. You must quote the exact requirement.
2. **The Objective Evidence (The "Facts"):** The specific facts that demonstrate the requirement was not met. This must be detailed enough that another auditor could follow the trail. Include specific document names, dates, observed actions, or interview statements.
3. **The Finding (The "Statement of Nonconformity"):** A clear, concise statement describing the nature of the nonconformity--the gap between the Requirement and the Evidence.

**Example of a Poorly Written Nonconformity:**
- *Finding:* The company isn't training its staff on AI ethics properly.

**Example of a Well-Written Nonconformity:**
- **Requirement:** ISO/IEC 42001 Clause 7.2 (Competence) requires the organization to "retain appropriate documented information as evidence of competence."
- **Evidence:** During the review of training records for the AI development team on October 24, 2025, no records of training on the newly released "Ethical AI Guidelines v2.0" could be provided for three senior data scientists (Employee IDs: 104, 107, 112), despite the internal policy requiring this training for all development staff by September 1st.
- **Finding:** The organization has failed to retain documented information as evidence of competence regarding ethical AI guidelines for all relevant personnel, in violation of Clause 7.2 and internal policy.

### Knowledge Check and Reflection
**Question 1:** Which of the following is an example of "Objective Evidence" that an auditor could use to write a nonconformity?
A) The auditor's personal belief that a specific AI algorithm is outdated.
B) A rumor from an employee that the AI system is biased against minorities.
C) A documented AI Risk Assessment report (Document ID: RA-2025-04) that is missing the required signature from the designated Risk Owner.
D) An article in a tech magazine criticizing the company's AI strategy.
*Answer: C*

**Question 2:** During an audit of Clause 8.1 (Operational Planning and Control), you observe a data scientist deploying a new AI model to production without completing the mandatory fairness testing checklist required by the company's internal procedures. When asked, the scientist says, "We were behind schedule, and my manager told me to skip it this one time." What is the finding?
A) An Opportunity for Improvement (OFI) suggesting they update their schedule.
B) A Nonconformity against Clause 8.1, as the organization failed to implement control of the processes in accordance with their established criteria.
C) Conformity, because the manager authorized the deviation.
D) A Nonconformity against the data scientist personally.
*Answer: B*

**Reflection Exercise:** Practice writing a nonconformity using the Requirement-Evidence-Finding structure. Imagine an organization's AI Policy states "All AI systems must be reviewed for privacy impacts annually." You find that the "Customer Service Chatbot" has been running for 18 months and no privacy review document exists.

### References
[1] ISMS.online. What Is Involved in an ISO 42001 Audit? https://www.isms.online/iso-42001/audit/
