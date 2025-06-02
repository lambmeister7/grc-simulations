# ZenFinTech Ltd – Risk Register  
_Version: 1.0_  
_Last updated: June 2025_  
_ISO/IEC 27001:2022 Compliance_  
_Confidentiality: Internal Use Only_

---

## Risk Scoring Methodology

| Score | Likelihood | Impact |
|-------|------------|--------|
| 1     | Rare       | Negligible |
| 2     | Unlikely   | Minor |
| 3     | Possible   | Moderate |
| 4     | Likely     | Major |
| 5     | Almost Certain | Severe |

**Risk Rating = Likelihood × Impact**

- **Low (1–6)**  
- **Medium (7–12)**  
- **High (13–25)**

---

## 📊 Risk Register

| Risk ID | Description | Likelihood | Impact | Risk Score | Existing Controls | Proposed Mitigation | Owner | Status |
|---------|-------------|------------|--------|------------|--------------------|----------------------|-------|--------|
| R-001 | Unauthorised access to customer data | 4 | 5 | **20 (High)** | MFA, user access logs | Conduct quarterly access reviews, implement Just-In-Time access | ISO | Open |
| R-002 | Data breach via misconfigured AWS S3 bucket | 3 | 5 | **15 (High)** | IAM policies, encryption | Set bucket policies to private by default; automate config audits | DevOps Lead | Open |
| R-003 | Insider threat from disgruntled employee | 3 | 4 | **12 (Medium)** | Exit checklist, NDAs | Add behaviour monitoring; implement anomaly detection tools | HR & Security | Open |
| R-004 | Incomplete GDPR subject access request response | 4 | 3 | **12 (Medium)** | SAR checklist, email template | Automate request tracking with deadlines and alerts | DPO | Open |
| R-005 | Third-party vendor data leak | 2 | 5 | **10 (Medium)** | Basic vendor agreements | Introduce vendor risk assessments; enforce ISO 27001 clause 5.22 | Procurement | Open |

---

## Notes

- Risks are reviewed **quarterly** or upon major change
- Mitigations feed into the **Statement of Applicability** and **Audit Plan**
- Each risk has an assigned owner responsible for follow-up actions

---

📌 _Prepared by:_  
**Lambert Agbeehia**  
GRC Consultant, ZenFinTech Ltd (Simulation Project)
