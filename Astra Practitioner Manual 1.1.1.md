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

## 9. Status Definitions

| Status | Meaning |
|:--|:--|
| Confirm | Needs follow-up validation. |
| Open | Identified and active. |
| In Progress | Being addressed. |
| Closed | Fully resolved. |
| Deferred | Intentionally delayed. |
| Promoted to Risk | Escalated into formal risk finding. |

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

