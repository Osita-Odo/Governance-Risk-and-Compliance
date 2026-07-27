# Assets-Threats-and-Vulnerabilities-Risk-Assessment-Labs


A collection of risk assessment and asset management activities completed as part of the Google Cybersecurity Certificate (Assets, Threats, and Vulnerabilities). Each activity applies a security framework or method to a realistic scenario, from investigating a suspicious USB drive to building a risk register for a bank. These activities demonstrate applying recognised frameworks (NIST CSF, SP 800-30, SP 800-53) to assess and prioritise risk, classify assets, and recommend practical controls that protect an organisation's data and operations.

## Summary

These labs move through the practical side of managing risk in an organisation. They cover how to inventory and classify assets, how to investigate a physical-media threat safely, how to run a structured vulnerability assessment using NIST guidance, how to analyse a real data leak through the lens of least privilege, and how to score and prioritise risks in a register. Together they show the full arc of identifying what needs protecting, understanding what threatens it, scoring the risk, and recommending controls.

## Knowledge gained

- **Asset management** — building an asset inventory and classifying devices by sensitivity and importance to decide where protection is most needed.
- **Data protection** — understanding data states (at rest, in transit, in use) and keeping data away from unauthorised users.
- **Safe threat investigation** — using virtualisation and isolation to examine untrusted media, and recognising USB baiting and social-engineering tactics.
- **Vulnerability assessment** — applying NIST SP 800-30 Rev. 1 to identify threat sources and events, score likelihood and severity, and write a vulnerability assessment report.
- **Least privilege** — applying NIST SP 800-53: AC-6 to limit access by role, revoke access when no longer needed, and audit privileges regularly.
- **Risk scoring and prioritisation** — using a risk register and risk matrix to calculate risk as Likelihood x Severity and rank remediation.
- **Frameworks** — navigating the NIST Cybersecurity Framework's function → category → subcategory → control structure.
- **Remediation** — recommending technical, operational, and managerial controls such as MFA, role-based access, encryption in transit, and IP allow-listing.

## Labs

| # | Lab | Focus | Key concepts |
| --- | --- | --- | --- |
| 01 | [Risk assessment: lost USB stick](01_Risk_assessment_lost_USB_stick.md) | USB baiting investigation | Virtualisation, PII, attacker mindset, controls |
| 02 | [Risk assessment: NIST SP 800-30 Rev. 1](02_Risk_assessment_NIST_SP_800-30.md) | Vulnerability assessment of an exposed server | Threat sources/events, likelihood, severity, remediation |
| 03 | [Asset classification and inventory](03_Asset_classification_and_inventory.md) | Home office asset management | Asset inventory, classification, data states |
| 04 | [Data leak worksheet and least privilege](04_Data_leak_worksheet_least_privilege.md) | Analysing a data leak | Least privilege, AC-6, access auditing |
| 05 | [Lab: risk matrix and risk register](05_Lab_risk_matrix.md) | Bank risk assessment | Risk register, risk matrix, prioritisation |


