# Registry-Persistence-Detection--TryHackMe--Cybersecurity-Learning-Journey
I completed Registry Persistence Detection room on TryHackMe! Learn to use the AutoRuns PowerShell module to detect persistence mechanisms that use the Registry.

# Registry Persistence Detection — TryHackMe Write-Up

## Overview

I successfully completed the **Registry Persistence Detection** room on TryHackMe, which focuses on identifying Windows persistence mechanisms that leverage the Windows Registry. This hands-on lab introduced the use of the **AutoRuns PowerShell module** to investigate startup locations commonly abused by attackers to maintain access to compromised systems.

The room provided practical experience in threat hunting, persistence analysis, and forensic investigation techniques used by security analysts and incident responders.

---

## Objectives

* Understand Windows Registry-based persistence techniques.
* Learn how attackers abuse Registry Run and RunOnce keys.
* Use the AutoRuns PowerShell module to enumerate startup entries.
* Identify suspicious autorun artifacts.
* Investigate malicious persistence mechanisms.
* Improve detection and analysis skills relevant to SOC and DFIR environments.

---

## Scenario

In this lab, I assumed the role of a security analyst tasked with investigating a Windows workstation suspected of harboring malicious persistence mechanisms.

The objective was to analyze startup locations, identify unauthorized Registry entries, and determine which artifacts were responsible for executing potentially malicious code during system startup.

Using PowerShell and the AutoRuns module, I performed a structured investigation to uncover suspicious Registry-based persistence and validate the associated executable responsible for the behavior.

---

## Key Concepts Covered

### Windows Registry Persistence

Registry persistence is one of the most common techniques used by attackers to maintain access after initial compromise. By creating Registry entries in startup locations, malicious programs can automatically execute whenever a user logs in or the system boots.

Common Registry locations include:

```text
HKCU\Software\Microsoft\Windows\CurrentVersion\Run
HKLM\Software\Microsoft\Windows\CurrentVersion\Run
HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce
HKLM\Software\Microsoft\Windows\CurrentVersion\RunOnce
```

---

## Tools Used

### AutoRuns PowerShell Module

The AutoRuns PowerShell module was used to enumerate and analyze persistence artifacts across the Windows operating system.

Capabilities include:

* Enumerating startup Registry entries
* Detecting suspicious autorun locations
* Reviewing startup executables
* Identifying persistence mechanisms
* Supporting incident response investigations

---

## Investigation Process

### 1. Enumerated Autorun Locations

Used the AutoRuns module to collect startup artifacts from the system and identify Registry entries configured to execute automatically.

### 2. Analyzed Registry Persistence

Reviewed Registry Run and RunOnce keys for unusual or unauthorized entries.

### 3. Identified Suspicious Artifact

Located a startup Registry entry that appeared inconsistent with legitimate system behavior.

### 4. Investigated Associated Executable

Traced the Registry value to the executable being launched during startup and analyzed its behavior.

### 5. Validated Persistence Mechanism

Confirmed that the Registry entry was responsible for executing the suspicious file whenever the system started.

---

## Skills Developed

* Windows Registry Analysis
* Persistence Detection
* Digital Forensics Fundamentals
* Threat Hunting
* PowerShell Investigation
* Incident Response Methodology
* Windows Internals
* Security Monitoring
* Malware Persistence Analysis

---

## Key Takeaways

* Registry-based persistence remains one of the most widely used attacker techniques.
* Startup Registry locations should be routinely monitored during investigations.
* AutoRuns provides valuable visibility into system startup behavior.
* Understanding persistence mechanisms is critical for effective incident response and threat hunting.
* PowerShell is an essential tool for forensic analysis and Windows security investigations.

---

## Conclusion

This room provided practical experience in identifying and investigating Registry-based persistence mechanisms commonly used by adversaries. By leveraging the AutoRuns PowerShell module, I gained hands-on exposure to detecting malicious startup entries and analyzing persistence artifacts in a Windows environment.

The lab reinforced important defensive security concepts and strengthened my understanding of Windows persistence techniques, making it a valuable exercise for both SOC analysts and incident responders.

---

**Platform:** TryHackMe
**Room:** Registry Persistence Detection
**Category:** Blue Team / DFIR / Threat Hunting
**Difficulty:** Beginner–Intermediate

---
LinkedIn:[https://www.linkedin.com/feed/update/urn:li:activity:7468010781465415680/]
X :[https://x.com/charisma1385/status/2062242593577029880]


#TryHackMe #BlueTeam #SOCAnalyst #DFIR #DigitalForensics #ThreatHunting #CyberSecurity #IncidentResponse #WindowsSecurity #PowerShell #AutoRuns #RegistryPersistence #MalwareAnalysis #SecurityOperations #CyberDefense
