# ASTRA Framework Comparison Document

---

## Overview
This document compares the ASTRA Threat Modeling and Security Architecture Review Framework against several well-known security and privacy threat modeling and risk management frameworks.

Frameworks compared:
- STRIDE (Microsoft)
- LINDDUN (Privacy Threat Modeling)
- PASTA (Process for Attack Simulation and Threat Analysis)
- NIST Risk Management Framework (RMF)

---

## Detailed Comparison

| Attribute | ASTRA | STRIDE (Microsoft) | LINDDUN (Privacy TM) | PASTA (Threat Modeling) | NIST RMF (Risk Management Framework) |
|:--|:--|:--|:--|:--|:--|
| **Primary Focus** | Lightweight security & privacy risk discovery tied to business context | Technical threat categorization for software systems | Privacy threat categorization for data flows | Full attack simulation across application threat surfaces | Formal compliance-driven risk governance |
| **Approach** | Interview-driven, real-time discovery and improvement | Model-specific threat enumeration | Privacy DFD-based threat identification | Multi-stage threat modeling with attacker-centric simulation | Highly structured formal documentation process |
| **Key Strengths** | Simplicity, adaptability, operational transparency, fast preliminary insights | Clear categories (Spoofing, Tampering, Repudiation, etc.), excellent for software developers | Focus on privacy threats often missing elsewhere | Rich multi-phase approach, attacker profiles, useful for deep app security | Regulatory alignment (FISMA, FedRAMP, DoD RMF) |
| **Pace and Complexity** | Fast, lightweight, avoids unnecessary complexity | Medium, requires DFDs and technical modeling | Medium, detailed privacy threat catalog | Slow, very detailed, simulation-intensive | Very slow, multi-year cycles common, bureaucratic burden |
| **Training Requirements** | Minimal — designed for immediate use without specialized training | Medium — requires understanding threat categories | Medium — requires learning threat trees and mappings | High — complex attack tree modeling and simulation | Very High — full training in NIST standards mandatory |
| **Typical Users** | Security architects, risk managers, technical leads, GRC professionals | Security engineers, app developers | Privacy engineers, DPOs, compliance teams | Application security engineers, architects | Risk management teams in government or highly regulated industries |
| **Business Alignment** | Strong — business context is the starting point | Weak — purely technical focus | Strong — privacy is a business driver | Moderate — attacker focus can misalign business context | Strong — mapped to regulatory and business risks |
| **Output Type** | Consolidated findings, preliminary risk snapshot, actionable plans | Threat models, DFDs with mappings | Privacy-enhanced DFDs | Threat trees, attack libraries, mitigation strategies | Formal risk reports, POA&Ms, ATO packages |
| **Use Cases** | Security architecture reviews, third-party assessments, vendor evaluations, early discovery | Threat modeling during system/software design | Privacy threat analysis | High-value application security threat simulation | Government and critical infrastructure security governance |
| **Risk Categorization Model** | RCID (Risk Context & Impact Domains) | None (implicit) | None (privacy-focused) | None (implicit) | Quantitative models (Loss Event Frequency, etc.) |

---

## Personality Snapshots

| Framework | "Personality" |
|:--|:--|
| **ASTRA** | Practical, collaborative, inquisitive, lightweight, governance-aware |
| **STRIDE** | Technical, systematic, developer-oriented |
| **LINDDUN** | Privacy-centric, DFD-focused |
| **PASTA** | Comprehensive, attacker-obsessed, heavyweight |
| **NIST RMF** | Bureaucratic, slow, regulation-focused |

---

## Summary
ASTRA provides a lightweight, business-aligned alternative that excels in early-stage discovery, third-party evaluations, and fast system assessments. While it sacrifices the extreme technical depth of PASTA or regulatory formality of NIST RMF, it offers unmatched operational simplicity, fast insight generation, and collaboration-focused execution.

ASTRA works best for:
- Security architecture and GRC assessments
- Third-party product/service evaluations
- Vendor and M&A due diligence
- Early-stage system/project threat discovery
- Organizations seeking a practical, non-bureaucratic starting point

ASTRA is also complementary to heavier frameworks, providing a discovery layer that can feed into deeper formal risk management processes as needed.

---

# Visual Comparison Matrix (Attached)

(Separate visual file: **ASTRA_Framework_Visual_Comparison.png**)

---

## RCID Update Note (v1.1.1)

ASTRA transitioned from Business Impact Areas (BIAs) to **Risk Context & Impact Domains (RCIDs)** to improve clarity and stakeholder alignment. RCIDs define both the context in which a risk arises and the domain it impacts — creating a more robust and narrative-friendly risk model.
# End of Document

