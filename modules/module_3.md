# ISO/IEC 42001 Lead Auditor Training Course: The Complete Guide

## Module 3: Planning and Risk Management in AIMS

### Learning Objectives
By the end of this module, you will be able to:
1. Understand the core requirements for planning the AIMS as outlined in Clause 6.
2. Clearly differentiate between AI Risk Assessment and AI System Impact Assessment.
3. Describe and apply a robust methodology for conducting an AI Risk Assessment.
4. Explain how to formulate an AI Risk Treatment Plan and select appropriate controls.
5. Understand the critical role of the Statement of Applicability (SoA).
6. Establish AI system objectives and develop actionable plans to achieve them.

### 3.1 Planning for the AIMS (Clause 6): The Engine Room
Clause 6 is the engine room of the AIMS. It is where the organization takes the understanding gained in Clause 4 (Context) and the commitment established in Clause 5 (Leadership) and turns them into a concrete, actionable strategy. The organization must determine the risks and opportunities that need to be addressed to ensure the AIMS can achieve its intended outcomes, prevent or reduce undesired effects, and achieve continual improvement [1].

Planning in ISO/IEC 42001 is not a theoretical exercise. It requires the organization to explicitly determine:
- **What** will be done to address risks and opportunities.
- **What resources** will be required.
- **Who** will be responsible for executing the plan.
- **When** the actions will be completed.
- **How** the results of these actions will be evaluated for effectiveness.

This proactive approach ensures that AI governance is integrated into the organization's strategic planning and operational realities, rather than being treated as a separate, isolated compliance task.

### 3.2 AI Risk Assessment Methodology: A Structured Approach
A central, non-negotiable requirement of ISO/IEC 42001 is the implementation of a formalized approach to AI risk management. The standard requires organizations to define and apply an AI risk assessment process that establishes and maintains AI risk criteria (including risk acceptance criteria) and ensures that repeated assessments produce consistent, valid, and comparable results [2].

The AI risk assessment process must be systematic and typically involves three distinct steps:

#### 3.2.1 Risk Identification
This is the process of finding, recognizing, and describing risks associated with the development, provision, or use of AI systems that could result in negative consequences. The organization must identify:
- **Sources of risk:** Where is the risk coming from? (e.g., poor quality training data, a vulnerable open-source library, a flawed algorithm).
- **Potential events:** What could happen? (e.g., the system outputs biased decisions, the system is hacked, the system degrades over time).
- **Causes and potential consequences:** Why would this happen, and what is the business impact?

#### 3.2.2 Risk Analysis
Once identified, the organization must comprehend the nature of the AI risks and determine the level of risk. This involves assessing two key factors:
1. **Consequences:** What is the severity of the impact if the event occurs? (e.g., minor financial loss vs. severe reputational damage or legal action).
2. **Likelihood:** What is the probability that the event will occur?

The combination of consequence and likelihood determines the overall level of risk.

#### 3.2.3 Risk Evaluation
Risk evaluation involves comparing the results of the risk analysis (the level of risk) with the established risk criteria to determine whether the risk and/or its magnitude is acceptable or tolerable. If a risk exceeds the organization's risk appetite, it must be treated.

| Risk Category | Example Scenario | Potential Consequences |
| :--- | :--- | :--- |
| **Technical/Security** | An attacker uses prompt injection to bypass a generative AI's safety filters, causing it to output malicious code. | System compromise, data breach, severe reputational damage. |
| **Ethical/Fairness** | An AI resume screening tool is trained on historical data that favors male applicants, leading to systemic bias. | Discrimination lawsuits, regulatory fines, loss of public trust. |
| **Operational/Performance** | "Concept drift" occurs when an AI fraud detection model degrades over time because consumer purchasing habits change. | Increased financial losses due to undetected fraud, operational inefficiency. |

