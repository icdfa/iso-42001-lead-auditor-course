# Assignment 1: Scenario-Based Audit Simulation

**Course:** ISO/IEC 42001 Lead Auditor
**Provider:** Center for Professional Development, International Cybersecurity and Digital Forensics Academy
**Assignment Type:** Scenario-Based Practical Simulation
**Total Marks:** 100
**Estimated Completion Time:** 4-6 hours
**Submission Format:** Written report in PDF or Markdown format

---

## Instructions to Candidates

This assignment is designed to simulate a real-world ISO/IEC 42001 Lead Auditor engagement. You will be presented with a detailed organizational scenario and a set of audit evidence. Your task is to act as the Lead Auditor, analyze the evidence, and produce the professional deliverables described in each task below.

You must base all findings strictly on the evidence provided. Do not make assumptions beyond what is stated. Your responses will be evaluated on accuracy, use of the correct ISO/IEC 42001 clause references, clarity of writing, and the quality of your professional judgment.

---

## The Scenario: MediScan AI Ltd.

**Organization Background:**
MediScan AI Ltd. is a private healthcare technology company with 250 employees, headquartered in London, UK. The company develops and sells an AI-powered diagnostic tool called **DiagnoScan**, which analyzes medical imaging data (X-rays, MRI scans) and generates diagnostic suggestions for licensed radiologists. DiagnoScan is currently deployed in 47 hospitals across the UK and Ireland.

MediScan AI Ltd. has been pursuing ISO/IEC 42001 certification for the past 12 months. You have been engaged as the Lead Auditor by an accredited Certification Body to conduct the Stage 2 (on-site) certification audit. The Stage 1 document review was completed two weeks ago. The Stage 1 report noted two minor concerns: (1) the AI Policy had not been formally communicated to all staff, and (2) the scope document did not explicitly address the company's use of a third-party cloud provider for model training.

The on-site Stage 2 audit is now underway. The following is a collection of evidence gathered by your audit team over two days.

---

## Audit Evidence Collected

### Evidence Item A -- Interview with the CEO
During the opening meeting, you ask the CEO, Dr. Sarah Holt, about her role in the AIMS. She states: *"I signed off on the AI Policy last year and I attend the quarterly management review meetings. However, I must be honest -- the day-to-day governance of the AI system is entirely managed by our Chief Data Officer (CDO). I trust him completely. I haven't personally reviewed the risk assessment results or the impact assessment for DiagnoScan, but I'm confident everything is in order."*

### Evidence Item B -- Review of the AI Policy
You review the AI Policy (Document ID: AIMS-POL-001, Version 2.1, dated 14 March 2025). The policy is well-structured and includes a commitment to patient safety, transparency, and continual improvement. However, you note that the policy does not include any commitment to satisfy applicable legal and regulatory requirements, including the UK Medical Devices Regulations 2002 (as amended) and the NHS AI Lab's guidance on AI in healthcare.

### Evidence Item C -- Review of the AI Risk Assessment
You review the AI Risk Assessment for DiagnoScan (Document ID: AIMS-RA-2025-01). The document identifies 14 risks. You note the following:
- Risk #7 is listed as: *"Potential for the AI model to produce inaccurate diagnoses for patients from underrepresented ethnic groups due to lack of diversity in training data."* The risk is rated as **High Likelihood / High Consequence**.
- The Risk Treatment column for Risk #7 states: *"Accepted. The model performs within acceptable accuracy thresholds on average."*
- There is no documented justification for why this specific high-rated risk was accepted rather than mitigated, and no evidence of a specific control to monitor for this demographic disparity.

### Evidence Item D -- Interview with the Lead Data Scientist
You interview Dr. James Okafor, the Lead Data Scientist. You ask him to describe the process for deploying a new version of the DiagnoScan model. He explains: *"Once we finish training and internal validation, I push the new model to our staging environment. My team does a final accuracy check, and then I deploy it to production. I have full deployment access."* You ask if there is a formal sign-off or change management process. He replies: *"Not a formal one, no. We move fast. I would inform the CDO by email, but there's no mandatory approval gate before a new model version goes live to hospitals."*

### Evidence Item E -- Review of Training Records
You request training records for all 18 members of the AI development team. The HR Manager provides records for 15 individuals. She states that the remaining three team members (hired in the last two months) have not yet completed the mandatory AIMS awareness and ethical AI training, as *"the next scheduled training cohort is in six weeks."*

### Evidence Item F -- Review of the AI System Impact Assessment
You review the AI System Impact Assessment for DiagnoScan (Document ID: AIMS-IMP-2025-01). The document is thorough and covers potential impacts on patients, radiologists, and hospital administrators. However, you note that the assessment was completed in January 2024 and has not been reviewed or updated since, despite a significant update to the DiagnoScan model (Version 3.0) being deployed in November 2024, which introduced a new feature for detecting early-stage lung cancer.

