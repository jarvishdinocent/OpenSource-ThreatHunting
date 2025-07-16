# OpenSource-ThreatHunting

Welcome to the OpenSource-ThreatHunting repository! This is an open-source initiative aimed at sharing threat intelligence, tools, and methodologies for effective threat hunting. Our goal is to provide valuable resources for security professionals, threat analysts, and incident responders to detect and mitigate advanced threats in the wild.

This repository contains various resources, including detailed threat intelligence reports, indicators of compromise (IOCs), tools, playbooks, and techniques for advanced threat detection.

## Table of Contents

- [Introduction](#introduction)
- [Threats](#threats)
- [Indicators of Compromise (IOCs)](#indicators-of-compromise-iocs)
- [Tools](#tools)
- [Playbooks](#playbooks)
- [MITRE ATT&CK](#mitre-attck)
- [Logs](#logs)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

The OpenSource-ThreatHunting repository serves as a centralized location for open-source threat intelligence. It is designed to help security researchers, threat hunters, and professionals who are looking for real-world data on threats, their tactics, and available detection methods.

The primary goal is to collect and share intelligence on common and emerging threats, providing tools, scripts, and playbooks for threat hunting and analysis.

---

## Threats

This section contains a curated list of threats and attack methods observed in recent cybersecurity incidents. Each threat is detailed with its description, techniques used, and mitigation strategies.

### 1. Amber Albatross
   - Description: The Amber Albatross intrusion chain contains multiple stages with anti-analysis techniques that make sandbox analysis difficult.

### 2. Mimikatz
   - Description: Mimikatz is a credential-dumping utility commonly leveraged by adversaries, penetration testers, and red teams to extract passwords.

### 3. Bazar
   - Description: The Bazar family of malware continued to be active in 2021, spurring ransomware infections. It uses Microsoft Certificate Services with `certutil.exe` to initiate downloads.

### 4. NetSupport Manager
   - Description: Commonly misused as a malicious remote access trojan (RAT), NetSupport Manager is often used for unauthorized remote access to victim machines.

### 5. BloodHound
   - Description: BloodHound is an open-source tool used to identify attack paths and relationships in Active Directory environments. Frequently seen in ransomware intrusions.

### 6. PlugX
   - Description: PlugX is a remote access trojan linked to espionage operators with ties to Chinese interests, often used in cyber espionage campaigns.

### 7. Charcoal Stork
   - Description: A suspected pay-per-install (PPI) provider that uses malvertising to deliver installers masquerading as cracked games or wallpapers.

### 8. Qbot
   - Description: A banking trojan that focuses on stealing user credentials and banking information.

### 9. ChromeLoader
   - Description: A browser hijacker capable of redirecting searches and sending search data to its command-and-control server, preventing users from uninstalling a malicious extension.

### 10. Raspberry Robin
   - Description: A worm-like activity cluster that spreads through external drives and leverages Windows Installer to download malicious files.

### 11. Cobalt Strike
   - Description: A popular command-and-control (C2) framework often used by adversaries, particularly in post-exploitation scenarios in ransomware attacks.

### 12. Rose Flamingo
   - Description: This threat uses SEO poisoning to trick victims into downloading malicious files.

### 13. Dridex
   - Description: A banking trojan distributed via phishing emails containing malicious Excel documents.

### 14. Scarlet Goldfinch
   - Description: A fake browser update activity cluster that tricks users into downloading a malicious JavaScript file, typically installing NetSupport Manager.

### 15. Emotet
   - Description: A modular trojan that serves as a downloader and dropper for other malware, primarily used for distributing ransomware.

### 16. Shlayer
   - Description: A macOS trojan known for delivering adware, often used in ad fraud activities.

### 17. Gamarue
   - Description: A USB worm that spreads malware via infected USB devices.

### 18. Silver Sparrow
   - Description: A macOS-based activity cluster with fully functional distribution methods, but no final payload.

### 19. Gootloader
   - Description: A JScript-based malware family used for SEO poisoning and delivering malicious ZIP archives that disguise themselves as documents.

### 20. SmashJacker
   - Description: A browser hijacker that distributes via sites offering downloads of wallpapers, games, and software.

### 21. HijackLoader
   - Description: A malware loader that injects additional payloads via process injection.

### 22. SocGholish
   - Description: A malware that masquerades as software updates for initial access, often linked to the suspected Russian cybercrime group Evil Corp.

### 23. IcedID
   - Description: A banking trojan frequently delivered through phishing campaigns.

### 24. TA551 (Shathak)
   - Description: A cybercrime group known for large-scale phishing campaigns that deliver malware payloads.

### 25. Impacket
   - Description: A collection of Python classes used for Windows network protocols, often seen in penetration testing and post-exploitation activities.

### 26. TrickBot
   - Description: A modular banking trojan that acts as a dropper for other malware and targets financial data.

### 27. LummaC2
   - Description: A malware-as-a-service (MaaS) stealer with fake CAPTCHAs and paste-and-run lures, sold on underground forums.

### 28. Yellow Cockatoo
   - Description: A cluster using SEO poisoning to trick users into installing a .NET RAT with infostealer capabilities.

For more details on each threat, check out the [Threats directory](./Threats/).

---

## Indicators of Compromise (IOCs)

The **IOC-Collections** directory contains data about known Indicators of Compromise associated with the threats listed above. IOCs include IP addresses, domains, file hashes, and URLs that can be used to detect threats in your environment.

For more information, check the [IOC-Collections directory](./IOC-Collections/).

---

## Tools

The **Tools** directory contains open-source scripts, utilities, and tools designed for threat hunting, malware analysis, and incident response. These tools can help automate the detection and identification of threats.

To explore the tools, check out the [Tools directory](./Tools/).

---

## Playbooks

The **Playbooks** directory contains step-by-step guides and playbooks that assist analysts in performing threat hunting and incident response. These playbooks are designed to guide analysts through the process of investigating and responding to specific types of attacks.

- [Detecting Mimikatz Activity](./Playbooks/detect_mimikatz_playbook.md): A playbook for identifying Mimikatz credential-dumping activity.
- [Phishing Investigation Playbook](./Playbooks/phishing_investigation_playbook.md): A playbook to investigate phishing campaigns.

For more detailed playbooks, check the [Playbooks directory](./Playbooks/).

---

## MITRE ATT&CK

The **MITRE ATT&CK** directory maps adversary tactics, techniques, and procedures (TTPs) to the MITRE ATT&CK framework. This is useful for identifying and understanding adversary behaviors and helps defenders design more effective detection strategies.

- [Initial Access](./MITRE-ATT&CK/initial_access.md): Techniques used for initial access to a target system.
- [Execution](./MITRE-ATT&CK/execution.md): Methods adversaries use to execute their malicious payloads.

For more details on MITRE ATT&CK techniques, visit the [MITRE-ATT&CK directory](./MITRE-ATT&CK/).

---

## Logs

The **Logs** directory contains sample logs that can be used for training, detection, and practice in analyzing threat activities. These logs simulate real-world scenarios and can help hone your threat-hunting skills.

- [Windows Event Logs](./Logs/log_sample_1.log): Sample logs showing suspicious PowerShell activity.
- [Firewall Logs](./Logs/log_sample_2.log): Sample logs indicating signs of a network intrusion.

Explore the [Logs directory](./Logs/) for sample log files.

---

## Contributing

We welcome contributions from the community! If you have any threat intelligence, IOCs, tools, playbooks, or techniques that could benefit others, please feel free to contribute.

To contribute:
1. Fork the repository.
2. Clone your fork to your local machine.
3. Create a new branch for your changes.
4. Add your changes (new threats, IOCs, tools, playbooks).
5. Submit a pull request.

For more detailed contribution guidelines, check the [CONTRIBUTING.md](./CONTRIBUTING.md) file.

---

## License

This repository is licensed under the [MIT License](LICENSE).

---

## Conclusion

Thank you for visiting the OpenSource-ThreatHunting repository! We aim to foster collaboration and knowledge sharing in the cybersecurity community. Feel free to explore the contents of the repository, use the resources provided, and contribute your own findings to help others in the fight against cyber threats.

