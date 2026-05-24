# Auditing Practical Guide: ISO/IEC 42001 Lead Auditor

**Provider:** Center for Professional Development, International Cybersecurity and Digital Forensics Academy
**Document Type:** Practical Reference Guide
**Standard Reference:** ISO/IEC 42001:2023 | ISO 19011:2018

---

## Foreword

This Practical Guide is your hands-on companion for the entire ISO/IEC 42001 audit lifecycle. While the course modules provide the theoretical foundation, this guide translates that knowledge into actionable steps, ready-to-use templates, interview question banks, and professional judgment frameworks. Whether you are preparing for your first Lead Auditor engagement or refreshing your skills, this guide is designed to sit open on your desk throughout every audit.

---

## Chapter 1: The Lead Auditor Mindset

### 1.1 What Makes a Great AI Auditor?
Auditing an Artificial Intelligence Management System is fundamentally different from auditing a traditional quality or information security management system. The subject matter -- AI systems -- is technically complex, rapidly evolving, and carries profound ethical implications. A great ISO/IEC 42001 Lead Auditor must blend three distinct skill sets:

**Technical Literacy:** You do not need to be a data scientist or machine learning engineer. However, you must understand the AI lifecycle well enough to ask the right questions. You must know what training data is, what model validation means, what "concept drift" looks like, and why a model's average accuracy can mask serious fairness problems for specific demographic groups. Without this literacy, auditees can mislead you -- not necessarily with malicious intent, but simply because they assume you do not understand the nuances.

**Auditing Rigor:** You must apply the seven principles of ISO 19011 (Integrity, Fair Presentation, Due Professional Care, Confidentiality, Independence, Evidence-based Approach, Risk-based Approach) with absolute consistency. Every finding must be grounded in objective, verifiable evidence. Your personal opinions about AI ethics, however well-intentioned, are not audit evidence.

**Professional Judgment:** The standard cannot anticipate every situation. There will be moments in every audit where you must exercise professional judgment -- deciding whether a finding is a major or minor nonconformity, determining whether a corrective action plan genuinely addresses the root cause, or managing a difficult conversation with a defensive CEO. This guide will help you develop that judgment.

### 1.2 The Auditor's Non-Negotiable Commitments
Before every engagement, a Lead Auditor must confirm the following:

- **No Conflict of Interest:** You have not provided consulting, implementation, or advisory services to the auditee organization within the past two years. You have no financial interest in the outcome of the audit.
- **Competence:** Your audit team collectively possesses the technical and auditing competence required for this specific engagement. If the auditee uses a specialized AI system (e.g., a medical diagnostic AI), you have included a technical expert on the team.
- **Confidentiality:** You will treat all information obtained during the audit as strictly confidential. You will not discuss findings with third parties, use information for personal gain, or share proprietary details of the auditee's AI systems.

---

## Chapter 2: Pre-Audit Preparation -- A Step-by-Step Walkthrough

### 2.1 Step 1 -- Receiving the Audit Brief
Your engagement begins when you receive the audit brief from the Certification Body (for third-party audits) or the audit client (for internal or second-party audits). The brief should specify:
- The auditee organization's name and primary contact.
- The proposed audit scope (which AI systems and organizational units are included).
- The audit objectives (e.g., initial certification, surveillance audit, recertification).
- The proposed audit dates and duration.
- Any known constraints or special requirements.

**Action:** Review the brief carefully. If the scope is unclear or the proposed duration seems insufficient for the complexity of the AIMS, raise this with the audit client *before* confirming the engagement.

### 2.2 Step 2 -- Conducting the Stage 1 (Document Review)
The Stage 1 audit is a desk-based review of the auditee's documented information. Its purpose is to assess the organization's readiness for the Stage 2 on-site audit and to gather information for planning.

**Documents to Request:**
Request the following documents from the auditee at least two weeks before the Stage 1:

