⚠️ Note: AURA provides AI-assisted compliance insights and does not replace certified audits or professional GRC evaluations.

# 🧠 AURA – Autonomous Unified Risk Auditor

### 🔒 AI-Powered Compliance Control Monitoring and Risk Analysis System

**AURA (Autonomous Unified Risk Auditor)** is an AI-driven compliance monitoring system designed to autonomously evaluate, analyze, and enhance ISO 27001 controls.  

Leveraging **Google Gemini**, **n8n workflow automation**, and **Google Sheets**, AURA continuously monitors compliance posture, identifies risk areas, and recommends corrective actions — turning static governance into a **living, intelligent compliance system**.

---

## 🏷️ Short Description

AURA automates compliance monitoring by using **AI reasoning** to evaluate ISO 27001 controls based on their implementation status and evidence.  
It autonomously assigns a **Risk Level (High / Medium / Low)** and suggests targeted corrective actions — directly updating your compliance sheet in real time.

---

## 💡 Overview

Manual compliance reviews are slow, repetitive, and reactive.  
AURA transforms this process into a **proactive, intelligent, and continuous auditing system**.  

Every week (or on demand), AURA:
- Reads control data from Google Sheets  
- Uses AI (Gemini) to assess risk and evidence quality  
- Outputs AI-based risk levels and corrective actions  
- Updates the compliance sheet automatically  

Essentially, AURA functions as a **digital compliance officer** — always vigilant, always improving.

---

## ⚙️ Key Features

| Feature | Description |
|----------|-------------|
| 🤖 **AI-Driven Risk Analysis** | Evaluates compliance controls using Gemini and classifies them as High, Medium, or Low risk. |
| 🔁 **Continuous Monitoring** | Scheduled audits ensure compliance data stays current. |
| 📊 **Google Sheets Integration** | Acts as both the data source and compliance dashboard. |
| 🧩 **Actionable AI Insights** | Suggests concise corrective actions for every gap identified. |
| 🧠 **Autonomous Workflow** | Built entirely using n8n — no manual intervention needed after setup. |
| 🕵️ **Audit-Ready Logs** | Easily extendable to maintain historical AI evaluation data. |
| ⚙️ **Framework-Agnostic Design** | Can expand beyond ISO 27001 to NIST, SOC 2, GDPR, etc. |

---

## 🧱 System Architecture
[Weekly Schedule Trigger]
↓
[Google Sheets → Fetch Control Data]
↓
[AI Node (Gemini) → Risk Evaluation]
↓
[Function Node → Parse & Structure Output]
↓
[Google Sheets → Update Risk + Suggested Action]

---

## 🧠 Technology Stack

| Component | Purpose |
|------------|----------|
| **n8n** | Workflow automation platform orchestrating the logic |
| **Google Gemini 2.5 / OpenAI GPT-4** | Large Language Models for compliance reasoning |
| **Google Sheets API** | Stores compliance data and AI results |
| **JavaScript (Function Nodes)** | Parses AI output and maps fields |
| **Google Apps Script / Looker Studio** | (Later) Reporting and visualization |

---

## 🧩 Workflow Logic Summary

1. **Trigger:** AURA runs weekly via n8n schedule.  
2. **Data Fetch:** Reads ISO 27001 controls from Google Sheets.  
3. **Filtering:** Selects partially implemented or non-implemented controls.  
4. **AI Analysis:**  
   - AI evaluates evidence, status, and control intent.  
   - Generates risk level and short corrective action.  
5. **Parsing & Structuring:** Converts Gemini output to structured JSON.  
6. **Updating:** Writes back results to the same Google Sheet.
   
---

## 🎯 Impact

- ⏱️ **80% reduction** in manual compliance effort  
- 📈 **Continuous monitoring** ensures real-time compliance visibility  
- 🧠 **AI-driven reasoning** standardizes risk evaluations  
- 🧾 **Audit readiness** through automation and version tracking  

---

## 🔮 Future Enhancements

| Stage | Feature |
|--------|----------|
| 2️⃣ | Dynamic dashboards (Looker Studio / Power BI). |
| 3️⃣ | Slack or email alerts for high-risk controls. |
| 4️⃣ | Multi-framework integration (ISO 27001, NIST, SOC 2, GDPR). |
| 5️⃣ | Historical log sheet for change tracking and audit trails. |
| 6️⃣ | AI Explainability field (“Reason for Risk Level”). |
| 7️⃣ | Web-based GRC dashboard (Flask / Next.js). |

---

## 🧩 Add-Ons & Integrations

- 🧾 **Auto-generated weekly PDF reports** for management.  
- 📧 **Email summaries** of latest compliance health.  
- 🔔 **Slack alerts** for urgent high-risk findings.  
- 🧠 **Feedback loop** for human validation and AI retraining.  
- 🧩 **Ticketing integration** with Jira or ServiceNow.  

---

## 🧑‍💻 Author

**Anamay Mishra**  
Cybersecurity Researcher 

---

## 📜 License

Open for educational and portfolio use.  
For commercial adaptation, please attribute to the author.

---

# Disclaimer

AURA (Autonomous Unified Risk Auditor) is an AI-powered compliance assistant designed to support governance, risk, and compliance (GRC) professionals by automating control monitoring, risk identification, and evidence analysis.

This system provides AI-based insights and risk assessments to assist in maintaining compliance posture.
However:

It does not constitute a formal compliance audit.

It does not guarantee full conformity with ISO 27001 or any other standard.

Human verification and certified audits are still required to ensure official compliance certification.

The recommendations generated by AURA should be treated as decision-support tools, not definitive compliance verdicts.
Organizations should engage qualified auditors or compliance officers for official assessments, certifications, and final risk validation.