### 3.3 AI System Impact Assessment: Beyond the Organization
While traditional risk assessment often focuses on technical and operational risks to the organization itself, ISO/IEC 42001 introduces a crucial specific requirement: the AI System Impact Assessment. This assessment shifts the focus outward, evaluating the potential consequences of the AI system on individuals, groups of individuals, and society at large [2].

An AI Impact Assessment must consider factors such as:
- **Human Rights:** Does the system potentially infringe on fundamental freedoms or privacy?
- **Fairness and Discrimination:** Could the system lead to unfair treatment or exclusion of specific demographic groups?
- **Societal Impact:** Does the system have the potential to spread misinformation, manipulate public opinion, or cause environmental harm?

The results of the impact assessment are not standalone; they must feed directly into the overall AI risk assessment and risk treatment processes. A risk that has a low financial impact on the company but a high negative impact on society must be addressed.

### 3.4 AI Risk Treatment and the Statement of Applicability (SoA)
Once risks have been evaluated and deemed unacceptable, the organization must define and apply an AI risk treatment process. This involves selecting appropriate AI risk treatment options:
- **Avoid the risk:** Decide not to start or continue with the AI project.
- **Mitigate the risk:** Implement controls to reduce the likelihood or consequence.
- **Transfer the risk:** Share the risk with another party (e.g., through insurance or outsourcing).
- **Accept the risk:** Make an informed decision to retain the risk by choice.

If the decision is to mitigate the risk, the organization must determine all controls that are necessary to implement the chosen risk treatment options.

#### The Role of Annex A and the SoA
ISO/IEC 42001 provides Annex A, which contains a comprehensive set of reference control objectives and controls specifically designed for AI systems. The organization must compare the controls it has determined necessary with those in Annex A to verify that no necessary controls have been omitted.

Finally, the organization must produce a Statement of Applicability (SoA). The SoA is a critical audit document. It must contain:
1. The necessary controls identified by the organization.
2. The justification for their inclusion.
3. Whether the necessary controls are implemented or not.
4. The justification for excluding any of the controls listed in Annex A [1].

### 3.5 AI System Objectives and Planning to Achieve Them
Risk management is about preventing bad things; objectives are about achieving good things. The organization must establish AI objectives at relevant functions and levels. These objectives must be:
- Consistent with the AI policy.
- Measurable (if practicable).
- Take into account applicable requirements and the results of risk and impact assessments.
- Monitored, communicated, and updated as appropriate.

When planning how to achieve its AI objectives, the organization must determine what will be done, what resources will be required, who will be responsible, when it will be completed, and how the results will be evaluated.

### Knowledge Check and Reflection
**Question 1:** What is the primary difference between an AI Risk Assessment and an AI System Impact Assessment according to ISO/IEC 42001?
A) Risk assessments are done by IT, while impact assessments are done by HR.
B) Risk assessments focus on financial loss to the company, while impact assessments focus only on environmental damage.
C) Risk assessments focus on the effect of uncertainty on the organization's objectives, while impact assessments focus on the consequences of the AI system on individuals, groups, and society.
D) There is no difference; they are two terms for the exact same process.
*Answer: C*

**Question 2:** If an organization decides that a specific control listed in Annex A is not relevant to their AI system, what must they do?
A) They cannot exclude any controls from Annex A; it is mandatory to implement all of them.
B) They must document the exclusion and provide a justification for it in the Statement of Applicability (SoA).
C) They must ask the ISO committee for permission to exclude it.
D) They can simply ignore it without documenting anything.
*Answer: B*

**Reflection Exercise:** Imagine you are auditing a company that has developed an AI tool to monitor employee productivity by tracking keystrokes and webcam activity. What are two specific societal or individual impacts you would expect to see addressed in their AI System Impact Assessment?

### References
[1] Scrut. Understanding ISO 42001: Key Insights and Benefits. https://www.scrut.io/post/iso-42001
[2] ISMS.online. Understanding ISO 42001 and Demonstrating Compliance. https://www.isms.online/iso-42001/
