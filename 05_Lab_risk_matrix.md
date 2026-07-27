# Lab: Risk Matrix and Risk Register

A risk assessment for a commercial bank, using a risk register and a risk matrix to score each risk by likelihood and severity, then prioritise remediation.

## Scenario

Joining a cybersecurity team at a commercial bank, I helped conduct a risk assessment of the bank's operational environment by working through its risk register. A **risk register** is a central record of potential risks to an organisation's assets, information systems, and data. For each recorded risk, I determined how likely it was to occur, how severely it could affect the bank, and then calculated a priority score so the team could rank where to focus first.

## Operational environment

The bank sits in a coastal area with low crime rates. Its data is handled by 100 on-premise and 20 remote employees. The customer base includes 2,000 individual and 200 commercial accounts. Its services are marketed by a professional sports team and ten local businesses. Strict financial regulations require the bank to secure its data and funds, including holding enough cash daily to meet Federal Reserve requirements.

## Concepts covered

- Risk registers
- Risk matrices
- Likelihood and severity scoring (1-3)
- Risk prioritisation (Likelihood x Severity)
- Operational-environment context in risk analysis

## Scoring definitions

- **Likelihood (1-3):** the chance of a vulnerability being exploited — 1 low, 2 moderate, 3 high.
- **Severity (1-3):** the potential damage to the business — 1 low, 2 moderate, 3 high.
- **Priority:** how urgently a risk must be addressed, calculated as **Likelihood x Severity = Risk**.

## Sample risk matrix

| Likelihood \ Severity | Low (1) | Moderate (2) | Catastrophic (3) |
| --- | --- | --- | --- |
| **Certain (3)** | 3 | 6 | 9 |
| **Likely (2)** | 2 | 4 | 6 |
| **Rare (1)** | 1 | 2 | 3 |

## Completed risk register (asset: Funds)

| Risk | Description | Likelihood | Severity | Priority |
| --- | --- | --- | --- | --- |
| Business email compromise | An employee is tricked into sharing confidential information | 2 | 2 | 4 |
| Compromised user database | Customer data is poorly encrypted | 2 | 3 | 6 |
| Financial records leak | A database server of backed-up data is publicly accessible | 3 | 3 | 9 |
| Theft | The bank's safe is left unlocked | 1 | 3 | 3 |
| Supply chain disruption | Delivery delays due to natural disasters | 1 | 2 | 2 |

## Analysis

**Notes on the environment:** The low crime rate means physical risks such as theft and disaster-driven supply chain disruption are less likely, so both scored low on likelihood. The financial records leak carries the highest impact and risk because it would affect the bank's finances, reputation, and regulatory compliance, potentially attracting heavy fines. Compromised user data is moderate in severity because encryption exists but needs strengthening, though it could still lead to a breach with serious consequences. Business email compromise is moderate in likelihood; even with a backup to fall back on, it could still carry serious regulatory and reputational consequences.

**Likelihood:** Scores were assigned on the 1-3 matrix. A supply chain disruption from a natural disaster scored 1 given the unpredictability of such events, while compromised-data events scored 2 because they are more likely given their possible causes.

**Severity:** No risk scored below 2, because data-breach risks such as business email compromise carry serious consequences. Bank customers trust the business to protect their money and personal information, and operations could halt if the bank fails to comply with regulations.

**Priority:** The financial records leak received the highest overall score of 9, meaning it is almost certain to occur and would greatly affect the bank's ability to operate. That high score signals the security team to remediate this risk before moving on to lower-scoring ones.

## Key takeaways

- A risk register turns scattered concerns into a structured, scorable list of risks per asset.
- Multiplying likelihood by severity produces a single priority score that makes risks directly comparable.
- Operational context matters: the same risk can score differently depending on the environment, such as a low-crime coastal location reducing physical-theft likelihood.
- The highest-priority risk here (financial records leak, score 9) should be remediated first, ahead of lower-scoring risks.