| Document | Purpose of Review |
| :--- | :--- |
| AIMS Scope Document | Verify that the scope is clearly defined and appropriate. |
| AI Policy | Verify it meets all requirements of Clause 5.2. |
| Statement of Applicability (SoA) | Identify which Annex A controls are included/excluded and why. |
| AI Risk Assessment (most recent) | Verify a methodology exists and has been applied. |
| AI System Impact Assessment (most recent) | Verify it covers impacts on individuals and society. |
| Risk Treatment Plan | Verify risks have been addressed with appropriate controls. |
| Internal Audit Reports (last cycle) | Identify previously found nonconformities and their status. |
| Management Review Minutes (last cycle) | Verify top management engagement with the AIMS. |
| Competence/Training Records (sample) | Verify personnel have the required skills. |
| Documented Procedures (key processes) | Verify operational controls are documented. |

**Stage 1 Output:** A written Stage 1 Report that summarizes the document review findings, identifies any significant gaps that must be resolved before Stage 2, and confirms the readiness for the on-site audit.

### 2.3 Step 3 -- Developing the Audit Plan
Based on the Stage 1 findings, develop a detailed, risk-based audit plan. Allocate more time to high-risk areas identified in the SoA and risk assessment.

**Audit Plan Template:**

| Time Slot | Activity | Auditor | Location | Clause(s) |
| :--- | :--- | :--- | :--- | :--- |
| Day 1, 09:00-09:30 | Opening Meeting | Lead Auditor | Boardroom | -- |
| Day 1, 09:30-11:00 | Interview: CEO / Top Management | Lead Auditor | Boardroom | 5.1, 5.2, 9.3 |
| Day 1, 11:00-12:30 | Interview: CDO / Risk Owner | Lead Auditor | CDO Office | 6.1, 6.2 |
| Day 1, 13:30-15:30 | Review: Risk & Impact Assessments | Lead Auditor + Technical Expert | Conference Room | 6.1.2, 6.1.3 |
| Day 1, 15:30-17:00 | Interview: Lead Data Scientist | Technical Expert | AI Lab | 7.2, 8.1 |
| Day 2, 09:00-11:00 | Observation: Model Deployment Process | Technical Expert | IT Operations | 8.1 |
| Day 2, 11:00-12:30 | Review: Training Records & Competence | Lead Auditor | HR Department | 7.2 |
| Day 2, 13:30-15:00 | Review: Monitoring Dashboards & Incident Logs | Technical Expert | IT Operations | 9.1 |
| Day 2, 15:00-16:00 | Audit Team Debrief & Conclusion Preparation | Audit Team | Conference Room | -- |
| Day 2, 16:00-17:00 | Closing Meeting | Lead Auditor | Boardroom | -- |

### 2.4 Step 4 -- Preparing Your Audit Checklists
Develop checklists for each clause you will audit. Below is a comprehensive checklist for the most critical clauses of ISO/IEC 42001.

---

## Chapter 3: The Master Audit Checklist for ISO/IEC 42001

> **Instructions:** For each item, record your finding as: **C** (Conformity), **NC** (Nonconformity), **OFI** (Opportunity for Improvement), or **NA** (Not Applicable). Record the specific evidence in the "Evidence Notes" column.

### Clause 4: Context of the Organization

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 4.1.1 | Has the organization identified relevant external issues (legal, regulatory, technological, societal)? | Documented context analysis; PESTLE or similar analysis. | | |
| 4.1.2 | Has the organization identified relevant internal issues (strategy, culture, resources, AI maturity)? | Internal context document; strategic plans. | | |
| 4.2.1 | Has the organization identified all relevant interested parties? | Stakeholder register or equivalent document. | | |
| 4.2.2 | Has the organization determined the relevant requirements of interested parties? | Requirements matrix; customer contracts; regulatory requirements list. | | |
| 4.3.1 | Is the AIMS scope clearly documented, including the AI systems and organizational units covered? | Scope document; confirm it is available as documented information. | | |
| 4.3.2 | Does the scope clearly state any exclusions and provide justification? | Scope document. | | |

