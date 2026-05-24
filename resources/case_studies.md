# Case Studies: How an ISO/IEC 42001 Audit is Conducted

**Provider:** Center for Professional Development, International Cybersecurity and Digital Forensics Academy
**Document Type:** Comprehensive Case Study Collection
**Standard Reference:** ISO/IEC 42001:2023 | ISO 19011:2018

---

## Introduction

The following case studies are designed to walk you through the complete ISO/IEC 42001 audit lifecycle from initiation to closure. Each case study presents a different organizational context, AI system type, and set of audit challenges. By studying how the Lead Auditor thinks, plans, investigates, and reports in each scenario, you will develop the professional judgment needed to handle real-world audit engagements.

Each case study is structured in phases, mirroring the actual audit process: Pre-Audit, Stage 1, Stage 2, Closing, and Follow-up.

---

## Case Study 1: FinGuard Analytics -- AI-Powered Credit Scoring (Financial Services)

### Organization Profile
**Organization:** FinGuard Analytics Ltd.
**Sector:** Financial Services (Consumer Lending)
**Size:** 180 employees
**AI System:** "CreditIQ" -- a machine learning model that automates credit scoring and loan approval decisions for personal loan applications.
**Audit Type:** Initial ISO/IEC 42001 Certification Audit (Third-Party)
**Audit Duration:** 2 days on-site (Stage 2)

---

### Phase 1: Pre-Audit -- Initiation and Stage 1 Document Review

**Audit Initiation:**
The Lead Auditor, Ms. Amara Diallo, receives the audit brief from the Certification Body. She reviews the brief and notes that CreditIQ processes approximately 5,000 loan applications per day and that automated decisions are made without human review for applications below a certain risk threshold. She immediately flags this as a high-risk area requiring focused attention during the audit, as automated financial decisions affecting consumers are subject to strict regulatory scrutiny under UK financial regulations.

Ms. Diallo contacts the auditee's AIMS Manager, Mr. Ben Carter, to establish communication and request the Stage 1 documentation package.

**Stage 1 Document Review Findings:**

Ms. Diallo reviews the submitted documents and produces the following Stage 1 summary:

| Document Reviewed | Finding |
| :--- | :--- |
| AI Policy (AIMS-POL-001 v1.2) | Policy is well-structured. However, it does not explicitly reference the FCA's (Financial Conduct Authority) Consumer Duty regulations, which require firms to deliver good outcomes for retail customers. This is a gap. |
| AIMS Scope Document | Scope clearly covers CreditIQ and the UK consumer lending division. Excludes the commercial lending division with a justification that it uses only rule-based systems. Justification is acceptable. |
| AI Risk Assessment (AIMS-RA-2025-03) | Risk assessment methodology is documented and appears repeatable. 22 risks identified. Risk #14 ("Model produces discriminatory outcomes for protected characteristics") is rated High and treated with a control: "Quarterly fairness testing." No evidence of the actual fairness testing reports is included. |
| AI System Impact Assessment | Impact assessment is present and covers impacts on loan applicants. However, it was last updated 14 months ago and does not reflect a significant model update (CreditIQ v4.0) deployed 6 months ago. |
| Statement of Applicability (SoA) | SoA is present. Three Annex A controls are excluded. Two exclusions have justifications; one exclusion (related to transparency of AI decisions) has no justification. |
| Internal Audit Report (Last Cycle) | One internal audit was conducted 8 months ago. It identified a minor nonconformity regarding training records. The corrective action is marked as "closed" but no verification evidence is attached. |
| Management Review Minutes | Management review was conducted 5 months ago. Minutes are brief and do not show evidence that risk assessment results were discussed. |

**Stage 1 Conclusion:**
Ms. Diallo issues a Stage 1 Report noting three areas of concern that must be addressed before Stage 2: (1) the missing justification for the SoA exclusion, (2) the outdated Impact Assessment, and (3) the lack of evidence for the closed corrective action. She recommends proceeding to Stage 2 on the condition that the auditee provides updated documentation addressing these points within two weeks.

FinGuard Analytics provides an updated SoA with the missing justification and an updated Impact Assessment. The corrective action evidence is also provided. Ms. Diallo reviews the updates and confirms Stage 2 can proceed.

