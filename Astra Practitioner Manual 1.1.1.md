# ASTRA Threat Modeling and Security Architecture Review Framework

# ASTRA Practitioner’s Manual (Version 1.1.1)

---

## Personal Note and Dedication

ASTRA is dedicated to **Karen**, my fiancée, who continues to inspire me to seek the light, to fight the Dark Side, and to believe that clarity, collaboration, and resilience are forces for good — in both life and work.

This project is my way of giving back to the professional community I've been privileged to be part of — offering not just a tool, but the benefit of lessons learned over decades of real-world experience.

It is also a personal statement: in a time of economic uncertainty, layoffs, and shifting priorities, I choose to build. I choose to share. I choose to lead with integrity and clarity.

ASTRA is meant for practitioners who believe that security and governance are not mere compliance checklists — they are missions. They are responsibilities.

Thank you for taking the time to explore ASTRA. May you find it useful, practical, and — most importantly — a tool for doing good.

— **Steve Gibbons**

---

## 1. Philosophy and Background

ASTRA was developed from over 25 years of hands-on experience with governance, risk management, security architecture review, and third-party evaluation across highly regulated, large-scale enterprise environments.

Its design reflects lessons learned while leading critical evaluation and governance initiatives at organizations such as Wells Fargo, American Express, Ameriprise Financial, and IBM. These experiences included:

- Reviewing internal development and third-party services.
- Supporting vendor onboarding, mergers and acquisitions (M&A) due diligence.
- Responding to regulatory and audit requirements.
- Driving modernization projects while maintaining resilience.

### Core Principles Behind ASTRA

- **Governance Must Align to Reality**
- **Third-Party Risk Cannot Be an Afterthought**
- **Architecture Reviews Must Prioritize Actionable Findings**
- **Collaboration Outperforms Confrontation**
- **Simplicity Eliminates Friction**
- **Flexibility is Key to Scalability**

---

## 2. Introduction

**ASTRA** (Architecture and Security Threat Review and Analysis) is a collaborative, business-driven methodology for security architecture review and threat modeling.

ASTRA is designed to:
- Align security analysis with real-world business context.
- Improve architecture understanding through structured interviews and artifact reviews.
- Identify risks, prioritize mitigations, and strengthen security postures.
- Deliver professional, actionable recommendations — **not audits**.

---

## 3. ASTRA Process Overview

| Phase | Purpose |
|:--|:--|
| **Align** | Understand business context and goals. Gather usage assumptions and constraints. |
| **Study** | Review technical design, architecture diagrams, data flows, and other artifacts. |
| **Target** | Plan key risk areas to investigate and structure interview questions accordingly. |
| **Review** | Conduct structured, collaborative interviews with SMEs and stakeholders. |
| **Analyze** | Consolidate findings, prioritize risks, recommend mitigations, and finalize deliverables. |

---

## 4. Work Products (Intermediary and Final)

| Work Product | Purpose |
|:--|:--|
| Business Context Questionnaire | Document client usage and business assumptions. |
| Technical Architecture Questionnaire | Capture system design, boundaries, components. |
| Emerging Risks Questionnaire | Supplemental tool for new technologies and evolving risks. |
| Unified Working Spreadsheet | Consolidated capture of observations, assumptions, risks, action items, follow-ups, and to-dos. |
| Risk Findings Table | **View of Unified Working Spreadsheet** filtered to show risk findings. |
| Critical Action Items Table | **View of Unified Working Spreadsheet** filtered to show urgent, blocking gaps. |
| Administrative To-Do Log | **View of Unified Working Spreadsheet** for minor documentation and enhancements. |
| Final Risk and Recommendations Report | Standalone or generated view summarizing prioritized risks and actions. |
| Client-Facing Guide | Optional onboarding guide explaining ASTRA's structure and expectations. |

---

## 5. Interview and Discovery Process

- **Group Interviews Supported**: Multiple SMEs, architects, and business owners may attend.
- **Attendance Mode Tracked**: In-person, video, or hybrid format recorded in Meeting Logistics.
- **Attribution Tracked**: Assign clarifications, assumptions, or discoveries to individuals where possible.
- **Gap Owners Assigned**: Each Critical Action Item must have an assigned owner.
- **Collaborative Tone**: Interviews are collaborative, discovery-driven, and improvement-focused — **never adversarial**.