### Clause 5: Leadership

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 5.1.1 | Can top management demonstrate active commitment to the AIMS (beyond just signing the policy)? | Interview with CEO/Board; management review minutes; resource allocation records. | | |
| 5.1.2 | Has top management ensured AIMS requirements are integrated into business processes? | Evidence of AI governance in business planning; project approval processes. | | |
| 5.2.1 | Is there a documented AI Policy that is appropriate to the organization's purpose? | AI Policy document. | | |
| 5.2.2 | Does the AI Policy include a commitment to satisfy applicable requirements (legal, regulatory)? | Review policy text for explicit commitment. | | |
| 5.2.3 | Does the AI Policy include a commitment to continual improvement of the AIMS? | Review policy text for explicit commitment. | | |
| 5.2.4 | Has the AI Policy been communicated to all relevant personnel? | Communication records; awareness training logs; intranet postings. | | |
| 5.3.1 | Are responsibilities and authorities for AIMS roles clearly assigned and communicated? | RACI matrix; job descriptions; organizational chart. | | |

### Clause 6: Planning

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 6.1.1 | Has the organization determined risks and opportunities that need to be addressed by the AIMS? | Risk register; documented risk and opportunity analysis. | | |
| 6.1.2 | Has the organization defined and applied a repeatable AI risk assessment process? | Risk assessment methodology document; multiple completed risk assessments. | | |
| 6.1.2 | Does the risk assessment identify risk owners and assess likelihood and consequence? | Review risk assessment records for completeness. | | |
| 6.1.3 | Has the organization defined and applied an AI System Impact Assessment process? | Impact assessment methodology; completed impact assessment for each AI system. | | |
| 6.1.4 | Has the organization defined and applied an AI risk treatment process? | Risk treatment plan; evidence of control implementation. | | |
| 6.1.4 | Has the organization produced a Statement of Applicability (SoA)? | SoA document; verify it includes all required elements (controls, justifications, exclusions). | | |
| 6.2.1 | Has the organization established AI objectives at relevant functions and levels? | Documented AI objectives; verify they are measurable and consistent with the AI Policy. | | |
| 6.2.2 | Has the organization developed plans to achieve its AI objectives? | Action plans; project plans; resource allocation records. | | |

### Clause 7: Support

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 7.1.1 | Has the organization determined and provided the necessary resources for the AIMS? | Budget records; staffing plans; infrastructure documentation. | | |
| 7.2.1 | Has the organization determined the necessary competence for AIMS-relevant roles? | Competence framework; job descriptions; skills matrix. | | |
| 7.2.2 | Has the organization ensured personnel are competent and retained evidence? | Training records; certifications; performance reviews. | | |
| 7.3.1 | Are relevant personnel aware of the AI Policy and their contribution to the AIMS? | Awareness training records; interview staff to verify awareness. | | |
| 7.4.1 | Has the organization determined relevant internal and external communications for the AIMS? | Communications plan; incident reporting procedures. | | |
| 7.5.1 | Does the AIMS include all documented information required by ISO/IEC 42001? | Review against the standard's list of required documented information. | | |
| 7.5.2 | Is documented information adequately controlled (access, version control, protection)? | Document management system; version history; access logs. | | |

### Clause 8: Operation

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 8.1.1 | Has the organization planned, implemented, and controlled the processes needed to meet AIMS requirements? | Documented procedures for AI lifecycle stages; evidence of process execution. | | |
| 8.1.2 | Does the organization have criteria for its AI processes and evidence of adherence? | Process criteria (e.g., accuracy thresholds, fairness metrics); test reports. | | |
| 8.1.3 | Does the organization control planned changes and review unintended changes? | Change management procedure; change log; impact assessments for changes. | | |
| 8.1.4 | Does the organization ensure outsourced AI processes are controlled? | Vendor contracts; SLAs; supplier audit records; due diligence documentation. | | |
| 8.2.1 | Does the organization manage data used in AI systems (quality, provenance, bias)? | Data governance policy; data quality reports; data lineage documentation. | | |

