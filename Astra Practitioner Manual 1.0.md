# ASTRA Threat Modeling and Security Architecture Review Framework

# ASTRA Practitioner’s Manual (Version 1.1)

---

## Personal Note and Dedication

ASTRA is dedicated to **Karen**, my fiancée, who continues to inspire me to seek the light, to fight the Dark Side, and to believe that clarity, collaboration, and resilience are forces for good — in both life and work.

This project is my way of giving back to the professional community I've been privileged to be part of — offering not just a tool, but the benefit of lessons learned over decades of real-world experience.

It is also a personal statement: in a time of economic uncertainty, layoffs, and shifting priorities, I choose to build. I choose to share. I choose to lead with integrity and clarity.

ASTRA is meant for practitioners who believe that security and governance are not mere compliance checklists — they are missions. They are responsibilities.

Thank you for taking the time to explore ASTRA. May you find it useful, practical, and — most importantly — a tool for doing good.

— **Steve Gibbons**

---

## 1. Introduction

**ASTRA** (Architecture and Security Threat Review and Analysis) is a collaborative, business-driven methodology for security architecture review and threat modeling.

ASTRA is designed to:
- Align security analysis with real-world business context.
- Improve architecture understanding through structured interviews and artifact reviews.
- Identify risks, prioritize mitigations, and strengthen security postures.
- Deliver professional, actionable recommendations — **not audits**.


## Philosophy and Background

ASTRA is the result of over 25 years of hands-on experience with governance, risk management, security architecture review, and third-party evaluation across highly regulated, large-scale enterprise environments.

Its development was shaped by the real-world needs encountered while leading or participating in critical evaluation and governance initiatives at Wells Fargo, American Express, Ameriprise Financial, and IBM. Across these organizations, extensive security and architecture reviews were performed on both internal developments and third-party services, including detailed risk analyses supporting vendor onboarding, mergers and acquisitions (M&A) due diligence, regulatory response efforts, and enterprise modernization projects.

ASTRA embodies several lessons learned from that frontline work:

- **Governance Must Align to Reality:**  
  Risk evaluations must focus on how technology supports business objectives, not just theoretical vulnerabilities.

- **Third-Party Risk Cannot Be an Afterthought:**  
  Understanding architectural risks, data protection practices, and operational maturity early is critical to managing vendor and M&A risks.

- **Architecture Reviews Must Prioritize Actionable Findings:**  
  Risk mitigation recommendations must be business-aligned and prioritized, not theoretical.

- **Collaboration Outperforms Confrontation:**  
  Evaluations succeed when approached as collaborative discovery and improvement efforts, not adversarial audits.

- **Flexibility is Key to Scalability:**  
  Methodologies must adapt across startups, enterprises, cloud-native, and hybrid environments.

- **Simplicity Eliminates Friction:**  
  Minimizing unnecessary complexity enables faster adoption, easier understanding, and more transparent results.

---

## 2. ASTRA Process Overview

| Phase | Purpose |
|:--|:--|
| **Align** | Understand business context and goals. Gather usage assumptions and constraints. |
| **Study** | Review technical design, architecture diagrams, data flows, and other artifacts. |
| **Target** | Plan key risk areas to investigate and structure interview questions accordingly. |
| **Review** | Conduct structured, collaborative interviews with SMEs and stakeholders. |
| **Analyze** | Consolidate findings, prioritize risks, recommend mitigations, and finalize deliverables. |

---

## 3. Work Products (Intermediary and Final)

| Work Product | Purpose |
|:--|:--|
| Business Context Questionnaire | Document client usage and business assumptions. |
| Technical Architecture Questionnaire | Capture system design, boundaries, components. |
| Unified Working Spreadsheet | Consolidated capture of observations, assumptions, risks, action items, follow-up questions, and to-dos. |
| Meeting Demographics Tab | Capture attendee names, roles, meeting format, date/time, and interviewer notes. |
| Final Risk and Recommendations Report | Primary client deliverable summarizing findings and actions. |
| Client-Facing Guide | Optional onboarding document explaining ASTRA approach. |

---

## 4. Interview Process