### Meeting Logistics Tab
Captures:
- Meeting ID, Date, Time
- Attendee Names and Roles
- Meeting Format (Video, In-person, Hybrid)
- Interviewer Name(s)
- Session Notes

### Main Tab Major Groupings

| Group | Columns |
|:--|:--|
| **General** | Record ID, Summary and Details |
| **Risk** | Business Impact Area, Severity, Likelihood, Inherent Risk |
| **Remediation** | Cost, Timeline, Difficulty, Mitigation Impact |
| **Resolve** | Residual Risk, Assigned Owner, Due Date, Status |

### Record Types

| Record ID Prefix | Record Type |
|:--|:--|
| O-xxx | Observation |
| A-xxx | Assumption |
| R-xxx | Risk Finding |
| AI-xxx | Critical Action Item |
| TD-xxx | Administrative To-Do |
| FU-xxx | Follow-up Question |

---

## 6. Field Option Definitions

(included fully — identical to previous update)


### Business Impact Areas (BIAs)

ASTRA focuses on tangible business consequences rather than internal functions. Below is the current taxonomy of supported Business Impact Areas (BIAs). These are used during assessment to describe the **potential organizational harm** if a risk were to materialize.

| **Business Impact Area**          | **Description** |
|:----------------------------------|:----------------|
| **Customer Safety / Human Harm**  | Risks that could result in physical injury, harm, or adverse health outcomes to users or the public. |
| **Privacy / PII / PHI**           | Loss, misuse, or unauthorized access to personal data, including health information or privacy breaches. |
| **Financial Loss**                | Direct or indirect monetary impact, including fraud, theft, penalties, or loss of revenue. |
| **Reputation / Trust**            | Harm to brand reputation, public trust, customer loyalty, or media exposure. |
| **Regulatory / Legal Exposure**   | Violations of laws, contracts, or regulatory frameworks; includes audit failures or lawsuits. |
| **Service Continuity / Availability** | Downtime, outages, or disruption of core services that affect customers or operations. |
| **Data Integrity / Quality**      | Loss of data accuracy, corruption, or tampering, undermining business or technical decisions. |
| **Unauthorized Access / Misuse**  | Breaches of access control, over-permissioning, or misuse of legitimate access. |
| **Internal Misuse / Insider Threat** | Accidental or malicious misuse of systems by employees, contractors, or partners. |
| **Supply Chain / Vendor Impact**  | Risks introduced through third-party software, services, or contractual dependencies. |
| **Innovation / Product Roadmap**  | Delays or derailment of product strategy, feature development, or technology adoption. |
| **Strategic or Mission Disruption** | Interference with long-term goals, market competitiveness, or organizational priorities. |

> **Note:**  
> *Security* itself is intentionally **not** a Business Impact Area.  
> Security is a safeguard mechanism — the BIAs represent the actual consequences when those safeguards fail.