---

### Phase 2: Stage 2 -- On-Site Audit (Day 1)

**Opening Meeting (09:00 - 09:30):**
Ms. Diallo opens the meeting, introduces herself and her Technical Expert (a specialist in financial ML models), and confirms the audit plan. She explains that the audit will be based on sampling and that the absence of findings does not guarantee the absence of nonconformities. The CEO, CFO, and AIMS Manager are present. The CEO expresses confidence in their AIMS and states that "responsible AI is at the heart of our business." Ms. Diallo notes this statement for follow-up during the management interview.

**Interview: CEO and CFO (09:30 - 11:00):**
Ms. Diallo interviews the CEO and CFO about their leadership role in the AIMS.

- *Auditor:* "You mentioned that responsible AI is at the heart of your business. Can you tell me about the last time you personally reviewed the results of the AI risk assessment?"
- *CEO:* "I review the AIMS dashboard that Ben [the AIMS Manager] sends me monthly. It shows green for most things."
- *Auditor:* "Can you describe what information is on that dashboard?"
- *CEO:* "Uptime, processing speed, approval rates... the usual metrics."
- *Auditor:* "Does the dashboard include the results of the fairness testing for CreditIQ -- for example, whether the model is approving or rejecting applications at different rates for different demographic groups?"
- *CEO (pausing):* "I don't think that's on the current dashboard. That's more of a technical detail that Ben and the data team handle."

**Auditor's Note:** This is a significant finding. The CEO is not receiving information about the AI system's fairness performance, which is one of the highest-rated risks in the risk assessment. This suggests a gap in the monitoring and reporting chain up to top management (Clause 9.1 and 9.3).

**Interview: AIMS Manager and Review of Risk Assessment (11:00 - 13:00):**
Ms. Diallo reviews the risk assessment with Mr. Carter and asks to see the quarterly fairness testing reports referenced as the control for Risk #14.

- *Mr. Carter:* "The fairness testing is done by the data science team. Let me pull those up."
- *After a 10-minute search:* "I can find the report from Q1 of this year, but I'm having trouble locating Q2 and Q3."
- *Auditor:* "The risk assessment states this is a quarterly control. We are now in Q4. I would expect to see three completed reports for this year. You have one. Can you confirm whether the Q2 and Q3 tests were conducted?"
- *Mr. Carter:* "I believe they were, but I cannot provide the documentation right now."

**Auditor's Note:** This is a nonconformity. The control documented in the risk treatment plan (quarterly fairness testing) is not being executed as planned, and evidence cannot be provided. This relates to Clause 8.1 (operational control) and Clause 9.1 (monitoring and measurement).

---

### Phase 3: Stage 2 -- On-Site Audit (Day 2)

**Observation: CreditIQ Decision Process (09:00 - 11:00):**
The Technical Expert observes the CreditIQ system processing live applications. He notes that for applications automatically approved or rejected by the model (below the human review threshold), no explanation is generated for the applicant. He asks the system administrator what happens when a customer calls to ask why their loan was rejected.

- *System Administrator:* "We tell them the decision was made by our automated system and give them a general list of factors that the system considers. We don't give them a specific reason because the model doesn't generate one."

**Technical Expert's Note:** This is a potential nonconformity against the AI Policy, which commits to "transparency in automated decisions," and potentially against applicable FCA Consumer Duty regulations (which require firms to explain automated decisions). This also relates to the SoA control on transparency that was originally excluded without justification (now included after the Stage 1 update, but apparently not yet implemented).

**Review: Training Records (11:00 - 12:30):**
Ms. Diallo reviews training records for the 12-person AI team. All 12 records are present and complete. This is a conformity.

**Audit Team Debrief (15:00 - 16:00):**
The audit team meets to consolidate findings. They agree on the following:

