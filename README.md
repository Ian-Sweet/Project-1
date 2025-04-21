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

## File Structure

