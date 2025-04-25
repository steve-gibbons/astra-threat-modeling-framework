# ASTRA Threat Modeling and Security Architecture Review Framework

# ASTRA Practitioner’s Manual (Version 1.0)

---

## 1. Introduction

**ASTRA** (Architecture and Security Threat Review and Analysis) is a collaborative, business-driven methodology for security architecture review and threat modeling.

ASTRA is designed to:
- Align security analysis with real-world business context.
- Improve architecture understanding through structured interviews and artifact reviews.
- Identify risks, prioritize mitigations, and strengthen security postures.
- Deliver professional, actionable recommendations — **not audits**.

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
| Artifact Inventory | Track gathered diagrams, documents, policies. |
| Interview Notes | Capture structured findings, gaps, owner attributions. |
| Risk Findings Table | Formal risk register with full scoring. |
| Critical Action Items Table | Track urgent missing information required to complete analysis. |
| Administrative To-Do Log | Capture non-blocking enhancements and documentation improvements. |
| Final Risk and Recommendations Report | Primary client deliverable summarizing findings and actions. |
| Client-Facing Guide | Optional onboarding document explaining ASTRA approach. |

---

## 4. Interview Process

- **Group Interviews Supported**: Multiple SMEs, architects, and business owners may attend.
- **Attendance Mode Tracked**: In-person, video, phone — track per attendee.
- **Attribution Tracked**: Whenever possible, attribute comments or clarifications to individual attendees.
- **Gap Owners Assigned**: Every Identified Gap must have a designated "Owner" for follow-up.
- **Collaborative Tone**: Interviews are exploratory and improvement-focused — **not confrontational or audit-driven**.

---

## 5. Findings vs. Action Items

| Category | Purpose |
|:--|:--|
| **Risk Findings** | Risks discovered during review that affect system security, privacy, or resilience. |
| **Critical Action Items** | Missing information that blocks the ability to accurately complete risk analysis. |

- Critical Action Items are either **Critical** (blocking) or **Administrative** (non-blocking).
- Unresolved Critical Action Items **escalate into Critical Risk Findings** in the final report.

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

## 7. Action Item Management

- Action Items are reserved only for **show-stopping gaps**.
- All Critical Action Items must be:
  - Assigned to an owner
  - Given a deadline
  - Tracked until resolved

### Resolution Policy
- **No final report may be issued while Critical Action Items remain unresolved.**
- **Missed deadlines promote the item to a Critical Risk Finding.**

Administrative To-Do Items (documentation, minor follow-ups) are tracked separately and do not block report delivery.

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
    - Risk Identified → Risk Finding
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
- Gaps are opportunities to **strengthen the system**, not blame.

---

## 11. Licensing and Use

- ASTRA is published under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** License.
- You are free to **share, adapt, and remix** the ASTRA materials with proper attribution.
- Attribution Requirement:

> "ASTRA Threat Modeling and Security Architecture Review Framework, developed by Steve Gibbons."

---

## Appendix: Provided Templates

- Interview Notes Template
- Risk Findings Table Template
- Critical Action Items Table Template
- Administrative To-Do Log
- Risk Matrix Chart
- Sample Filled Risk Tables
- Client-Facing Guides

---

# End of ASTRA v1.0 Practitioner's Manual

---