- **Group Interviews Supported**: Multiple SMEs, architects, and business owners may attend.
- **Attendance Mode Tracked**: In-person, video, phone — documented on the Meeting Demographics tab.
- **Attribution Tracked**: Whenever possible, attribute comments or clarifications to individual attendees.
- **Gap Owners Assigned**: Every Identified Gap must have a designated "Owner" for follow-up.
- **Collaborative Tone**: Interviews are exploratory and improvement-focused — **not confrontational or audit-driven**.

---

## 5. Findings, Action Items, To-Dos, Assumptions, and Follow-Up Questions

| Record ID Prefix | Record Type |
|:--|:--|
| O-xxx | Observation |
| A-xxx | Assumption |
| R-xxx | Risk Finding |
| AI-xxx | Critical Action Item |
| TD-xxx | Administrative To-Do |
| FU-xxx | Follow-up Question |

- **Observations** and **Assumptions** often require follow-up confirmation (status: Confirm).
- **Follow-Up Questions** (FU-xxx) are logged explicitly and tracked for closure.
- **Action Items** are reserved only for show-stopping gaps.
- **To-Dos** track non-blocking enhancements and improvements.
- **Unresolved Critical Action Items escalate into Critical Risk Findings.**

---

## 6. Risk Prioritization and Scoring

| Element | Definition |
|:--|:--|
| **Severity** | Potential business impact if risk materializes. |
| **Likelihood** | Probability that risk will materialize. |
| **Inherent Risk** | Calculated Severity x Likelihood before mitigations. |
| **To Repair: Cost** | Estimated cost to fix. |
| **To Repair: Timeline** | Estimated time to fix. |
| **To Repair: Difficulty** | Technical and organizational difficulty. |
| **Residual Risk** | Estimated risk level after recommended mitigation is applied. |

### ASTRA Risk Matrix

| Severity / Likelihood | Very Low | Low | Medium | High |
|:--|:--|:--|:--|:--|
| **Informational** | Informational | Informational | Informational | Informational |
| **Low** | Informational | Low | Medium | Medium |
| **Medium** | Low | Medium | Medium | High |
| **High** | Medium | Medium | High | Critical |
| **Critical** | High | High | Critical | Critical |

---

## 7. Status Definitions

| Status | Meaning |
|:--|:--|
| Confirm | Item requires clarification or validation. |
| Open | Item identified and actively tracked. |
| In Progress | Work actively underway. |
| Closed | Completed or resolved. |
| Deferred | Postponed intentionally. |
| Promoted to Risk | Follow-up or Action escalated to a Risk Finding. |

---

## 8. Escalation Rules

| Scenario | Escalation Outcome |
|:--|:--|
| Critical Action Item unresolved by deadline | Promoted to Critical Risk Finding in final report. |
| Administrative To-Do Item open | Tracked but does not block report or create a new finding. |

---

## 9. Visual Flows

### Interview and Discovery Flow

```
Discovery →
    - Observation Identified → Observation Record
    - Assumption Identified → Assumption Record
    - Follow-up Question Identified → FU Record
    - Risk Identified → Risk Finding Record
    - Missing Info Identified → Critical Action Item
        - If Resolved → No Impact
        - If Unresolved → Becomes Critical Risk Finding
```

### Risk Assessment Flow

```
Severity Estimated
Likelihood Estimated
 ↓
Inherent Risk Calculated
 ↓
"To Repair" Cost, Timeline, Difficulty Estimated
 ↓
Residual Risk Estimated
 ↓
Risk Prioritized
```

---

## 10. Client Communication Philosophy

- Emphasize that ASTRA is **not an audit**.
- Focus on **discovery**, **understanding**, and **shared improvement**.
- Interviews are **inquisitive** — not confrontational.
- Gaps are opportunities to **strengthen the system**, not assign blame.

---

## 11. Licensing and Use

- ASTRA is published under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** License.
- You are free to **share, adapt, and remix** the ASTRA materials with proper attribution.
- Attribution Requirement:

> "ASTRA Threat Modeling and Security Architecture Review Framework, developed by Steve Gibbons."

---

## Appendix: Provided Templates

- Unified Working Spreadsheet
- Business Context Questionnaire
- Technical Architecture Questionnaire
- Quick Guide to Unified Working Spreadsheet

---

# End of ASTRA v1.0 Practitioner’s Manual

---

