# Risk Assessment: Lost USB Stick

A risk assessment of a USB baiting scenario, examining the security risks of an unknown USB drive found on hospital grounds and the controls that could mitigate such attacks.

## Scenario

As part of the security team at Rhetorical Hospital, I found a USB stick bearing the hospital's logo in the car park. Following best practice, the drive was investigated inside virtualisation software: a simulated instance of a computer that is isolated from other files and networks, so an infected drive cannot affect other systems.

Inspecting the drive in the virtual environment revealed a mix of personal and work-related files apparently belonging to Jorge Bailey, the hospital's human resources manager, including family and pet photos, a new hire letter, and an employee shift schedule. None of the files were opened, which is the correct approach.

## Concepts covered

- USB baiting attacks
- Safe investigation using virtualisation and isolation
- Personally identifiable information (PII) exposure
- Attacker mindset and social engineering
- Technical, operational, and managerial controls

## Assessment

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
