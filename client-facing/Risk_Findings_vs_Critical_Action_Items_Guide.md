# Understanding Risk Findings vs. Critical Action Items in ASTRA

---

## Risk Findings

- **What They Are**:  
  Documented risks identified through system analysis, interviews, or observation.

- **What They Show**:  
  Severity, Likelihood, Inherent Risk, Feasibility to Repair, Expected Residual Risk after fixes.

- **Purpose**:  
  Prioritize remediation efforts based on business impact and repair feasibility.

---

## Critical Action Items

- **What They Are**:  
  Urgent missing information, documentation gaps, or decisions needed to complete the security review.

- **Severity**:  
  - **Critical** — Blocks risk evaluation or report delivery.
  - **Administrative** — Minor clean-up or enhancement (non-blocking).

- **What Happens if Unresolved**:  
  - Critical Action Items escalate into Critical Risk Findings in the final report.

- **Purpose**:  
  Ensure complete and accurate threat modeling and architecture assessment.

---

## Why ASTRA Separates Them

| Category | Purpose |
|:--|:--|
| **Risk Findings** | Address real-world vulnerabilities and weaknesses directly. |
| **Critical Action Items** | Address missing pieces needed to complete evaluation accurately. |

---

## Visual Flow
Discovery →
↳ Finding Risk Directly → Risk Finding
↳ Missing Information → Critical Action Item
↳ If Resolved → Normal reporting
↳ If Not Resolved → Escalates into Critical Risk
