# Data Leak Worksheet and Least Privilege

An analysis of a data leak caused by over-permissioned folder sharing, using the principle of least privilege and the NIST Cybersecurity Framework to identify issues and recommend controls.

## Scenario

A sales manager shared access to a folder of internal-only documents with their team during a meeting. The folder held files for an unannounced product, along with customer analytics and promotional materials. After the meeting, the manager did not revoke access but warned the team to wait for approval before sharing the promotional materials.

Later, during a video call with a business partner, a sales representative intended to share a link to the promotional materials but accidentally shared a link to the internal folder instead. The business partner, assuming it was the promotional content, posted the link on their company's social media page, exposing internal information publicly.

## Concepts covered

- Principle of least privilege
- Access control (NIST SP 800-53: AC-6)
- Data classification
- NIST Cybersecurity Framework (CSF)
- Regular access auditing

## Data leak worksheet

**Control: Least privilege**

**Issues — what factors contributed to the leak?**
The manager did not apply least privilege; access to the internal folder should have been kept restricted or revoked until release was approved. The sales representative, aware of the data's nature, should also have classified it promptly to reduce the chance of mistakes. In short, access to the internal folder was not limited to the sales team and manager, and the business partner should never have been in a position to share it publicly.

**Review — what does NIST SP 800-53: AC-6 address?**
AC-6 addresses the principle of least privilege: how an organisation can protect data privacy by granting users only the access they need. It also suggests control enhancements to improve the effectiveness of least privilege.

**Recommendations — how might least privilege be improved?**
- Restrict access to sensitive resources based on user role.
- Automatically revoke access to information after a set period.
- Regularly audit user privileges.

**Justification — how would these address the issues?**
Role-based access ensures no one can reach data irrelevant to their work, which protects privacy, supports compliance, and limits leakage. Restricting shared links to internal files to employees only, and requiring managers and security teams to audit access to team files regularly, would further limit exposure of sensitive information.

## Security plan snapshot (NIST CSF)

The NIST Cybersecurity Framework uses a hierarchical, tree-like structure. Reading from left to right, it moves from a broad security **function**, to a more specific **category**, then **subcategory**, and finally to individual security **controls** and their references. This structure maps the high-level goal (for example, protecting data) down to the concrete control that achieves it (for example, AC-6 least privilege).

## Key takeaways

- Least privilege limits both accidental and deliberate data exposure by granting only the access a role requires.
- Access that is granted should be time-bound and revoked when no longer needed, rather than left open indefinitely.
- Classifying data promptly helps prevent handling mistakes such as sharing the wrong link.
- Regular privilege audits are a practical control for catching over-permissioned access before it causes a leak.
- NIST SP 800-53: AC-6 is the reference control for least privilege, and the NIST CSF connects such controls to broader security functions.