| **ASTRA BIA**                      | **ASTRA Description**                                                                                      | **NIST/FIPS 199**         | **ISO 27005**                    | **FAIR**                          | **HITRUST/HIPAA**                  |
|-----------------------------------|------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------|-----------------------------------|------------------------------------|
| **Customer Safety / Human Harm**  | Risk of physical harm, injury, or adverse health outcomes affecting users, employees, or the public.      | *(Not defined)*            | Personal safety (optional)       | *(Not explicit)*                  | Patient Safety, Device Failure     |
| **Privacy / PII / PHI**           | Unauthorized access, use, or exposure of personally identifiable or health-related information.            | Confidentiality            | Personal Data Disclosure         | Privacy Violations                | PHI Disclosure                     |
| **Financial Loss**                | Direct or indirect monetary damage, including theft, fraud, fines, penalties, or lost revenue.             | *(Not explicit)*           | Asset Value, Fraud               | Fines, Response/Replacement Cost  | Financial Penalties, Cost of Breach|
| **Reputation / Trust**            | Damage to organizational reputation, public perception, or customer confidence.                            | *(Not explicit)*           | Reputational Impact              | Reputation Damage                 | Loss of Public Trust               |
| **Regulatory / Legal Exposure**   | Legal consequences due to regulatory non-compliance, contract violations, or lawsuits.                     | *(Implied under CIA)*      | Legal Obligations, Compliance    | Fines & Judgments                 | Audit Failure, Civil Penalties     |
| **Service Continuity / Availability** | Disruption or downtime of services that impact users, customers, or internal operations.              | Availability               | Operational Disruption           | Productivity Loss                 | Downtime, System Unavailability    |
| **Data Integrity / Quality**      | Compromised accuracy, completeness, or consistency of critical business or operational data.               | Integrity                  | Data Corruption                  | Loss of Integrity                 | Clinical Decision Risk             |
| **Unauthorized Access / Misuse**  | Improper or excessive access to systems, data, or privileges—whether accidental or malicious.              | Confidentiality            | Misuse or Abuse of Privileges    | Primary Loss Event, Loss Frequency| Improper Access                    |
| **Internal Misuse / Insider Threat** | Harm caused by employees, contractors, or trusted partners through error or malicious actions.          | *(Not explicit)*           | Insider Misuse                   | Secondary Loss Event              | Workforce Misuse                   |
| **Supply Chain / Vendor Impact**  | Risk originating from third-party software, platforms, service providers, or suppliers.                    | *(Not explicit)*           | Third-Party Dependency Risk      | External Dependencies             | Third-Party Service Providers      |
| **Innovation / Product Roadmap**  | Disruption to planned innovation, R&D efforts, or key product and feature rollouts.                        | *(Not defined)*            | Business Strategy Impact         | Competitive Advantage Loss        | R&D Delay, Innovation Risk         |
| **Strategic or Mission Disruption** | Risk to high-level business strategy, market position, or organizational mission.                        | *(Not defined)*            | Strategic Objectives Impact      | Strategic Risk                    | Business Continuity Disruption     |

---

## 7. Findings, Action Items, Assumptions, Follow-Ups

| Record ID Prefix | Record Type | Purpose |
|:--|:--|:--|
| O-xxx | Observation | General system or process observations. |
| A-xxx | Assumption | Conditions or usage expectations not confirmed. |
| R-xxx | Risk Finding | Discovered threat or vulnerability. |
| AI-xxx | Critical Action Item | Missing information or immediate resolution gap. |
| TD-xxx | Administrative To-Do | Documentation or minor clean-up. |
| FU-xxx | Follow-up Question | Clarifications to verify with stakeholders. |

- Action Items must be resolved or escalated to formal risks.
- Observations and Assumptions often start with status "Confirm."

---

## 8. Risk Prioritization and Scoring

| Element | Definition |
|:--|:--|
| Severity | Potential business impact if realized. |
| Likelihood | Chance of occurrence. |
| Inherent Risk | Pre-mitigation combined risk. |
| Cost | Estimated financial/resource effort to remediate. |
| Timeline | Estimated time to complete remediation. |
| Difficulty | Technical/organizational remediation difficulty. |
| Mitigation Impact | Estimated effectiveness of repair. |
| Residual Risk | Post-mitigation remaining risk. |

### Risk Matrix

| **Severity / Likelihood** | **Low**     | **Medium**  | **High**      |
|---------------------------|-------------|-------------|----------------|
| **Low**                   | Minimal     | Low         | Medium         |
| **Medium**                | Low         | Medium      | High           |
| **High**                  | Medium      | High        | Critical       |
| **Critical**              | High        | Critical    | Showstopper    |

---

### Risk Rating Levels

| **Category**     | **Level** | **Description**                                                                                                                                       | **Response Guidance**                         | **Default Treatment Timeframe**        |
|------------------|-----------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|----------------------------------------|
| **Minimal**       | 0         | No meaningful risk or impact. Observations or notes that require no action but are logged for awareness or traceability.                            | Log only; no action required                  | None                                   |
| **Low**           | 1         | Minimal impact and low likelihood. Minor issues that are unlikely to cause harm. May be addressed during routine reviews.                          | Accept or defer; track optionally             | Next review cycle (e.g., quarterly)    |
| **Medium**        | 2         | Moderate impact or likelihood. Could cause inefficiencies, non-critical failures, or minor compliance issues.                                       | Mitigate or monitor                           | Within 30–90 days                      |
| **High**          | 3         | Significant impact or likelihood. May result in data exposure, downtime, or reputational harm.                                                     | Prompt mitigation required                    | Within 30 days                         |
| **Critical**      | 4         | Severe risk with high likelihood or impact. Could result in legal violations, major outages, or serious financial harm.                            | Immediate remediation or escalation           | Within 7 days                          |
| **Showstopper**   | 5         | Unacceptable and systemic risk. Immediate danger to operations, safety, or compliance.                                                              | Executive intervention required               | Immediate (24–48 hours max)            |
---

