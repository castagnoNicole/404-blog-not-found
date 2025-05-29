---
title: "Getting My Hands Dirty: A Masterclass in ICS Exploitation"
categories:
  - Blog
tags:
  - ics
  - hacking
---

Back in March, I joined a masterclass all about hacking *(ethically, of course!)* Industrial Control Systems, or ICS. I needed a crash course for my internship project, and this class promised exactly that. An exacting morning full of new hacking techniques!

The class brought together a diverse group: researchers and system administrators from Belgian companies. Everyone was curious about how industrial communication protocols work. The sysadmins wanted to learn how to keep their OT (Operational Technology) networks safe, while the researchers were more interested in how these systems could be attacked - for ethical purposes of course!

## Expert Guidance from the Field
The session was led by Tijl Deneut, a well-known researcher and lecturer at Howest University College, recognized for his work uncovering ICS vulnerabilities. He regularly conducts these classes in collaboration with Hendrik Derre, combining academic rigor with real-world insight.

### All About Hands-On
I’ve always found that I learn best by actually doing things, not just reading about them. This class totally delivered on that front. We spent most of our time getting hands-on with real tools and real (simulated) devices.

Our lab environment simulated a tile factory, complete with PLCs (Programmable Logic Controllers) and HMIs (Human-Machine Interfaces) from multiple vendors. It felt pretty close to what you’d find in the wild.

Here’s a breakdown of some key exploits we practiced:

- **SMB Remote Code Execution (MS17-010):** We began with a classic vulnerability on Windows XP. Using zzz_exploit.py, we created a new Windows user and dumped user credentials. Even though passwords were hashed, we could leverage “pass-the-hash” techniques to move laterally within the network.
  
- **Beckhoff HMI Authentication Bypass (CVE-2015-4051):** Next, we targeted older Beckhoff HMIs, exploiting a web interface vulnerability using a Python script provided by our instructor. This demonstrated how legacy devices often lack basic security controls.

- **Schneider Electric Epoch Cookie Attack (CVE-2017-6026):** Some Schneider Electric devices use epoch time as a session cookie, which can be easily retrieved via SNMP to hijack sessions. This highlighted the risks of weak authentication mechanisms in industrial devices.

## Final thoughts
At Howest, our curriculum covers IT penetration testing but only touches on ICS. This masterclass filled that gap, offering exposure to specialized tools and techniques for industrial environments-skills that are increasingly in demand as OT networks face rising cyber threats.

This event was invaluable for anyone looking to expand their expertise from traditional IT security into the world of ICS. I would gladly attend again and highly recommend it to pentesters and security professionals who want to acquire knowledge in protecting critical infrastructure.
