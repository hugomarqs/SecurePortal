# 🔐 SecurePortal – Governance & Risk Management Project  
*A Practical Cybersecurity Risk Assessment Exercise based on ISO 27005, NIST CSF, CIS Controls, and ISO 27001*

---

## 📌 Overview  
This project simulates the governance, risk management, and security evaluation process of an internal corporate web application called **SecurePortal**.  

The purpose of the project is to demonstrate practical skills in:

- Cybersecurity Governance  
- Risk Assessment (ISO 27005)  
- Risk Scoring & Modeling  
- Threat & Vulnerability Identification  
- Mitigation Planning  
- Security Architecture Analysis  
- Project Management (Roadmap & Prioritization)  

This type of project is commonly performed by **IT Risk Analysts**, **Governance Analysts**, and **GRC professionals**.

---

## 🔥 Highlights

- ✔ Full Risk Assessment following **ISO 27005**
- ✔ Governance approach aligned with **ISO 27001**
- ✔ Risk Matrix (Heatmap) included (PNG + PDF)
- ✔ Architecture Mockup included
- ✔ Risk Scoring, Likelihood & Impact Models
- ✔ Mitigation Plan aligned with **NIST CSF** & **CIS Controls**
- ✔ Roadmap covering 3 sprints (Governance + Project Management)
- ✔ Professional documentation included (PDFs)

---

## 🎯 Objectives of the Project  

The main objectives of this project were:

1. **Create a governance context** for a corporate internal application.  
2. **Identify critical assets** and evaluate their importance.  
3. **Perform a full risk assessment** following the ISO 27005 methodology.  
4. **Build a risk scoring model** to classify risks by probability and impact.  
5. **Design a visual risk heatmap (risk matrix)**.  
6. **Create a simplified architecture mockup** for security analysis.  
7. **Propose mitigation controls** aligned with NIST CSF, CIS Controls, and ISO 27001.  
8. **Develop a short roadmap** simulating project management steps.  

---

## 🏢 Project Context  

**SecurePortal** is a fictitious internal web application used by employees to:

- Access internal company documents  
- View internal policies  
- Manage identity-based operations  

It contains **sensitive internal information**, making it a suitable target for:

- Web attacks  
- Credential-based attacks  
- Data leakage  
- Service disruption  

The project treats SecurePortal as a real corporate system, applying standard governance and risk processes.

---

## 🧱 1. Asset Inventory  

| Asset                    | Type       | Value | Justification                                |
|--------------------------|------------|-------|----------------------------------------------|
| SecurePortal Web App     | Application | High  | Access to internal sensitive information     |
| Internal Database        | Information | High  | Stores credentials & confidential material   |
| User Accounts            | Identity    | Medium| Authentication to the system                 |
| Linux Server             | Infrastructure | Medium | Hosts backend and database                  |

---

## ⚠️ 2. Risk Assessment (ISO 27005)

The following risks were identified as the most relevant:

### 🔥 **Risk 1 – SQL Injection**
- **Asset:** Internal Database  
- **Threat:** Unauthorized data access  
- **Vulnerability:** Weak input validation  
- **Impact:** High  
- **Likelihood:** Medium  
- **Risk Level:** High  

**Mitigations:**  
- Input sanitization  
- Prepared statements  
- WAF (Web Application Firewall)  
- SAST/DAST testing  

---

### 🔐 **Risk 2 – Unauthorized Access (Weak Authentication)**
- **Asset:** User Accounts  
- **Threat:** Credential stuffing / brute force  
- **Vulnerability:** No MFA, weak password policy  
- **Impact:** High  
- **Likelihood:** Medium  
- **Risk Level:** High  

**Mitigations:**  
- MFA  
- Rate limiting  
- Strong password policy  
- Login attempt monitoring  

---

### 💾 **Risk 3 – Backup Failure**
- **Asset:** Database  
- **Threat:** Data loss / corruption  
- **Vulnerability:** Inconsistent backups  
- **Impact:** High  
- **Likelihood:** Low  
- **Risk Level:** Medium  