### Risk Treatment Strategies

ASTRA supports tagging each risk with a high-level treatment strategy to clarify intent and support structured decision-making. Optional subcategories are included parenthetically.

| **Treatment Strategy** | **Description** |
|------------------------|-----------------|
| **Avoid**              | Eliminate the source of the risk entirely (e.g., remove the feature, cancel the project). |
| **Mitigate (Reduce Likelihood)** | Apply controls to lower the chance of occurrence (e.g., hardening, access controls). |
| **Mitigate (Reduce Impact)**     | Reduce the consequences if the risk occurs (e.g., failover, backups). |
| **Mitigate (Partial + Accept Residual)** | Address what’s feasible, formally accept the remaining residual risk. |
| **Accept**             | Acknowledge the risk and take no immediate action (e.g., low-priority, business-justified). |
| **Transfer (Insurance)** | Use cyber insurance or similar financial instruments to offset potential losses. |
| **Transfer (Contractual)** | Shift responsibility to another party through SLAs or third-party agreements. |
| **Monitor Only**       | Track the risk with no current action planned, often due to uncertainty or emerging nature. |
| **Escalate**           | Forward the risk to governance or leadership for review, funding, or executive decision. |
| **Defer**              | Temporarily delay treatment, pending redesign or further analysis. |
| **Retire**             | Risk no longer applies (e.g., system decommissioned or dependency removed). |

> Use the `Risk Treatment Strategy` column in the ASTRA tracker to capture one of the options above. Additional notes can be added in a `Treatment Notes` field if needed.

## 9. Status Definitions


Each record in the unified working spreadsheet must include a `Status` to track its current state. The following values are supported across all record types:

| **Status**            | **Meaning** |
|:----------------------|:------------|
| **Confirm**           | Item requires clarification, confirmation, or follow-up to determine relevance or accuracy. Common for observations and assumptions. |
| **Open**              | Actively tracked — relevant and accepted into the working set for further action, review, or resolution. |
| **In Progress**       | Work is actively underway by the responsible owner or team. |
| **Closed**            | Fully resolved — no further action required. Applies to all record types. |
| **Deferred**          | Intentionally postponed. Still relevant, but not being addressed during the current review or cycle. |
| **Promoted to Risk**  | Used when a follow-up or action item has escalated into a full Risk Finding due to missed deadlines or newly identified impact. Triggers creation of a new `R-xxx` record.

> **Note:** Status values are required for all entries in the unified spreadsheet. Default status for Observations and Assumptions is typically **Confirm**.

---

## 10. Escalation Rules

| Scenario | Escalation Outcome |
|:--|:--|
| Critical Action Item unresolved | Escalated to Critical Risk Finding. |
| Administrative To-Do still open | Non-blocking; logged but does not prevent reporting. |

---

## 11. Visual Flows

### Interview and Discovery Flow
```
Discovery →
    - Observation Identified → Observation
    - Assumption Identified → Assumption
    - Follow-Up Identified → Follow-up Question
    - Risk Identified → Risk Finding
    - Missing Info Identified → Critical Action Item
        - If Resolved → No Impact
        - If Unresolved → Becomes Risk Finding
```

### Risk Assessment Flow
```
Severity Estimated
Likelihood Estimated
 ↓
Inherent Risk Calculated
 ↓
Cost/Timeline/Difficulty Estimated
 ↓
Mitigation Impact Estimated
 ↓
Residual Risk Estimated
 ↓
Risk Prioritized
```

---

## 12. Client Communication Philosophy

- ASTRA is **not an audit**.
- Emphasize **learning and discovery**.
- Engage stakeholders collaboratively.
- Frame findings as **improvements** and **risk maturity wins**.

---

## 13. Licensing and Use

- Published under **Creative Commons Attribution 4.0 International (CC BY 4.0)** License.
- Proper attribution required.

> "ASTRA Threat Modeling and Security Architecture Review Framework, developed by Steve Gibbons."

---

## Appendix: Provided Templates

- Unified Working Spreadsheet Template
- Business Context Questionnaire Template
- Technical Architecture Questionnaire Template
- Quick Guide to Spreadsheet Usage

---

# End of ASTRA v1.1.1 Practitioner’s Manual