### Clause 9: Performance Evaluation

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 9.1.1 | Has the organization determined what to monitor and measure for the AIMS and AI systems? | Monitoring and measurement plan; KPI definitions. | | |
| 9.1.2 | Is there evidence that monitoring and measurement is being performed and results analyzed? | Performance dashboards; monitoring reports; trend analysis. | | |
| 9.2.1 | Does the organization have a documented internal audit program? | Audit program document; audit schedule. | | |
| 9.2.2 | Are internal audits conducted at planned intervals by competent, impartial auditors? | Internal audit reports; auditor qualifications; evidence auditors did not audit own work. | | |
| 9.3.1 | Does top management conduct formal management reviews at planned intervals? | Management review meeting minutes; agenda; attendance records. | | |
| 9.3.2 | Do management review inputs include all required items (previous actions, trends, feedback, risks)? | Review meeting minutes against the list of required inputs in Clause 9.3.2. | | |
| 9.3.3 | Do management review outputs include decisions on improvement, changes, and resources? | Review meeting minutes for documented decisions and action items. | | |

### Clause 10: Improvement

| # | Audit Question | Evidence to Seek | Finding | Evidence Notes |
| :--- | :--- | :--- | :--- | :--- |
| 10.1.1 | When nonconformities occur, does the organization react, analyze root causes, and implement corrective actions? | Nonconformity log; corrective action records; root cause analysis documentation. | | |
| 10.1.2 | Does the organization review the effectiveness of corrective actions taken? | Evidence of follow-up verification; closed nonconformity records. | | |
| 10.2.1 | Does the organization continually improve the suitability, adequacy, and effectiveness of the AIMS? | Evidence of proactive improvements; updated risk assessments; revised procedures. | | |

---

## Chapter 4: Conducting Effective Audit Interviews

### 4.1 The OSCE Interview Framework
Effective audit interviews follow a structured approach. Use the OSCE framework to guide every interview:

- **O -- Open:** Begin with open-ended questions to establish rapport and gather broad information. ("Can you describe your role in the AI development process?")
- **S -- Specific:** Drill down into specific areas of interest or concern. ("You mentioned you conduct bias checks -- can you show me the most recent bias evaluation report for the DiagnoScan model?")
- **C -- Clarify:** Clarify any ambiguous or contradictory statements. ("Earlier you said the risk assessment is updated annually, but this document is dated 18 months ago -- can you help me understand that?")
- **E -- Evidence:** Always request to see the evidence that supports what the interviewee is telling you. ("That sounds like a robust process. Could I see the completed checklist from the last model deployment?")

### 4.2 Interview Question Bank by Clause

**For Top Management (Clause 5 -- Leadership):**
- "How do you personally demonstrate your commitment to responsible AI governance within this organization?"
- "When did you last review the results of the AI risk assessment, and what decisions did you make as a result?"
- "How do you ensure that AI governance considerations are factored into major business decisions, such as launching a new AI product?"
- "What would you say are the top three AI-related risks your organization faces today?"

**For the Chief Data Officer / Risk Owner (Clause 6 -- Planning):**
- "Walk me through the process you follow when you need to assess the risks of a new AI system before deployment."
- "How do you decide whether a risk should be accepted, mitigated, or avoided?"
- "Can you explain the purpose of your Statement of Applicability and how it was developed?"
- "How do you ensure that the impact of your AI systems on vulnerable individuals or minority groups is adequately assessed?"

**For the Lead Data Scientist / AI Developer (Clause 8 -- Operation):**
- "Describe the steps you follow from the moment you decide to train a new model to the moment it goes live in production."
- "What controls do you have in place to detect and address bias in your training data?"
- "What happens if you discover that a deployed model is performing below its expected accuracy threshold?"
- "How do you manage changes to an existing model -- for example, retraining it with new data?"

**For the HR Manager (Clause 7 -- Support):**
- "How do you determine what AI-related training is required for different roles in the organization?"
- "How do you track whether employees have completed their mandatory AIMS training?"
- "What happens when a new employee joins the AI team -- what is the onboarding process for AIMS awareness?"

