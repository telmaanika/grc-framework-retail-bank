# Governance, Risk & Compliance Framework – Retail Banking Institution

This project simulates a full GRC (Governance, Risk & Compliance) framework for a fictional retail bank that provides checking, savings, loan services, online banking, ATM access, and card processing.

Retail banks are highly regulated and must implement strong cybersecurity and compliance programs to protect customer financial data.

This project includes:
- A risk register  
- GRC controls mapping  
- Policy templates  
- PCI DSS & NIST CSF controls  
- Compliance gap analysis  
- Audit readiness checklist  

---

## Project Overview

A retail bank handles sensitive data including:
- Cardholder data  
- Customer PII  
- Loan applications  
- Online banking credentials  
- Transaction history  
- ACH transfer data  

This project demonstrates how a GRC analyst or cybersecurity analyst would:
1. Identify risks  
2. Map controls  
3. Assess compliance gaps  
4. Document required policies  
5. Prepare the institution for cybersecurity audits  

**My Notes:**  
This was my choice retail bank because it helped me understand cybersecurity risks in financial systems and how compliance frameworks like NIST and PCI DSS are applied.

---

## Regulatory Frameworks Considered

| Framework | Description |
|-----------|--------------|
| **NIST CSF** | Cybersecurity best practices (Identify, Protect, Detect, Respond, Recover) |
| **PCI DSS** | Cardholder data protection requirements |
| **GLBA** | Gramm–Leach–Bliley Act – Data privacy & safeguarding |
| **FFIEC** | Banking cybersecurity guidelines |
| **SOC 2** | Controls for service organizations |

---

# 📊 Risk Register `risk_register.csv`

```csv
RiskID,Asset,Threat,Impact,Likelihood,Score,Current Controls,Recommended Controls
1,Customer PII,Unauthorized Access,Critical,Medium,20,Password login,MFA + device trust
2,Card Data,Database Breach,Critical,Medium,20,Encryption at rest,Tokenization + key rotation
3,ATM Network,Malware Attack,High,Medium,15,Antivirus,EDR + network segmentation
4,Online Banking,Credential Stuffing,High,High,25,Basic monitoring,Bot protection + rate limiting
5,Loan Application Data,Phishing Attacks,High,Medium,15,Email filter,Security awareness training
6,Core Banking System,Insider Threat,High,Low,10,Role-based access,Log monitoring + segregation of duties


NIST Cybersecurity Framework (CSF)
NIST Category	Application in Retail Banking
ID.AM	Maintain inventory of ATMs, POS devices, servers
PR.AC	MFA for customers + employees
PR.DS	Encrypt all financial data
DE.CM	Monitor online banking logs
RS.MI	Incident response playbook for fraud cases
RC.IM	Lessons learned after suspicious transactions
✔ PCI DSS (Cardholder Data)
Requirement	Bank Implementation
3.0	Protect stored card data
4.0	TLS 1.2+ for all card transactions
7.0	Restrict access to cardholder data
10.0	Log and monitor access to card data
11.0	Penetration testing and vulnerability scans
✔ GLBA Safeguards Rule

Mandatory controls:

Access control

Encryption

Incident response plan

Vendor risk management

Data retention & disposal

Employee security training

 Gap Analysis Summary
Area	Current State	Gap	Severity
MFA	Customer login uses passwords only	MFA missing	High
Logging	Insufficient fraud monitoring	Need SIEM integration	High
Vendor Risk	Third-party payment processor not assessed	Missing vendor reviews	Medium
Policies	Outdated data retention policy	Needs revision	Medium
Awareness	Staff training yearly only	Needs quarterly phishing training	Medium

My NConducting a gap analysis helped me practice evaluating compliance maturity and identifying missing controls.)

Policy Template ; Information Security Policy – Retail Bank

## 1. Purpose
To protect customer financial data, ensure regulatory compliance, and maintain trust in the bank’s services.

## 2. Scope
Applies to all employees, contractors, systems, third-party vendors, and customer-facing services.

## 3. Security Requirements
- All employees must use MFA.  
- All customer PII and financial data must be encrypted.  
- Access must follow least privilege.  
- Logging and monitoring must be enabled for critical systems.  
- Employees must complete quarterly cybersecurity training.

## 4. Incident Response
- Report incidents within 1 hour.  
- Contain affected systems immediately.  
- Notify compliance team and regulators as needed.  

## 5. Enforcement
Failure to comply may result in disciplinary action.

Audit Readiness Checklist
Copy into audit_checklist.md
# Audit Readiness Checklist – Retail Bank

## Administrative Controls
- [ ] Security policies updated (last 12 months)
- [ ] Vendor risk assessments completed
- [ ] GLBA compliance training logged

## Technical Controls
- [ ] MFA enabled for all users
- [ ] Encryption at rest & in transit
- [ ] SIEM integrated with core banking logs
- [ ] Vulnerability scans performed monthly

## Physical Controls
- [ ] Server room access restricted
- [ ] CCTV logs retained 90 days

## PCI DSS Controls
- [ ] Quarterly penetration testing
- [ ] Access logs reviewed daily
- [ ] Firewall rules documented

📁 Folder Structure (Create this in GitHub)
grc-framework-retail-bank/
│
├─ README.md
├─ risk_register.csv
├─ controls_mapping.md
├─ information_security_policy.md
└─ audit_checklist.md

🧠 Personal Reflection

This project helped me understand the compliance requirements of retail banking, including PCI DSS, GLBA, and NIST CSF. I learned how to evaluate gaps, map controls, prepare risk registers, and write policy documentation similar to real GRC analysts.

👤 Author
Telma Anika
Email: tellyannika@gmail.com


