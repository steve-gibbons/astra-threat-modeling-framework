# Quick Guide to ASTRA Unified Working Spreadsheet

## Purpose
The ASTRA Unified Working Spreadsheet simplifies real-time note-taking during threat modeling and security architecture reviews by capturing all observations, assumptions, risks, action items, follow-up questions, and administrative to-dos in one place.

## Meeting Logistics Tab
Captures logistical and attendee information separately:
- Meeting ID
- Date
- Time
- Attendee Names
- Roles Represented
- Meeting Format (Video, In-person, Hybrid)
- Interviewer(s)
- Additional Notes

This tab provides critical context for each session, ensuring traceability and supporting proper documentation of participants and session conditions.

## Major Groupings of the Main Tab
The Main Tab organizes assessment information into three logical groups:

| Group | Columns |
|:--|:--|
| **General** | Record ID, Summary and Details |
| **Risk** | Business Impact Area, Severity, Likelihood, Inherent Risk |
| **Remediation** | Cost, Timeline, Difficulty, Impact (Mitigation Impact) |
| **Resolve** | Residual Risk, Assigned Owner, Due Date, Status |

This structure matches the natural assessment flow: understanding the risk, evaluating remediation options, and managing resolution.

## Record Types

| Record ID Prefix | Record Type |
|:--|:--|
| O-xxx | Observation |
| A-xxx | Assumption |
| R-xxx | Risk Finding |
| AI-xxx | Critical Action Item |
| TD-xxx | Administrative To-Do |
| FU-xxx | Follow-up Question |

## Field Option Definitions

### Business Impact Area (BIA)
**Purpose:** Classify the primary business consequence if the identified risk materializes.

**Options:**
- **Financial** — Direct monetary loss (e.g., theft, fines, lost revenue).
- **Reputational** — Damage to brand, customer trust, or public image.
- **Operational** — Disruption of internal systems, services, or business operations.
- **Safety** — Harm to physical health, life, or environment.
- **Regulatory** — Violation of laws, standards, or contractual obligations.
- **Privacy** — Unauthorized access or misuse of personal or sensitive data.
- **Other** — Impact not covered above (describe in Notes).

**Note:** Security/InfoSec is intentionally not a BIA category because it represents a cause or vector, not a direct business impact. Business owners experience security failures through tangible consequences like financial loss, operational disruption, or regulatory violations.

### Severity
**Purpose:** Rate the potential seriousness of the impact if the risk materializes.

**Options:**
- **High** — Severe impact on business operations, finances, reputation, safety, or compliance.
- **Medium** — Moderate disruption, recoverable without major long-term effects.
- **Low** — Minor inconvenience or negligible business impact.

### Likelihood
**Purpose:** Estimate how likely the risk is to occur.

**Options:**
- **High** — Likely to happen within the expected operational lifecycle.
- **Medium** — Possible but not guaranteed; moderate chance.
- **Low** — Unlikely under normal conditions; rare event.

### Inherent Risk
**Purpose:** Combined pre-mitigation risk level, derived from Severity and Likelihood.

**Options:**
- **Critical** — High Severity + High Likelihood.
- **High** — High impact or high probability individually.
- **Medium** — Moderate impact and probability.
- **Low** — Low impact and/or low probability.
- **Informational** — Not a direct risk, but noteworthy.

(Determined using the Risk Matrix.)

### Cost (Remediation Group)
**Purpose:** Estimate the effort or resources required to fix the identified issue.

**Options:**
- **High** — Significant expense, new project, major investment.
- **Medium** — Manageable cost, requires planning and allocation.
- **Low** — Minimal cost, can be handled within existing budgets.

### Timeline (Remediation Group)
**Purpose:** Estimate the time needed to complete mitigation.

**Options:**
- **High** — More than 6 months.
- **Medium** — 1-6 months.
- **Low** — Less than 1 month.
- *(Or specify explicit duration if needed.)*

### Difficulty (Remediation Group)
**Purpose:** Assess the technical and organizational challenge level to fix the issue.

**Options:**
- **High** — Significant technical complexity, cross-team or leadership involvement required.
- **Medium** — Moderate technical challenge, local to project or platform team.
- **Low** — Straightforward fix, minimal friction expected.

### Impact (Remediation Group)
**Purpose:** Measure how much the proposed mitigation is expected to reduce risk.

**Options:**
- **High** — Fix will almost fully eliminate the risk.
- **Medium** — Fix will reduce but not eliminate the risk.
- **Low** — Fix will only slightly mitigate the risk.

### Residual Risk
**Purpose:** Estimate the risk level that will remain after the mitigation is applied.

**Options:**
- **High** — Substantial risk remains even after mitigation.
- **Medium** — Some manageable risk remains.
- **Low** — Minimal risk remains after mitigation.
- **Informational** — Mitigation effectively eliminates operational risk, leaving informational observations.

### Status
**Purpose:** Track the current state of the finding, action item, or assumption.

**Options:**
- **Confirm** — Needs immediate follow-up or verification.
- **Open** — Newly identified and active.
- **In Progress** — Work underway to address.
- **Closed** — Fully resolved and verified.
- **Deferred** — Deliberately postponed.
- **Promoted to Risk** — Critical action item or follow-up converted into a formal risk finding.

## How to Use
- Use the Main Tab during interviews to log observations, assumptions, risks, action items, follow-up questions, and administrative to-dos immediately.
- Use Business Impact Area, Severity, Likelihood, and Inherent Risk columns to quickly assess potential issues.
- Capture Remediation-related information (Cost, Timeline, Difficulty, Impact) when mitigation options are discussed.
- Assign owners, due dates, and statuses for tracking follow-up and closure.
- Record meeting and participant details separately in the Meeting Logistics Tab.
- Review and finalize statuses post-interview to ensure traceability and completion.

**Note**: Entries should remain clear, concise, and comprehensive to support smooth report generation.

