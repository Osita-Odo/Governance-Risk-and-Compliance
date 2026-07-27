# Asset Classification and Inventory

An asset management activity: building an inventory of devices on a home office network and classifying them by sensitivity and importance to determine which need extra protection.

## Scenario

Operating a small business from a home office, I created an inventory of network devices to determine which ones hold sensitive information requiring extra protection. Asset management is a critical part of any security plan. It starts with an asset inventory (a catalogue of assets to protect) and then classifies those assets by their importance and sensitivity to risk.

## Concepts covered

- Asset management and asset inventory
- Asset classification by sensitivity
- Network devices and network access
- Data states (at rest, in transit, in use)
- NIST Cybersecurity Framework (CSF)
- Policies, standards, and procedures

## Asset inventory

Three devices with access to the home network were identified, catalogued, and classified. A typical completed inventory records, for each device, the network access it has, the sensitivity of the data it handles, and how it is used:

| Asset | Network access | Sensitivity | Notes |
| --- | --- | --- | --- |
| Laptop / desktop computer | Constant | Confidential | Stores business files and login credentials; highest protection priority |
| Smartphone | Constant | Confidential | Holds email, contacts, and authentication apps |
| Smart home / streaming device | Occasional | Internal-only / low | Limited sensitive data but still a potential entry point to the network |

Devices that store or access confidential business information are classified at a higher sensitivity and therefore receive stronger controls, while devices handling little sensitive data are classified lower but are still tracked because any networked device is a possible attack surface.

## Key terms

- **Asset:** an item perceived as having value to an organisation.
- **Asset classification:** labelling assets based on sensitivity and importance to an organisation.
- **Asset inventory:** a catalogue of assets that need to be protected.
- **Asset management:** the process of tracking assets and the risks that affect them.
- **Compliance:** adhering to internal standards and external regulations.
- **Information security (InfoSec):** keeping data in all states away from unauthorised users.
- **NIST Cybersecurity Framework (CSF):** a voluntary framework of standards, guidelines, and best practices to manage cybersecurity risk.
- **Policy:** a set of rules that reduce risk and protect information.
- **Procedures:** step-by-step instructions to perform a specific security task.
- **Regulations:** rules set by a government or authority to control how something is done.
- **Risk:** anything that can affect the confidentiality, integrity, or availability of an asset.
- **Standards:** references that inform how to set policies.
- **Threat:** any circumstance or event that can negatively affect assets.
- **Vulnerability:** a weakness that can be exploited by a threat.

## Data and its states

**Data** is information that is translated, processed, or stored by a computer. It exists in three states:

- **Data at rest:** data not currently being accessed.
- **Data in transit:** data travelling from one point to another.
- **Data in use:** data being accessed by one or more users.

## Key takeaways

- Effective asset management begins with a complete inventory, then classification by sensitivity and importance.
- Classifying assets shows where to concentrate protection: devices holding confidential data warrant the strongest controls.
- Every networked device is a potential entry point, so even low-sensitivity assets belong in the inventory.
- Protecting data means securing it across all three states: at rest, in transit, and in use.
