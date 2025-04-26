# Quick Guide to ASTRA Unified Working Spreadsheet

## Purpose
The ASTRA Unified Working Spreadsheet simplifies real-time note-taking during threat modeling and security architecture reviews by capturing all observations, assumptions, risks, action items, follow-up questions, and administrative to-dos in one place.

## Spreadsheet Structure

### Main Records Tab

| Record ID Prefix | Record Type |
|:----------------|:------------|
| O-xxx | Observation |
| A-xxx | Assumption |
| R-xxx | Risk Finding |
| AI-xxx | Critical Action Item |
| TD-xxx | Administrative To-Do |
| FU-xxx | Follow-up Question |

### Columns in the Main Records Tab

- **Record ID**: Unique identifier for each entry based on record type prefix.
- **Summary and Details**: Enter all relevant notes, details, context, or clarifications in this single narrative field.
- **Category**: Select from InfoSec, Privacy, Operational, or Other.
- **Severity**: Critical, High, Medium, Low, or N/A (primarily for Risk Findings).
- **Likelihood**: High, Medium, Low, or N/A (primarily for Risk Findings).
- **To Repair: Cost**: High, Medium, Low, or N/A.
- **To Repair: Timeline**: Enter estimated time required or mark N/A.
- **To Repair: Difficulty**: High, Moderate, Low, or N/A.
- **Residual Risk**: High, Medium, Low, or N/A.
- **Assigned Owner**: Specify the responsible person or role.
- **Due Date**: Target completion date.
- **Status**:
  - **Confirm**: Needs immediate follow-up or verification (especially for Observations, Assumptions, and Follow-up Questions).
  - **Open**: Item identified and actively tracked.
  - **In Progress**: Work or clarification actively underway.
  - **Closed**: Completed or resolved.
  - **Deferred**: Postponed intentionally.
  - **Promoted to Risk**: Follow-up or Action escalated to a formal Risk Finding.

### Meeting Demographics Tab

Captures logistical and attendee information separately:
- Meeting ID
- Date
- Time
- Attendee Names
- Roles Represented
- Meeting Format (Video, In-person, Hybrid)
- Interviewer(s)
- Additional Notes

## How to Use
- Use the Main Records Tab during interviews to log observations, assumptions, risks, action items, follow-up questions, and administrative to-dos immediately.
- Update statuses and assigned owners actively during and after the session.
- Use the Meeting Demographics Tab to record participant and logistical details at the beginning of each interview.
- Review and finalize statuses post-interview to ensure traceability and closure.

**Note**: Keep entries clear, concise, and comprehensive for efficient follow-up and final reporting.

