# Risk Assessment: NIST SP 800-30 Rev. 1

A vulnerability assessment of a publicly accessible database server, conducted using the NIST SP 800-30 Rev. 1 guidance and documented as a written vulnerability assessment report.

## Scenario

As a newly hired cybersecurity analyst at an e-commerce company, I assessed a remote database server that stores customer information. Employees around the world query the server to find potential customers. The database had been open to the public since the company launched three years earlier, which is a serious vulnerability. The task was to assess the risk and communicate it to decision makers in a written report explaining how the exposed server threatens business operations and how it can be secured.

## About NIST SP 800-30 Rev. 1

NIST SP 800-30 is a publication that provides guidance on performing risk assessments, outlining strategies for identifying, analysing, and remediating risk. Organisations use it to understand the likelihood and severity of risks so they can make informed decisions about allocating resources, implementing controls, and prioritising remediation. "Rev. 1" indicates the first revised version of the publication.

## Concepts covered

- Vulnerability assessment
- Threat sources and threat events
- Likelihood and severity scoring (qualitative and quantitative)
- Risk calculation (Likelihood x Severity)
- Vulnerability assessment reporting
- Remediation strategy

## Threat sources

NIST SP 800-30 categorises threat sources as entities or circumstances that can negatively affect an organisation's information systems, considering the intent and capabilities of both internal and external sources.

- **Standard user:** employee, customer
- **Privileged user:** system administrator
- **Group:** competitor, supplier, business partner, nation state
- **Outsider:** hacker, hacktivist, advanced persistent threat (APT)
- **Hardware:** storage, processing, communications failures
- **Software:** operating systems, networking, malicious software
- **Operational environment:** temperature/humidity controls, faulty power supplies
- **Natural hazards:** power outages, extreme weather events

## Threat events

Threat events are actual instances where a threat source exploits a vulnerability and causes harm. Examples relevant to an exposed database server include reconnaissance and surveillance, obtaining sensitive information via exfiltration, altering or deleting critical information, crafting counterfeit certificates, installing network sniffers, denial-of-service (DoS) attacks, disrupting mission-critical operations, obfuscating future attacks, and man-in-the-middle attacks.

## Scoring scales

Both likelihood and severity are scored on a 1-3 scale:

| Qualitative | Quantitative | Description |
| --- | --- | --- |
| High | 3 | Almost certain to occur; multiple, severe, or catastrophic effects |
| Moderate | 2 | Somewhat likely; significantly reduces functionality of operations and assets |
| Low | 1 | Highly unlikely; minor or negligible effects |

Overall risk is calculated as **Likelihood x Severity**.

## Vulnerability assessment report

**System description:** The server has a powerful CPU and 128GB of memory, runs the latest version of Linux, and hosts a MySQL database management system. It uses a stable IPv4 network connection, interacts with other servers, and includes SSL/TLS encrypted connections.

**Scope:** The assessment covers the current access controls of the system over a three-month period (June to August 20XX), guided by NIST SP 800-30 Rev. 1.

**Purpose:** The report explains why the database server is valuable to the business, why securing its data matters, and how the business would be affected if the server were disabled.

### Risk assessment

| Threat source | Threat event | Likelihood | Severity | Risk |
| --- | --- | --- | --- | --- |
| Competitor (example) | Obtain sensitive information via exfiltration | 1 | 3 | 3 |
| Outside hacker | Alter/delete critical information | 3 | 3 | 9 |
| Hacker | Install persistent and targeted network sniffers | 3 | 3 | 9 |
| Business partner | Obtain sensitive information via exfiltration | 1 | 3 | 3 |

**Approach:** Risks were evaluated against the business's data storage and management methods, weighing the likelihood of each threat and its impact against day-to-day operational needs.

**Remediation strategy:** Implement authentication, authorisation, and auditing so that only authorised users reach the database server. This includes strong passwords, role-based access control, and multi-factor authentication to limit privileges. Encrypt data in motion using TLS rather than SSL, and apply IP allow-listing to corporate offices so that random users on the internet cannot connect to the database.

## Key takeaways

- A publicly accessible database is a high-impact vulnerability; the highest-scoring risks (score 9) came from hackers able to alter data or install network sniffers.
- NIST SP 800-30 provides a structured way to identify threat sources and events, then score likelihood and severity to prioritise remediation.
- Effective remediation combines access control (MFA, role-based access, allow-listing) with strong encryption of data in transit.

