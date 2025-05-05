# Understanding Risk Findings vs. Critical Action Items in ASTRA

---

## Risk Findings

- **What They Are**:  
  Documented risks identified through system analysis, interviews, or observation.

- **Record Prefix**: `R-xxx`

- **RCID Required**: Each Risk Finding must be tagged with a Risk Context & Impact Domain (RCID) that describes the nature and consequence of the risk.

- **What They Show**:  
  Severity, Likelihood, Inherent Risk, Feasibility to Repair, Expected Residual Risk after fixes.

- **Purpose**:  
  Prioritize remediation efforts based on business impact and repair feasibility.

---

## Critical Action Items

- **What They Are**:  
  Urgent missing information, documentation gaps, or decisions needed to complete the security review.

- **Record Prefix**: `AI-xxx`

- **RCID Requirement**: RCID is required if the item escalates into a Risk Finding. Optional otherwise.

- **Severity**:  
  - **Critical** — Blocks risk evaluation or report delivery.
  - **Administrative** — Minor clean-up or enhancement (non-blocking).

- **What Happens if Unresolved**:  
  Critical Action Items escalate into Critical Risk Findings in the final report.

- **Purpose**:  
  Ensure complete and accurate threat modeling and architecture assessment.

---

## Why ASTRA Separates Them

| Category | Purpose |
|:--|:--|
| **Risk Findings** | Address real-world vulnerabilities and weaknesses directly. |
| **Critical Action Items** | Address missing information needed to complete evaluation accurately. |

---

## Visual Flow

**Discovery Phase:**

- Finding risk directly → Becomes a **Risk Finding** (`R-xxx`)  
  - Must include RCID categorization
- Finding missing information → Becomes a **Critical Action Item** (`AI-xxx`)  
  - If resolved → Normal reporting  
  - If unresolved → Escalates into a **Critical Risk Finding** with full RCID tagging

---
