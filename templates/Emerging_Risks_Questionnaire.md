# Emerging Risks Questionnaire (ASTRA v1.1)

**Purpose:**  
This questionnaire supplements the standard ASTRA assessment when emerging technologies are detected, to help uncover associated risks, dependencies, and control gaps.

---

## AI and Machine Learning (ML)
- Are AI/ML models integrated into decision-making processes within the system?
- Is sensitive, regulated, or proprietary data used for training or operating AI/ML models?
- Is there a formal validation process for model quality, performance, and drift detection?
- Are mechanisms in place to detect bias, manipulation, or misuse of AI/ML models?
- Are any open-source or third-party AI/ML models integrated, and how are these dependencies managed?

## Large Language Models (LLMs)
- Are LLMs used to generate, summarize, or influence system functionality or business logic?
- Are LLM interactions logged, stored, or processed further, and how is sensitive data handled?
- What measures are in place to detect hallucinations, injection attacks, or prompt manipulation?
- Are external LLM APIs (e.g., OpenAI, Anthropic) utilized, and how are API security and privacy concerns addressed?

## Internet of Things (IoT)
- Are IoT devices (e.g., sensors, wearables, cameras) deployed as part of the system architecture?
- How are IoT devices segmented from critical internal systems and networks?
- Are processes in place for IoT firmware updates, security patching, and lifecycle management?
- Are IoT device inputs trusted for critical decisions, and how are they validated against spoofing or tampering?

## Blockchain and Decentralized Systems
- Is blockchain technology used to support critical business functions (e.g., transactions, identity, smart contracts)?
- Are blockchain consensus mechanisms, smart contracts, and governance models evaluated for risks?
- Are smart contracts formally audited, and are there contingency plans if vulnerabilities are discovered?

## Supply Chain and Third-Party Services
- Are critical system operations reliant on third-party SaaS, cloud services, or external APIs?
- How are vendor security, privacy, and incident response capabilities evaluated and monitored over time?
- Are there contingency or exit strategies if a critical third-party provider experiences disruption or compromise?

## Autonomous Systems and Robotics
- Are autonomous decision-making systems (e.g., robotic process automation, self-driving modules) incorporated into operations?
- What mechanisms exist to override or shut down autonomy in the event of failure or unexpected behavior?
- How are these systems protected against adversarial inputs or physical tampering?

---

# End of Emerging Risks Questionnaire (ASTRA v1.1)

