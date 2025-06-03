# ZenFinTech Ltd – AWS S3 Cloud Risk Assessment Brief  
_Service Reviewed: Amazon Simple Storage Service (S3)_  
_Date: June 2025  
_Prepared by: Lambert Agbeehia – GRC Consultant_

---

## 1. Executive Summary

ZenFinTech Ltd uses AWS S3 for storing customer documents, logs, and internal backups. This assessment identifies key security and compliance risks related to S3 usage, with control mappings to **ISO/IEC 27001:2022** and the **NIST Cybersecurity Framework (CSF)**.

---

## 2. Risk Identification

| Risk ID | Risk Description | Likelihood | Impact | Risk Level |
|--------|------------------|------------|--------|------------|
| CR-001 | Publicly exposed S3 buckets | High | Severe | **High** |
| CR-002 | Insecure object-level permissions | Medium | High | **High** |
| CR-003 | Lack of encryption for sensitive data | Medium | Medium | **Medium** |
| CR-004 | Insufficient logging & monitoring | Medium | Medium | **Medium** |
| CR-005 | Absence of versioning or lifecycle policies | Low | Medium | **Low** |

---

## 3. Control Mapping

| Framework | Relevant Controls |
|-----------|-------------------|
| **ISO/IEC 27001:2022** | A.8.10 (Storage Media Protection), A.8.16 (Monitoring Activities), A.5.15 (Access Control), A.5.23 (Information Security in Cloud Services) |
| **NIST CSF** | PR.AC-4 (Access enforcement), PR.DS-1 (Data-at-rest protection), DE.CM-7 (Monitoring for unauthorized access), PR.IP-6 (Data handling policies) |

---

## 4. Recommendations

1. **Bucket Privacy Enforcement**
   - Ensure all S3 buckets are **private by default**
   - Use S3 Block Public Access and enforce service control policies (SCPs)

2. **Encryption Standards**
   - Enable **SSE-S3 or SSE-KMS** for all buckets handling sensitive data
   - Enforce encryption via bucket policies and deny unencrypted uploads

3. **Fine-Grained IAM & ACL Audits**
   - Restrict object-level permissions to least privilege
   - Avoid using `*` in bucket policies

4. **Monitoring & Alerts**
   - Enable **CloudTrail + AWS Config** for S3 access logging
   - Integrate with AWS Security Hub and set alerts for misconfigurations

5. **Lifecycle & Versioning**
   - Apply versioning to critical buckets
   - Define lifecycle rules for archiving, deletion, or transition to Glacier

---

## 5. Residual Risk & Follow-Up

After mitigation, risk posture is reduced to **Low–Medium** range. A re-assessment should be conducted after major infrastructure changes or annually as part of the ISMS cycle.

---

## 6. Appendix: Resources

- [AWS S3 Security Best Practices](https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html)
- [ISO/IEC 27001:2022 Overview](https://www.iso.org/standard/27001)
- [NIST CSF Controls Reference](https://www.nist.gov/cyberframework)