### Evidence Item G -- Interview with a Hospital Client
As part of the audit, you speak with the Head of Radiology at St. Thomas' Hospital (a DiagnoScan client). She states: *"We rely heavily on DiagnoScan. Occasionally, the system flags cases with very high confidence scores that our radiologists then disagree with. We have been logging these disagreement incidents in our own internal system, but we have no formal mechanism to report them back to MediScan AI. We've mentioned it informally to our account manager, but nothing has been set up formally."*

---

## Assignment Tasks

### Task 1: Audit Finding Analysis (40 Marks)

For each of the seven evidence items (A through G), analyze the evidence and determine whether it represents:
- **(C) Conformity** -- The evidence demonstrates the requirement is being met.
- **(NC) Nonconformity** -- The evidence demonstrates a requirement is not being met.
- **(OFI) Opportunity for Improvement** -- The requirement is met, but there is a risk of future failure or a potential enhancement.

For each item you classify as **NC**, you must write a complete, formal nonconformity report using the PLO structure:
1. **The Requirement:** State the exact ISO/IEC 42001 clause and quote the relevant requirement.
2. **The Objective Evidence:** State the specific facts from the scenario that demonstrate the failure.
3. **The Finding:** Write a clear, concise statement of the nonconformity.
4. **Severity:** Classify as Major or Minor Nonconformity, with justification.

*Marking Criteria: 5 marks per evidence item (2 marks for correct classification, 3 marks for quality of PLO write-up where applicable).*

---

### Task 2: Audit Conclusions and Certification Recommendation (20 Marks)

Based on your findings from Task 1, write a formal **Audit Conclusion** section as it would appear in the final audit report. Your conclusion must:

1. Provide an overall summary of the AIMS's conformity with ISO/IEC 42001.
2. State the number and severity of nonconformities identified.
3. Make a clear, justified **certification recommendation**: Should ISO/IEC 42001 certification be **granted**, **withheld pending corrective action**, or **refused**? Justify your recommendation by referencing the specific findings.

*Marking Criteria: 10 marks for the quality and completeness of the audit conclusion summary; 10 marks for the certification recommendation and its justification.*

---

### Task 3: Corrective Action Review (20 Marks)

MediScan AI Ltd. has responded to two of your nonconformities with the following proposed corrective action plans. Review each plan and determine whether it is **Acceptable** or **Not Acceptable**. Provide a detailed justification for your decision.

**Proposed CAP for Nonconformity related to Evidence C (Risk Treatment):**
> *"We will update the risk register to change the treatment for Risk #7 from 'Accepted' to 'Mitigated.' We will add a note stating that the model's average accuracy is acceptable."*

**Proposed CAP for Nonconformity related to Evidence D (Change Management):**
> *"We will immediately create a formal Change Management Procedure for AI model deployments. This procedure will require mandatory sign-off from the CDO and a completed fairness and safety checklist before any new model version is deployed to production. We will implement this within 30 days and provide evidence of the first deployment completed under the new procedure."*

*Marking Criteria: 10 marks per CAP review (5 marks for the correct Accept/Reject decision, 5 marks for the quality of justification).*

---

### Task 4: Closing Meeting Preparation (20 Marks)

You are preparing to conduct the closing meeting with MediScan AI Ltd.'s senior management team. Write a structured **Closing Meeting Agenda and Speaking Notes** that you would use to lead this meeting. Your notes must include:

1. An opening statement thanking the auditee and reiterating the audit scope and objectives.
2. A statement explaining the nature of sampling-based audits and its implications.
3. A summary of positive observations and areas of strong conformity.
4. A clear and professional presentation of the nonconformities, including how you would handle potential pushback from the CEO.
5. A statement of the next steps and the certification decision timeline.

*Marking Criteria: 4 marks per section (clarity, professionalism, and accuracy of content).*

---

## Submission Checklist

Before submitting, ensure your assignment includes:
- [ ] Your full name and student ID.
- [ ] Completed Task 1 with a finding for each of the seven evidence items.
- [ ] Completed Task 2 with a formal audit conclusion and certification recommendation.
- [ ] Completed Task 3 with a justified review of both corrective action plans.
- [ ] Completed Task 4 with structured closing meeting notes.

---

## Grading Rubric Summary

| Task | Description | Marks |
| :--- | :--- | :--- |
| Task 1 | Audit Finding Analysis (7 items) | 40 |
| Task 2 | Audit Conclusions & Certification Recommendation | 20 |
| Task 3 | Corrective Action Plan Review | 20 |
| Task 4 | Closing Meeting Preparation | 20 |
| **Total** | | **100** |

**Pass Mark:** 70/100

---

*(c) 2026 International Cybersecurity and Digital Forensics Academy. All Rights Reserved.*
