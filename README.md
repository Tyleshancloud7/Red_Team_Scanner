# 🔐 AegisRT AI: Enterprise Agentic Security & Governance Platform
<img width="1536" height="1024" alt="image0" src="https://github.com/user-attachments/assets/150bae35-1402-4408-8da8-a59438eefa31" />


## 🧠 Overview
AegisRT AI is a next-generation, full-stack security-as-a-service (SaaS) platform designed specifically for the era of Agentic AI and Large Language Models (LLMs). It serves as a comprehensive AI Security, Red Teaming, and GRC (Governance, Risk, and Compliance) command center.

The platform is engineered for SOC teams, security engineers, and enterprise AI architects who need to monitor, test, and secure AI agents and LLM integrations against emerging adversarial patterns and architectural vulnerabilities.

---

## 🎯 Purpose & Vision
AegisRT AI was built to bridge the critical gap between traditional cybersecurity and the unique, non-deterministic risks introduced by generative AI. 

### Problems Solved:
*   Traditional Security Gaps: Conventional firewalls and WAFs are blind to semantic attacks like prompt injection or goal hijacking.
*   AI/LLM Security Risks: LLMs introduce new attack vectors such as insecure output handling and sensitive data exposure through model interaction.
*   Agentic AI Risks: As AI moves from "chatbots" to "agents" with tool-use capabilities, the risk of Excessive Agency and Unauthorized Tool Execution becomes a primary threat to enterprise infrastructure.

AegisRT provides the real-world relevance needed to deploy AI agents with confidence by providing a "Defense Engine" that monitors every interaction.

---

## 🚨 Problem Statement
Current security tools are insufficient for the AI era because:
1.  Semantic Blindness: They cannot distinguish between a legitimate user request and a sophisticated prompt injection attack.
2.  Agentic Autonomy: AI agents often have access to internal APIs and tools; without a governance layer, a single compromised prompt can lead to full system compromise (RCE).
3.  Lack of Auditability: Traditional logs do not capture the "intent" or "reasoning" behind AI decisions, making forensic analysis nearly impossible.

---

## 💡 Solution Overview
AegisRT AI combines three core pillars into a single unified interface:
1.  Security Scanning: Automated red-teaming of AI prompts and agent behaviors.
2.  AI Risk Detection: Real-time analysis of intent, trust scores, and adversarial patterns.
3.  Agent Governance: A centralized inventory for authorized AI assets with strict ownership verification and audit logging.

---

## 🏗 Architecture Breakdown

### System Architecture
*   Frontend: A high-performance React 19 SPA styled with Tailwind CSS 4, utilizing Framer Motion for immersive UI transitions and Recharts for real-time risk telemetry.
*   Backend: An Express.js server providing secure API routing and serving as the orchestration layer for AI services.
*   Database: Google Firestore (NoSQL) for immutable audit logs, asset inventory, and security findings.
*   AI Orchestration: Integrated with the Gemini 3.1 Pro and Flash models via the @google/genai SDK for deep semantic analysis and report generation.

### Agent Architecture
The platform utilizes a multi-agent specialized architecture:
*   Risk Agent: Analyzes prompts in the Command Center for OWASP LLM and ASI risks.
*   Audit Agent: Monitors asset lifecycle, verification events, and compliance mapping.
*   Reporting Agent: Synthesizes complex security findings into executive-grade documentation.
*   Voice Engine Agent: Utilizes Gemini 2.5 Flash TTS to provide real-time audio alerts for critical security breaches.

---

## 🔐 Security & Safety Model
*   Authorization Enforcement: Every asset must be verified via DNS TXT records or corporate email before scanning is permitted.
*   Scope Control: The platform enforces strict boundaries on what prompts and behaviors are analyzed, preventing unauthorized testing.
*   Audit Logging: Every decision made by the AI agents is recorded in an immutable Firestore ledger, ensuring non-repudiation.
*   Safe Execution Design: AegisRT is a diagnostic and defensive platform. It identifies vulnerabilities so they can be patched, rather than providing tools for offensive exploitation.

---

## 🧠 AI Security Framework Integration

