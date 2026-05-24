# ISO/IEC 42001 Lead Auditor Training Course: The Complete Guide

## Module 7: Preparing for an ISO/IEC 42001 Audit

### Learning Objectives
By the end of this module, you will be able to:
1. Understand the necessary steps involved in initiating an audit.
2. Describe the purpose, scope, and execution of a document review (Stage 1 Audit).
3. Develop a comprehensive, risk-based audit plan.
4. Create effective audit working documents, including detailed checklists and sampling plans.
5. Understand how to allocate resources and assign tasks to the audit team effectively.

### 7.1 Initiating the Audit: Laying the Groundwork
The audit process begins long before the auditor arrives on site. The initiation phase sets the tone for the entire audit. The primary goals here are to establish formal contact with the auditee, confirm the authority to conduct the audit, and determine the feasibility of the audit.

**Key steps in initiation:**
- **Establish Contact:** The Lead Auditor formally contacts the auditee's representative. This communication outlines the audit's purpose, proposed scope, and proposed dates. It also establishes the communication channels that will be used throughout the audit.
- **Determine Feasibility:** The Lead Auditor must assess whether the audit can be successfully executed. This is a critical "go/no-go" decision point. Feasibility involves confirming that:
 - Sufficient and appropriate information is available for planning and conducting the audit.
 - Adequate cooperation from the auditee is expected.
 - Adequate time and resources (including auditor competence) are available.
 If the audit is deemed unfeasible (e.g., the organization refuses to provide basic documentation), an alternative must be proposed to the audit client, or the audit must be canceled.

### 7.2 Document Review (Stage 1 Audit): The Desk Study
Before conducting the on-site assessment, the auditor must review the auditee's documented information. In formal certification audits, this is known as the Stage 1 Audit [1]. The purpose is twofold: to determine conformity with the standard on paper, and to gather information to support the planning of the on-site audit (Stage 2).

**Documents typically reviewed for ISO/IEC 42001 include:**
- The AI Policy and the documented scope of the AIMS.
- The AI Risk Assessment methodology and the results of recent risk assessments.
- The AI System Impact Assessment methodology and results.
- The Statement of Applicability (SoA) - this is a crucial document that guides the Stage 2 audit.
- Procedures for AI system lifecycle management (design, development, deployment).
- Records of previous internal audits and management reviews.

The output of the document review informs the Lead Auditor whether the organization is ready for the on-site audit. If the Stage 1 audit reveals that the organization hasn't even completed a risk assessment, there is no point in proceeding to Stage 2. The Lead Auditor will report these significant gaps, and the on-site audit may be postponed until the issues are resolved.

### 7.3 Preparing the Audit Plan: The Roadmap
The audit plan is the roadmap for the on-site audit. It must be flexible enough to permit changes based on information gathered during the audit, but structured enough to ensure all objectives are met within the allotted time. The Lead Auditor prepares the plan based on the information gathered during the document review and the audit program objectives.

A risk-based approach must be applied when planning. Areas of the AIMS that pose higher risks (e.g., a generative AI model interacting directly with the public) should be allocated more audit time than lower-risk areas (e.g., an internal tool used for sorting IT support tickets).

**A comprehensive audit plan should include:**
- **Audit Objectives:** What the audit intends to achieve (e.g., verify conformity to ISO/IEC 42001 for certification).
- **Audit Scope:** The boundaries of the audit (e.g., physical locations, organizational units, specific AI systems covered).
- **Audit Criteria:** The reference documents against which conformity is determined (ISO/IEC 42001, the organization's internal AI policies, applicable legal requirements).
- **Locations, Dates, and Expected Time:** A detailed schedule of meetings and audit activities.
- **Roles and Responsibilities:** Specific assignments for audit team members and any accompanying persons (e.g., guides or technical experts).

### 7.4 Developing Audit Working Documents: The Auditor's Toolkit
Audit working documents are tools used by auditors to structure their work, record evidence, and ensure that the audit covers all necessary requirements efficiently.

#### 7.4.1 Audit Checklists
Checklists are structured lists of questions or points to verify during the audit. They ensure that the auditor does not forget to check specific requirements of the standard. However, checklists are a guide, not a script. They should not restrict the auditor from investigating additional leads or "pulling the thread" when an issue arises during the audit.

*Example Checklist Item for Clause 6.1.2 (AI Risk Assessment):*
- **Requirement:** The organization shall define and apply an AI risk assessment process.
- **Question for Auditee:** Can you walk me through the process you use to identify and evaluate AI risks for new projects?
- **Evidence to Look For:** Documented risk assessment methodology; completed risk assessment reports for recent AI projects.
- **Question for Auditee:** How do you ensure that repeated assessments produce consistent results?
- **Evidence to Look For:** Standardized risk matrices or scoring rubrics; evidence of calibration among risk assessors.

#### 7.4.2 Sampling Plans
Auditors cannot review every single line of code, every single training data file, or every single record. They must rely on sampling. A sampling plan defines how the auditor will select a representative subset of data to draw conclusions about the whole system.

- **Statistical Sampling:** Selecting samples randomly based on statistical formulas to achieve a specific confidence level. (e.g., randomly selecting 50 out of 10,000 AI decisions to review for accuracy).
- **Judgment-Based Sampling:** Selecting samples based on the auditor's experience, knowledge, and risk assessment. (e.g., specifically selecting AI projects that were flagged as "high risk" in the impact assessment, or selecting records from a newly hired data scientist).

### Knowledge Check and Reflection
**Question 1:** During the Initiation phase, the Lead Auditor determines that the organization has not yet finalized its AI Policy and refuses to share any risk assessment data due to "pending legal review." What is the most appropriate action for the Lead Auditor?
A) Proceed to the on-site audit anyway and write nonconformities for everything.
B) Determine that the audit is unfeasible at this time and propose postponing the audit to the audit client.
C) Write the AI Policy for the organization so the audit can proceed.
D) Skip the document review and go straight to interviewing employees.
*Answer: B*

**Question 2:** Why is a "risk-based approach" important when developing an audit plan?
A) It ensures the auditor spends equal time on every single clause of the standard.
B) It allows the auditor to focus their limited time and resources on the areas of the AIMS that pose the greatest potential impact or have the highest likelihood of nonconformity.
C) It guarantees that the auditor will find a major nonconformity.
D) It allows the auditor to skip auditing the top management.
*Answer: B*

**Reflection Exercise:** You are preparing a checklist to audit Clause 7.2 (Competence). Write two specific questions you would ask the HR manager, and list the specific documented evidence you would ask to see to verify their answers.

### References
[1] ISMS.online. What Is Involved in an ISO 42001 Audit? https://www.isms.online/iso-42001/audit/