**Mitigations:**  
- Daily backups  
- Regular restoration tests  
- Off-site backup storage  

---

## 📊 3. Risk Scoring Model  

Risk Score Formula:  

| Score | Meaning |
|-------|---------|
| **1** | Low severity or low likelihood |
| **2** | Moderate conditions |
| **3** | High severity or easily exploitable |

---

## 📈 4. Likelihood Model  

| Level | Description |
|-------|-------------|
| **Low (1)** | Rare or unlikely exploitation |
| **Medium (2)** | Reasonably possible |
| **High (3)** | Frequent, easy to exploit, or historically common |

---

## 🧨 5. Impact Model  

| Level | Description |
|-------|-------------|
| **Low (1)** | Minimal operational effect |
| **Medium (2)** | Noticeable operational disruption |
| **High (3)** | Severe consequences, reputational & regulatory damage |

---

## 🔥 6. Risk Matrix (Heatmap)

The matrix below represents the risks assessed according to the 3x3 **Likelihood x Impact** model.

```
                            **LIKELIHOOD**
                 ┌────────────────────────┬────────────────────────┬────────────────────────┐
                 │       Low (1)        │       Medium (2)        │        High (3)         │
┌────────────────┼────────────────────────┼────────────────────────┼────────────────────────┤
│ High (3)       │        🟨 R3            │        🟧 R1 + R2       │         🟥 —        │
│                │   (Backup Failure)     │ (SQLi + Unauthorized)  │      (Critical)         │
├────────────────┼────────────────────────┼────────────────────────┼────────────────────────┤
│ Medium (2)      │          🟩 —           │          🟨 —           │          🟧 —      │
│                │      (Low)           │      (Medium)           │       (High)            │
├────────────────┼────────────────────────┼────────────────────────┼────────────────────────┤
│ Low (1)      │          🟩 —           │          🟩 —           │          🟨 —         │
│                │      (Low)           │      (Low)           │       (Low)                 │
└────────────────┴────────────────────────┴────────────────────────┴────────────────────────┘
                               **IMPACT**
```


## 🏗️ 7. Architecture Mockup

The simplified architecture of SecurePortal is represented as follows:

![Architecture Mockup](architecture_mockup.png)


Architecture components:

- **Frontend Web**
- **API Backend**
- **Internal Database**
- **Authentication/MFA Server**

---

## 🛠 8. Mitigation Plan  

| Risk | Mitigation | Priority | Deadline |
|------|------------|----------|----------|
| SQL Injection | Input validation, WAF | High | 30 days |
| Unauthorized Access | MFA, rate limiting | High | 15 days |
| Backup Failure | Backup policy review | Medium | 45 days |

---

## 🚀 9. Roadmap (Project Management)

### **Sprint 1**
- Implement MFA  
- Create password policy  
- Review backup process  

### **Sprint 2**
- Implement input validation  
- Configure WAF  
- Backup restoration tests  

### **Sprint 3**
- Create risk dashboard  
- Finalize documentation  

---

## 🎤 10. Pitch (For Interview Use)

> “This project allowed me to apply practical risk governance processes using ISO 27005, evaluate web application risks, build a scoring model, develop a risk matrix, and design an architectural mockup. I defined mitigation controls aligned with NIST CSF, CIS Controls, and ISO 27001 and built a small roadmap simulating real-world GRC project management.”

---

## 👤 Author  
**Hugo Marques**  
Cybersecurity & IT Risk Enthusiast  

---

## 📚 Frameworks Referenced  
- **ISO 27005** – Risk Management  
- **ISO 27001** – Security Controls & Governance  
- **NIST CSF** – Protect, Detect, Respond  
- **CIS Controls** – Practical technical controls  

---

## 🗂️ Files in This Repository  

---

## ✔ Conclusion 
This project demonstrates initiative, understanding of GRC, and the ability to structure a real risk management workflow — perfect for GRC/IT Risk Analyst roles.





