# Technical Architecture Questionnaire (ASTRA v1.2)

**Purpose:**  
To understand the **technical design**, **architecture boundaries**, **data flows**, **dependencies**, and **security posture** of the system — without duplicating business-level context captured in the Business Context Questionnaire.

---

## System Overview

- What is the system’s name, internal reference, or service ID?
- What does the system do from a **technical perspective** (brief summary)?
- Is it built in-house, purchased, or provided by a third party?

---

## Architecture & Boundaries

- What are the **major components** of the system? *(e.g., services, databases, APIs)*
- Where are the **boundaries** of the system? *(e.g., network zones, trust zones, cloud regions)*
- What is **in scope** and what is **explicitly out of scope** for this evaluation?

---

## Key Data Flows & Interactions

- What are the **primary data flows** within the system and between external entities?
- What types of data are **ingested, processed, stored, and shared**?
- Are there any **high-risk data types** (e.g., PII, PHI, financial data)?

---

## Authentication & Access Control

- How do **internal users**, **external users**, and **systems** authenticate to the system?
- What **authorization models** are in place? *(e.g., RBAC, ABAC, custom)*
- Are there **third-party identity providers** (e.g., SSO, OIDC) involved?

---

## Dependencies & Integrations

- What **external systems, services, or vendors** does this system rely on?
- Are there **upstream or downstream dependencies** that could introduce risk?
- Are **APIs or data exchange interfaces** documented and controlled?

---

## Hosting & Network Topology

- Where is the system **hosted**? *(e.g., on-premises, public cloud, hybrid)*
- What **network zones** or **environments** (e.g., dev, test, prod) are used?
- Are there **firewalls, security groups, or segmentation** controls in place?

---

## Security Safeguards & Monitoring

- What **security controls** are already implemented? *(e.g., encryption, logging, MFA)*
- How is **logging and monitoring** performed? *(e.g., SIEM, SOC coverage)*
- Are **vulnerability management** or **penetration testing** results available?

---

## Known Architectural Assumptions or Constraints

- Are there any **documented assumptions** or **known limitations** in the system’s design?
- Are there **architecture decisions** made for business reasons that introduce known risk?

---

## Planned Technical Changes or Roadmaps

- Are there **upcoming architecture changes**, migrations, or redesigns planned?
- Are there **future features** or **technical debt** already identified?

---

## Notes

Use this questionnaire to guide technical stakeholder interviews or self-assessments. Responses can be summarized into the Unified Working Spreadsheet or attached as a standalone artifact.
