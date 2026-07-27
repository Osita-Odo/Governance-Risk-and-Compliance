# Risk Assessment: Lost USB Stick

A risk assessment of a USB baiting scenario, examining the security risks of an unknown USB drive found on hospital grounds and the controls that could mitigate such attacks.

## Scenario

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/aa8ef3b2-f9fb-4b93-b303-9539a5223122" />

Jorge's drive contains a mix of personal and work-related files. For example, it contains folders that appear to store family and pet photos. There is also a new hire letter and an employee shift schedule.
Review the types of information that Jorge has stored on this device. Then, in the Contents row of the activity template, write 2-3 sentences (40-60 words) about the type of information that's stored on the USB drive.
Note: USB drives often contain an assortment of personally identifiable information (PII). Attackers can easily use this sensitive information to target the data owner or others around them. 
The flash drive appears to contain a mixture of personal and work-related files. Consider how an attacker might use this information if they obtained it. Also, consider whether this whole event was staged.
For example, an attacker could have placed these files on the USB drive as a distraction. They might have targeted Jorge or someone he knows, hoping they would find the device and plug it into their workstation. In doing so, the attacker could establish a backdoor into the company's systems while the unsuspecting target browsed through the files.
In the Attacker mindset row of the activity template, write 2-3 sentences (40-60 words) about how this information could be used against Jorge or the hospital.
Pro tip: The Cybersecurity and Infrastructure Security Agency (CISA) provides some security tips on using caution with USB drives, including keeping personal and business drives separate.
You have not opened any of the files on the device, which is best practice. 
Attackers sometimes conduct USB baiting attacks to deliver malicious code that they've crafted.
However, this USB drive was still a security risk even though it did not contain malicious code. It could have easily been found by an attacker who might have used its contents to plan a variety of attacks.
Consider some of the risks associated with USB baiting attacks:
•	What types of malicious software could be hidden on these devices? What could have happened if the device were infected and discovered by another employee?
•	What sensitive information could a threat actor find on a device like this?
•	How might that information be used against an individual or an organization?
In the Risk analysis row of the activity template, write 3 or 4 sentences (60-80 words) describing any technical, operational, or managerial controls that could mitigate USB baiting attacks.
<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/233ef99e-9ac4-43d4-a81f-1c94818994f0" />


## Concepts covered

- USB baiting attacks
- Safe investigation using virtualisation and isolation
- Personally identifiable information (PII) exposure
- Attacker mindset and social engineering
- Technical, operational, and managerial controls

## Assessment

<img width="400" height="600" alt="image" src="https://github.com/user-attachments/assets/fef0501a-e01a-4247-831a-5b8277c49189" />

### Contents

The USB drive holds a combination of personal and professional material. On the personal side, it contains folders of family and pet photographs. On the professional side, it holds a new hire letter and an employee shift schedule, both of which relate to the HR manager's role. Together, these amount to personally identifiable information about the owner and colleagues.

### Attacker mindset

An attacker could use this information to target Jorge or the hospital directly. Personal photos and HR documents provide detail that supports convincing phishing or social-engineering approaches. The event may also have been staged: an attacker could have planted the drive as bait, hoping an employee would plug it into a workstation and unknowingly open a backdoor into the hospital's systems while browsing the files.

### Risk analysis

Even without malicious code, the drive is a security risk because its contents could support further attacks if found by a threat actor. USB baiting can deliver malware such as ransomware, spyware, or a remote-access backdoor once the device is connected. Controls that mitigate this include:

- **Technical:** disabling autorun, restricting USB ports through endpoint controls, and requiring that unknown media only be examined inside isolated virtual environments.
- **Operational:** keeping personal and business drives separate, and training staff never to plug in found devices.
- **Managerial:** a clear removable-media policy and an incident-reporting procedure for discovered devices.

## Key takeaways

- Unknown USB drives should never be plugged into production systems; virtualisation provides a safe, isolated way to investigate them.
- A drive can be a security risk even when it carries no malware, because the PII it holds can fuel targeted attacks.
- USB baiting relies on curiosity, so a combination of technical restrictions, staff awareness, and clear policy is the most effective defence.