### OWASP Top 10 for LLMs
AegisRT maps every finding to the OWASP LLM framework, specifically addressing:
*   LLM01: Prompt Injection: Detecting direct and indirect injection patterns.
*   LLM02: Insecure Output Handling: Identifying risks in how agent responses are consumed.
*   LLM06: Sensitive Data Exposure: Monitoring for PII and credential leaks in prompts.
*   LLM08: Excessive Agency: Flagging prompts that attempt to escalate agent permissions.

### Agentic Security Risks (ASI01–ASI10)
The platform is a pioneer in detecting Agentic Security Issues:
*   ASI01: Goal Hijacking: Detecting when a prompt attempts to redirect an agent's primary mission.
*   ASI02: Tool Misuse: Identifying unauthorized attempts to call internal APIs or functions.
*   ASI03: Privilege Abuse: Monitoring for attempts to bypass RBAC within the AI context.
*   ASI07: Communication Risks: Analyzing multi-agent interactions for collaborative attacks.

---

## ⚙️ Features
*   Asset Onboarding + Verification: Securely register and verify ownership of AI endpoints.
*   Risk Command Center: A sandbox for testing prompts against adversarial patterns with real-time scoring.
*   Live Threat Map: A visual representation of the security posture across all organizational nodes.
*   AI-Generated Reports: One-click generation of professional security audits.
*   Real-time Audit Feed: A live stream of security events and agent decisions.

---

## 🧩 User Workflow (Step-by-Step)
1.  Authentication: Secure Google-based SSO login.
2.  Asset Registration: Add a new AI Agent or API endpoint to the inventory.
3.  Ownership Verification: Add a generated DNS TXT record to the asset's domain to prove authorization.
4.  Sandbox Testing: Use the Risk Command Center to run "Red Team" prompts against the AegisRT engine.
5.  Analysis: Review the Risk Score, Trust Score, and detailed findings mapped to OWASP/ASI.
6.  Audit Review: Check the Audit Logs to see how the system recorded the scan event.
7.  Reporting: Navigate to Security Reports to generate a formal PDF-ready document for stakeholders.

---

## 📊 Findings & Reporting
*   Severity Levels: Critical, High, Medium, Low.
*   Risk Scoring Model: A hybrid 0-100 score calculated based on intent severity and framework mapping.
*   Remediation Guidance: Every finding includes specific, actionable steps for developers to harden their AI integrations.

---

## 🖥 Technology Stack
*   Frontend: React 19, Vite, Tailwind CSS 4, Framer Motion, Recharts, Lucide React.
*   Backend: Node.js, Express.
*   Database: Google Cloud Firestore.
*   Authentication: Firebase Auth (Google SSO).
*   AI Models: Gemini 3.1 Pro (Analysis), Gemini 3.1 Flash (Reporting), Gemini 2.5 Flash (TTS).

---

## 🔍 Example Use Cases
*   Securing a Customer Service Bot: Testing if a user can trick the bot into revealing internal system prompts or customer data.
*   Auditing an AI Coding Assistant: Ensuring the assistant doesn't suggest insecure code or leak proprietary snippets.
*   Compliance Readiness: Generating a report for a SOC2 audit to prove that AI risks are being actively monitored and managed.

---

## 🛡 GRC & Compliance Alignment
AegisRT supports enterprise governance by:
*   NIST AI RMF Alignment: Mapping risks to the NIST AI Risk Management Framework.
*   SOC2/ISO 27001 Support: Providing the audit trail required for modern security certifications.
*   Automated Policy Enforcement: Ensuring that AI deployments adhere to internal security standards.

---

## 🚀 Business Value
*   Reduced Time-to-Market: Deploy AI features faster by automating the security review process.
*   Risk Mitigation: Prevent costly data breaches and brand damage resulting from AI exploits.
*   Operational Efficiency: Replace manual red-teaming with AI-driven automated scanning.

---

## 🔮 Future Enhancements
*   Automated Red-Teaming (Auto-Scan): Scheduled periodic scans of production endpoints.
*   SIEM Integration: Direct export of security events to Splunk, Sentinel, or Datadog.
*   Custom Policy Engine: Allow organizations to define their own "Forbidden Intents" and "Safety Guardrails."

---

## 📌 Conclusion
AegisRT AI represents the future of cybersecurity. As enterprises move from static software to dynamic, agentic AI systems, the need for a dedicated security layer becomes non-negotiable. AegisRT provides the visibility, governance, and protection required to lead in the AI-first world.

