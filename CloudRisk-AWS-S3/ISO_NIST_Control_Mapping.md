# ZenFinTech Ltd – Cloud Risk Control Mapping  
_Service: AWS S3_  
_Date: June 2025_  
_Analyst: Lambert Agbeehia_

---

## 🎯 Objective

This mapping aligns five identified AWS S3 cloud risks with specific ISO/IEC 27001:2022 Annex A controls and NIST Cybersecurity Framework (CSF) subcategories. It ensures each risk is traceable to a formal control reference for audit and remediation planning.

---

## 🔐 Risk-to-Control Mapping Table

| Risk ID | Risk Description | ISO/IEC 27001:2022 Controls | NIST CSF Controls |
|---------|------------------|-----------------------------|-------------------|
| **R1** | Public exposure of S3 buckets | A.5.15 – Access Control<br>A.5.23 – Information Security in Cloud Services | PR.AC-4 – Access enforcement<br>PR.AC-6 – Least privilege |
| **R2** | Lack of encryption on sensitive files | A.8.10 – Storage Media Protection<br>A.8.11 – Secure Disposal | PR.DS-1 – Protect data at rest<br>PR.DS-2 – Protect data in transit |
| **R3** | Over-permissive IAM roles or ACLs | A.5.15 – Access Control<br>A.5.16 – Identity Management | PR.AC-1 – Identities and credentials<br>PR.AC-4 – Access enforcement |
| **R4** | No monitoring or misconfiguration alerts | A.8.16 – Monitoring Activities<br>A.5.31 – Security Review of Cloud Services | DE.CM-7 – Monitoring for unauthorised access<br>DE.CM-8 – Audit log review |
| **R5** | No lifecycle or versioning strategy | A.5.10 – Acceptable Use of Assets<br>A.8.14 – Data Retention | PR.IP-6 – Data lifecycle policies<br>PR.DS-5 – Data retention and disposal |

---

## 🧩 Additional Notes

- **ISO Clause 5.23** is critical for cloud service use cases, mandating that cloud risks be reviewed during procurement, operation, and termination stages.
- **NIST PR (Protect)** and **DE (Detect)** categories are the most relevant for AWS S3, especially for storage, access, and visibility.
- Risks with high exposure (R1–R2) must be tied into your **ISMS risk register** and your **cloud security policy** for full compliance alignment.

---

📌 _Prepared by:_  
**Lambert Agbeehia**  
Cybersecurity & GRC Consultant  
[GitHub](https://github.com/lambmeister7) | [LinkedIn](https://www.linkedin.com/in/lambert-agbeehia-1480a018b/)
