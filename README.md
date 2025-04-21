# Packet Crafting & Honeypot Lab (NDG Lab 14)

**Author:** Ian Sweet  
**Course:** CPS 401 – Defensive Security  
**Date:** April 18, 2025  
**Institution:** Boise State University  

## Overview

This project was completed to demonstrate packet crafting and honeypot techniques using Python and firewall configuration tools. The lab explores how attackers might use custom packets to evade detection, and how defenders can use crafted responses and honeypots to detect and deter reconnaissance activity.

## Summary

Lab 14 introduced packet crafting and scanner honeypots using the Scapy tool. We began by generating basic IP and TCP packets to understand packet structure and formatting. This helped illustrate how Scapy builds packets and how header information is layered and modified.

Next, we adjusted firewall rules using pfSense to allow all TCP SYN packets. We then captured and sniffed these packets using Scapy, analyzing the different TCP flag types like SYN (S), SYN-ACK (SA), and ACK (A).

Finally, we created a spoofed honeypot script (`spoofopen.py`) that made it appear as though all ports on a system were open. This technique is useful for confusing port scanners and can trigger alerts when suspicious scanning behavior is detected.

## Real-World Application

Packet crafting is a critical concept in both offensive and defensive security. Attackers may use malformed or custom packets to bypass firewalls or IDS systems. Conversely, security analysts can leverage crafted packets and honeypots to:

- Detect stealthy scanning attempts
- Understand attacker tactics
- Monitor unauthorized access attempts

An example use case: a SOC analyst could deploy a honeypot that logs all scans to seemingly open ports, identifying early-stage reconnaissance before an actual exploit is attempted.

## Skills Demonstrated

- Python scripting for network traffic simulation
- Packet structure manipulation with Scapy
- Firewall policy adjustment using pfSense
- Basic threat deception techniques with honeypots
- TCP flag analysis and packet sniffing

## Tools & Technologies

- Python 3
- Scapy
- pfSense Firewall
- Wireshark (optional analysis)
- Custom honeypot script (`spoofopen.py`)

## File Structure


# Honeypot simulation script (deceptive open ports)
# Scapy-generated packet creation
# TCP packet sniffer with Scapy
# Visual outputs from the lab
# Project summary ([SweetIan_NDG14–Packet Crafting_Module5_04-18-2025.pdf](https://github.com/user-attachments/files/19827682/SweetIan_NDG14.Packet.Crafting_Module5_04-18-2025.pdf)

## Conclusion

This lab provided valuable hands-on experience with custom packet generation, real-time traffic analysis, and deceptive network defenses. These are key skills for blue team defenders and SOC analysts looking to proactively understand and respond to network-based threats.

By learning to build and analyze raw packets, and simulate attacker behavior through honeypots, I’ve built a deeper understanding of how network threats operate — and how to counter them.

## Contact

**Ian Sweet**  
Email: iansweet315@u.boisestate.edu