**For IT Operations / Monitoring Team (Clause 9 -- Performance Evaluation):**
- "What metrics do you monitor for your AI systems on a day-to-day basis?"
- "How do you distinguish between a normal fluctuation in model performance and a significant degradation that requires action?"
- "How are AI-related incidents reported and tracked?"

### 4.3 Handling Difficult Interview Situations

**Situation: The Interviewee is Evasive**
Some interviewees will give vague, high-level answers to avoid exposing problems. The best response is to ask for specific examples and evidence. If they say "We always follow the procedure," ask: "Could you show me the record from the last time you followed that procedure?"

**Situation: The Interviewee is Overly Technical**
In AI audits, technical staff may use jargon to deflect scrutiny. Do not pretend to understand something you do not. Ask them to explain it in plain language. "I want to make sure I understand this correctly -- could you explain what you mean by 'regularization' in the context of your model's fairness controls?"

**Situation: The Interviewee Becomes Defensive or Hostile**
Remain calm, professional, and factual. Remind them that the audit is a collaborative process aimed at improvement, not punishment. Restate your finding objectively and offer to discuss it further with their management representative if needed.

---

## Chapter 5: Writing Findings -- The Professional Standard

### 5.1 The PLO Structure in Depth
Every nonconformity must be written using the PLO (Provision-Location-Objective Evidence) structure, also commonly referred to as the Requirement-Evidence-Finding structure. A nonconformity that cannot be clearly traced back to a specific requirement and specific objective evidence is not a valid finding.

**The Three Elements:**

**1. The Provision (The Requirement):**
State the specific clause of ISO/IEC 42001 or the organization's own documented policy that has not been met. Quote the exact text of the requirement.
> *Example: "ISO/IEC 42001 Clause 7.2 requires the organization to 'retain appropriate documented information as evidence of competence.'"*

**2. The Location (Where/Who):**
Identify where the evidence was found -- the specific department, document, or person. This makes the finding traceable and actionable.
> *Example: "During a review of training records for the AI Development Team on 24 May 2026..."*

**3. The Objective Evidence (The Facts):**
State the specific, verifiable facts that demonstrate the requirement was not met. Be precise. Include document IDs, dates, names (where appropriate), and specific data points.
> *Example: "...no records of completion of the mandatory 'Ethical AI Guidelines v2.0' training could be provided for three data scientists (Employee IDs: 104, 107, 112), despite the internal AIMS procedure (AIMS-PROC-007) requiring this training for all development staff by 1 September 2025."*

**The Final Finding Statement:**
Combine the above into a single, clear statement.
> *"The organization has failed to retain documented information as evidence of competence for all relevant AI development personnel, specifically regarding the 'Ethical AI Guidelines v2.0' training, in violation of ISO/IEC 42001 Clause 7.2 and internal procedure AIMS-PROC-007."*

### 5.2 Major vs. Minor Nonconformity: Making the Call
One of the most important judgment calls a Lead Auditor makes is classifying a nonconformity as Major or Minor. This classification directly affects the certification outcome.

| Classification | Definition | Certification Impact | Example |
| :--- | :--- | :--- | :--- |
| **Major Nonconformity** | The absence of, or total breakdown of, a required system element. A situation that raises significant doubt about the ability of the AIMS to achieve its intended outcomes. A situation that could result in significant harm to individuals or society. | Certification cannot be granted or maintained until all major NCs are closed and verified. | No AI Risk Assessment has ever been conducted. A deployed AI system is causing demonstrable harm with no controls in place. |
| **Minor Nonconformity** | A single observed lapse or failure that does not indicate a systemic breakdown of the AIMS. The overall system element is in place and functioning, but there is a specific, isolated failure. | Certification may be granted, but the auditee must submit and implement a corrective action plan within an agreed timeframe. | Three out of 18 training records are missing. One risk in the risk register lacks a documented treatment justification. |

---

## Chapter 6: Post-Audit Activities

### 6.1 The Audit Report -- Structure and Standards
The audit report is the formal, permanent record of the audit. It must be objective, accurate, and complete. The Lead Auditor is responsible for its content.