| Finding | Clause | Severity |
| :--- | :--- | :--- |
| CEO does not receive AI fairness performance data; management review inputs are incomplete. | 9.1, 9.3 | Minor NC |
| Quarterly fairness testing (Risk #14 control) has only been conducted once in three quarters; Q2 and Q3 reports cannot be evidenced. | 8.1, 9.1 | **Major NC** |
| CreditIQ does not generate individual explanations for automated rejection decisions, contrary to the AI Policy commitment to transparency. | 5.2, 8.1 | **Major NC** |
| The previously closed internal audit corrective action (training records) is confirmed as resolved. | 10.1 | Conformity |
| The AI Impact Assessment has been updated and now reflects CreditIQ v4.0. | 6.1.3 | Conformity |

---

### Phase 4: Closing Meeting

Ms. Diallo opens the closing meeting with the CEO, CFO, and AIMS Manager present. She thanks the team for their cooperation and reiterates the sampling caveat. She presents the positive findings first, acknowledging the updated Impact Assessment and the complete training records.

She then presents the two major nonconformities. The CEO pushes back on the fairness testing finding, stating that the tests were "definitely done" and that it is just a documentation issue.

Ms. Diallo responds calmly: *"I understand your position, and I want to be clear that I am not suggesting the tests were not done. However, ISO/IEC 42001 requires that documented information be retained as evidence of the implementation of controls. Without that evidence, I cannot confirm conformity. The requirement is not just to conduct the test, but to retain the record. This is a major nonconformity because the control for your highest-rated risk cannot be verified."*

The CEO accepts the finding.

**Certification Recommendation:** Certification is withheld pending the closure of the two major nonconformities. The auditee has 90 days to submit corrective action plans and evidence of implementation.

---

### Phase 5: Follow-Up and Closure

FinGuard Analytics submits corrective action plans within 30 days:

**CAP for Major NC 1 (Fairness Testing):**
> *Root Cause: The fairness testing process was not formally assigned to a specific role with accountability. The data science team assumed it was being done by someone else. Corrective Action: A formal "AI Fairness Testing" procedure (AIMS-PROC-012) has been created, assigning the quarterly test to the Lead Data Scientist with a mandatory sign-off from the AIMS Manager. Q2 and Q3 tests have been retroactively conducted and documented. A recurring calendar reminder and management dashboard widget have been implemented to ensure visibility.*

**Ms. Diallo's Assessment:** Acceptable. The root cause (lack of ownership and accountability) is correctly identified, and the corrective action (formal procedure, assigned role, management visibility) directly addresses it.

**CAP for Major NC 2 (Transparency):**
> *Root Cause: The transparency commitment in the AI Policy was not translated into a specific operational requirement for the CreditIQ system during the policy update. Corrective Action: CreditIQ v4.1 has been developed and deployed, which generates a plain-language explanation of the top three factors influencing each automated decision. This explanation is provided to applicants via email within 24 hours of a rejection decision. Evidence: Updated system specification, sample rejection emails, and deployment log attached.*

**Ms. Diallo's Assessment:** Acceptable. The root cause (policy not operationalized) is correctly identified, and the corrective action (technical implementation of explanations) is effective and verifiable.

Ms. Diallo reviews the submitted evidence, confirms both corrective actions are implemented and effective, and closes both major nonconformities. She recommends that the Certification Body grant ISO/IEC 42001 certification to FinGuard Analytics.

---

## Case Study 2: CityGuard -- AI-Powered Predictive Policing (Public Sector)

### Organization Profile
**Organization:** CityGuard Municipal Authority
**Sector:** Public Sector (Law Enforcement Support)
**Size:** 3,200 employees
**AI System:** "PredictSafe" -- an AI system that analyzes historical crime data, social media activity, and geographic information to generate risk scores for specific neighborhoods, used by police commanders to allocate patrol resources.
**Audit Type:** Second-Party Audit (commissioned by the City Council to assess the police authority's AI governance)
**Audit Duration:** 3 days on-site

---

### Phase 1: Pre-Audit and Stage 1

The Lead Auditor, Mr. David Osei, notes immediately that this is an extremely high-risk AI system. Predictive policing tools have been widely criticized for perpetuating racial bias and for their potential to infringe on civil liberties. He assembles an audit team that includes a Technical Expert in law enforcement AI and a Legal Expert in data protection and human rights law.

**Stage 1 Key Findings:**
- The AI Policy exists but makes no reference to human rights, civil liberties, or the Equality Act 2010.
- The AI Risk Assessment identifies "potential for racial bias" as a risk but rates it as "Low Likelihood" with no supporting justification for this rating.
- No AI System Impact Assessment has been conducted. The organization states they "did not believe one was required as the system is only used for resource allocation, not individual decisions."
- The SoA excludes three Annex A controls related to human oversight and transparency, with the justification: "Operational security."

**Stage 1 Conclusion:** Mr. Osei issues a Stage 1 Report with a strong recommendation that the audit proceed, but flags the absence of an Impact Assessment as a critical gap that must be addressed. He also notes that the rating of "Low Likelihood" for racial bias risk appears to contradict substantial published research on this topic and will require detailed scrutiny during Stage 2.

---

### Phase 2: Stage 2 -- Key Audit Moments

**Interview: Police Commander (Clause 5 -- Leadership):**
- *Auditor:* "Your AI Policy does not mention human rights or civil liberties. Given that PredictSafe generates risk scores for neighborhoods, how does the organization ensure that the system does not disproportionately target communities based on race or socioeconomic status?"
- *Commander:* "Our officers are professionals. They use the scores as one input among many. The final decision is always human."
- *Auditor:* "I understand. However, research consistently shows that even when humans are 'in the loop,' they tend to defer to algorithmic recommendations, particularly under time pressure. Does your AI Policy or any operational procedure address this automation bias risk?"
- *Commander:* "Not explicitly, no."

**Technical Expert's Observation (Clause 8 -- Operation):**
The Technical Expert reviews the PredictSafe model's training data. He finds that the historical crime data used to train the model reflects arrest records, not actual crime rates. Since arrest rates are themselves influenced by historical over-policing of certain neighborhoods, the model has effectively learned to replicate and amplify historical policing patterns. This is a fundamental data quality and bias issue.

**Review of Impact Assessment (Clause 6.1.3):**
As noted in Stage 1, no Impact Assessment exists. When Mr. Osei raises this with the AIMS Manager, she states: *"We assessed the impact on our operational efficiency, but we didn't think we needed to assess the impact on the public because the system doesn't make decisions about individuals."*

Mr. Osei explains: *"ISO/IEC 42001 Clause 6.1.3 requires an assessment of the consequences of the AI system on individuals, groups of individuals, and society. A system that generates neighborhood risk scores, which then influence where police patrols are concentrated, can have profound impacts on the residents of those neighborhoods -- including increased likelihood of contact with law enforcement, potential for wrongful suspicion, and erosion of community trust. The absence of this assessment is a major nonconformity."*

---

### Phase 3: Audit Findings Summary

| Finding | Clause | Severity |
| :--- | :--- | :--- |
| No AI System Impact Assessment has been conducted for PredictSafe. | 6.1.3 | **Major NC** |
| The AI Policy contains no commitment to human rights or civil liberties protections, despite the high-risk nature of the AI system. | 5.2 | **Major NC** |
| The "Low Likelihood" rating for racial bias risk is not supported by any documented justification or evidence, contradicting substantial published research. | 6.1.2 | **Major NC** |
| Training data consists of arrest records (a proxy for historical policing patterns) rather than actual crime data. No data quality or bias assessment has been conducted on the training dataset. | 8.1 (Data Management) | **Major NC** |
| Three Annex A controls related to human oversight are excluded from the SoA with the justification "operational security," which is not a valid justification for excluding controls designed to protect individuals from harm. | 6.1.4 | Minor NC |

**Certification Recommendation:** Certification is refused at this stage due to the number and severity of major nonconformities. Mr. Osei recommends that the City Council commission a comprehensive AI Ethics Review before the organization re-applies for certification.

---

## Case Study 3: ShopSmart -- AI-Powered Recommendation Engine (Retail)

### Organization Profile
**Organization:** ShopSmart E-Commerce Ltd.
**Sector:** Retail / E-Commerce
**Size:** 450 employees
**AI System:** "RecommendAI" -- a collaborative filtering recommendation engine that suggests products to customers based on their browsing and purchase history.
**Audit Type:** Surveillance Audit (annual check to maintain existing ISO/IEC 42001 certification)
**Audit Duration:** 1 day on-site

---

### Phase 1: Pre-Audit

This is ShopSmart's first annual surveillance audit since achieving certification 12 months ago. The Lead Auditor, Ms. Priya Nair, reviews the previous audit report and notes that there were two minor nonconformities at the time of certification, both of which were closed. She plans a focused surveillance audit that checks whether the AIMS is being maintained and whether the closed nonconformities have remained closed.

She also notes from the Stage 1 document review that ShopSmart has deployed a significant new feature since the last audit: RecommendAI now includes a "Dynamic Pricing" module that adjusts product prices in real-time based on individual customer profiles. This is a material change that was not covered in the original certification scope.

---

### Phase 2: Stage 2 -- Key Audit Moments

**Interview: AIMS Manager (Clause 8.1 -- Change Management):**
- *Auditor:* "I noticed from your documentation that a Dynamic Pricing module was added to RecommendAI approximately four months ago. Can you walk me through the change management process that was followed before this feature was deployed?"
- *AIMS Manager:* "Yes, we went through our standard software development lifecycle. The engineering team tested it thoroughly."
- *Auditor:* "Did the change management process include an updated AI Risk Assessment and AI System Impact Assessment to cover the new functionality?"
- *AIMS Manager (hesitating):* "The original risk assessment and impact assessment cover RecommendAI as a whole. We didn't do a separate one for this specific feature."
- *Auditor:* "Dynamic pricing based on individual customer profiles introduces new risks that were not present in a simple recommendation engine -- for example, the risk of price discrimination against specific demographic groups, or the risk of exploiting vulnerable customers. These are materially different risks from those covered in your original assessment. Can you show me where these new risks are documented?"
- *AIMS Manager:* "They're not documented separately."

**Auditor's Note:** This is a nonconformity against Clause 8.1, which requires the organization to control planned changes and to review the consequences of changes on the AIMS. The addition of dynamic pricing is a significant change that required an updated risk and impact assessment.

**Review of Monitoring Data (Clause 9.1):**
Ms. Nair reviews the monitoring dashboards for RecommendAI. She is pleased to see that the organization has implemented robust monitoring, including customer click-through rates, conversion rates, and a new fairness metric tracking recommendation diversity across different customer demographics. This is a strong conformity and an area of best practice.

---

### Phase 3: Audit Findings Summary

| Finding | Clause | Severity |
| :--- | :--- | :--- |
| The addition of the Dynamic Pricing module to RecommendAI was not subject to an updated AI Risk Assessment or AI System Impact Assessment prior to deployment. | 8.1 | Minor NC |
| Robust post-deployment monitoring is in place, including fairness metrics. | 9.1 | Conformity (Best Practice) |
| Both previously identified nonconformities remain closed and effective. | 10.1 | Conformity |
| Management review was conducted on schedule with all required inputs. | 9.3 | Conformity |

**Certification Recommendation:** Certification is maintained. The minor nonconformity regarding the Dynamic Pricing change management must be addressed within 60 days.

---

## Key Lessons Across All Three Case Studies

Studying these three cases reveals several universal principles that every ISO/IEC 42001 Lead Auditor must internalize:

**Lesson 1 -- The AI Policy Must Be Operationalized.** In both FinGuard and CityGuard, the AI Policy contained commitments (transparency, responsible use) that were not translated into specific operational controls. An AI Policy is only as valuable as the operational procedures that implement it.

**Lesson 2 -- High-Risk AI Demands Proportionate Scrutiny.** The risk-based approach to auditing means that a predictive policing tool (CityGuard) demands far more scrutiny than a product recommendation engine (ShopSmart). The Lead Auditor must calibrate their audit intensity to the potential for harm.

**Lesson 3 -- Change Management is a Critical Control Point.** The ShopSmart case demonstrates that even a well-functioning AIMS can develop gaps when AI systems change. Every material change to an AI system must trigger a review of the risk and impact assessments.

**Lesson 4 -- Documentation is Not Optional.** In FinGuard, the fairness tests may well have been conducted. But without documentation, they do not exist from an audit perspective. "Trust me, we did it" is never acceptable as audit evidence.

**Lesson 5 -- The Auditor Must Understand the Technology.** In all three cases, the auditors' technical knowledge was essential to uncovering the most significant findings. An auditor who does not understand what training data is, or what dynamic pricing means, would have missed the most critical nonconformities.

---

*(c) 2026 International Cybersecurity and Digital Forensics Academy. All Rights Reserved.*
