# Suricata IDS Home-Lab

## ℹ️Overview

The goal of setting up a Suricata home-lab is to gain practical experience in deploying and configuring an Intrusion Detection System (IDS) for network security monitoring. Suricata is an open-source IDS capable of detecting and preventing various network-based threats. This home-lab provides individuals with hands-on experience in setting up, configuring, and utilizing Suricata to enhance network security.   

## 🧮Requirements

- **Hardware**:
  - Computer with at least 16GB RAM and dual-core processor
- **VM/ISO Image**:
  - Windows Machine(Victim Machine)
  - Kali Linux(Attacker Machine)

## 🖼️Lab Diagram

![Home-Lab (3)](https://github.com/0xrajneesh/Home-Lab/assets/40385860/f7891499-7a73-4f03-99dc-df2a2720904c)


## </> Setting up the Suricata Home-Lab

- **Setting up Suricata IDS Server**
  -  Import Ubuntu Server 22.04 OVA file in Virtualbox
  -  Install Suricata IDS package
 
- **Setting up Victim Server-1**
  -  Import Ubuntu Server 22.04 OVA file in Virtualbox
  -  Install DVWA(Damn Vulnerable Web Application)

- **Setting up Victim Server-2**
  -  Import Metasploitable 2 OVA Image
 
- **Setting up Victim Server-3**
  -  Import Typhoon OVA image
 


## 🧑‍💻Excercises- Network-based attacks
-  **Nmap Stealth Scan Detection**: Create a Suricata rule to detect TCP SYN packets sent to multiple ports within a short time frame, indicative of Nmap stealth scans.  
-  **Nmap OS Fingerprinting Detection**: Develop a Suricata rule to detect ICMP echo requests and responses with specific TTL values, characteristic of Nmap OS fingerprinting activities.  
-  **Nmap Service Version Detection Detection**: Formulate a Suricata rule to detect Nmap service version detection probes based on unique HTTP GET requests or TCP SYN/ACK packets.  
-  **Metasploit Exploit Payload Detection**: Craft a Suricata rule to detect Metasploit exploit payload traffic based on unique signatures or payloads commonly used in exploits.  
-  **Metasploit Reverse Shell Detection**: Develop a Suricata rule to detect Metasploit reverse shell connections by monitoring for outbound TCP connections to known attacker IP addresses.  
-  **Metasploit Meterpreter Communication Detection**: Create a Suricata rule to detect Meterpreter communication activities by analyzing HTTP or TCP traffic with characteristic Meterpreter payloads.
- **Metasploit Credential Harvesting Detection**: Formulate a Suricata rule to detect Metasploit credential harvesting activities by monitoring for specific LDAP or SMB traffic patterns indicative of credential theft.  