**Standard Audit Report Structure:**
1. **Cover Page:** Audit reference number, auditee name, audit dates, audit team members, report date.
2. **Executive Summary:** A brief, high-level overview of the audit scope, objectives, and overall conclusion.
3. **Audit Scope, Objectives, and Criteria:** Detailed statement of what was audited and against what criteria.
4. **Audit Process Summary:** A description of the audit activities conducted (interviews, document reviews, observations), including any limitations or obstacles encountered.
5. **Audit Findings:** A detailed list of all findings (conformities, nonconformities, OFIs), each written in the PLO format.
6. **Audit Conclusions:** The overall assessment of the AIMS's conformity and effectiveness, and the certification recommendation.
7. **Appendices:** Audit plan, attendance lists, checklist records.

### 6.2 Reviewing Corrective Action Plans
When the auditee submits a corrective action plan (CAP) for each nonconformity, the Lead Auditor must review it critically. A good CAP addresses the **root cause**, not just the symptom.

**The Five-Question Test for a CAP:**
1. Does the CAP correctly identify the root cause of the nonconformity?
2. Does the proposed action directly address that root cause?
3. Is the proposed action realistic and achievable within the proposed timeframe?
4. Does the CAP include a mechanism to verify that the action has been implemented?
5. Does the CAP include a mechanism to verify that the action was *effective* (i.e., the nonconformity will not recur)?

If the answer to any of these questions is "No," the CAP must be rejected and the auditee must revise it.

### 6.3 Closing Nonconformities
A nonconformity is only closed when the Lead Auditor has verified, through objective evidence, that:
1. The corrective action has been fully implemented.
2. The action has been effective in eliminating the root cause.

Evidence for closing can be submitted remotely (e.g., updated documents, training records, screenshots of new system controls) or verified during a follow-up on-site visit, depending on the severity of the nonconformity.

---

## Chapter 7: Quick Reference -- ISO/IEC 42001 Clause Summary

| Clause | Title | Core Requirement |
| :--- | :--- | :--- |
| **4.1** | Understanding the organization | Determine internal and external issues relevant to the AIMS. |
| **4.2** | Interested parties | Identify stakeholders and their requirements. |
| **4.3** | Scope | Define and document the boundaries of the AIMS. |
| **5.1** | Leadership | Top management must demonstrate active commitment. |
| **5.2** | AI Policy | Establish, implement, and maintain an AI Policy. |
| **5.3** | Roles & Responsibilities | Assign and communicate AIMS roles. |
| **6.1** | Risks & Opportunities | Plan actions to address risks and opportunities. |
| **6.1.2** | AI Risk Assessment | Define and apply a repeatable risk assessment process. |
| **6.1.3** | AI System Impact Assessment | Assess impacts on individuals, groups, and society. |
| **6.1.4** | AI Risk Treatment | Select and implement controls; produce the SoA. |
| **6.2** | AI Objectives | Establish measurable AI objectives and plans to achieve them. |
| **7.1** | Resources | Provide necessary resources for the AIMS. |
| **7.2** | Competence | Ensure and evidence personnel competence. |
| **7.3** | Awareness | Ensure personnel are aware of the AI Policy and their role. |
| **7.4** | Communication | Determine internal and external communication needs. |
| **7.5** | Documented Information | Create, control, and maintain required documented information. |
| **8.1** | Operational Planning & Control | Plan, implement, and control AI system lifecycle processes. |
| **9.1** | Monitoring & Measurement | Monitor and measure AIMS and AI system performance. |
| **9.2** | Internal Audit | Conduct planned, impartial internal audits. |
| **9.3** | Management Review | Top management reviews the AIMS at planned intervals. |
| **10.1** | Nonconformity & Corrective Action | React to nonconformities, analyze root causes, and act. |
| **10.2** | Continual Improvement | Continually improve the AIMS. |

---

*(c) 2026 International Cybersecurity and Digital Forensics Academy. All Rights Reserved.*
