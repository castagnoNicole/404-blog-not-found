---
title: "Securing Connected Vehicles: Insights from Upstream Security’s Marco Fenoglio"
categories:
  - Blog
tags:
  - threat intelligence
  - AI
  - automotive
  - interview
---

This interview was recorded for the Howest IT Student Podcast, available on Spotify. Listen to the full conversation for deeper insights into automotive cybersecurity!
{: .notice}

Last week, I had the chance to sit down with Marco Fenoglio, Director of EMEA Customer Success at Upstream Security. 
With over 20 years in automotive cybersecurity, Marco shared cutting-edge insights on everything from regulatory battles to AI-powered vSOCs.

Here’s what stood out:

## Regulatory compliance
We kicked off by comparing two major frameworks shaping automotive cybersecurity:
- UNECE R155: A global baseline requiring OEMs to implement Cyber Security Management Systems (CSMS) and Threat Analysis & Risk Assessments (TARA). “R155 is a starting point, not an endgame,” Marco noted. “Compliance alone won’t stop dynamic threats.”
- China’s GB 44495-2024: A prescriptive standard mandating 27 specific tests for vehicles. “It’s like R155 on steroids—granular, but still limited to certain vehicle classes.”

## The Automotive Threat Matrix
Auto-ISAC’s Automotive Threat Matrix (ATM)—modeled after MITRE ATT&CK—provides a common language for classifying vehicle-specific attacks. Upstream’s AutoThreat®PRO leverages ATM to:
- Map dark web chatter to real-world attack techniques (e.g., EV charger API exploits).
- Link findings to R155 Annex 5 requirements, streamlining compliance.

Marco highlighted a case where ATM helped trace a ransomware attack on a temperature sensor supplier to vulnerabilities in CAN BUS protocols.

## Remote Attacks & EV Charger Exploits
Marco shared sobering stats from Upstream’s 2024 report:
- 92% of attacks were remote, with 84% requiring no physical proximity.
- EV charger vulnerabilities spiked: From QR code payment scams to zero-days in Open Charge Point Protocol (OCPP) backends

## vSOC Evolution: From Compliance to AI-Powered Defense
Marco is a big fan of AI. He thinks that is the right tool detect ongoing attack in a timely manner. 
More than once during our interview he remarked that just satisfying regualatory requiriments doesn't make the company secure.
For vSOC, Vehicle Security Operations Centers, AI can be fundamental in dectecting an ongoing attack in a timely manner. 
Modern vSOCs are evolving in four stages:

- **Stage 1.0 - R155 & R156 Compliance:** Initially, OEMs establish a dedicated vSOC for compliance, implementing CSMS and SUMS.
  
- **Stage 2.0 - Remediation & Automation:** The vSOC develops end-to-end playbooks to automate responses and integrates with enterprise IT systems for cross-organization visibility.

- **Stage 3.0 - Data-Driven:** Focus shifts to integrating as many data feeds as possible, using automotive-specific cybersecurity analytics for near real-time threat detection.

- **Stage 4.0 - The GenAI Powered vSOC:** Generative AI is leveraged for greater visibility, streamlined investigations, and long-term efficiency,
analyzing massive data, filtering alerts, automating investigations, and enhancing TARA for large-scale risks. The vSOC becomes cross-functional,
expanding coverage to autonomous vehicles, mobility applications, and Smart Mobility devices.

## Proactive Defense: Why Dark Web Intel Matters
Upstream’s team monitors 1,133 active threat actors across dark web forums. This intel helps:
- Prioritize vulnerabilities (e.g., LiDAR spoofing risks).
- Anticipate ransomware campaigns targeting Tier-1 suppliers.

## Bridging the Cybersecurity Gap
The takeaways

more collaboration is necessary: Share threat data across OEMs, insurers, and smart cities, EV charging stations
Proactivity towards cybersecurity not just regulatory compliance
