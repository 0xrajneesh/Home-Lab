# Wireshark Home_Lab

## ℹ️Overview

This home-lab is focussed on setting up Wireshark Home-Lab and getting hands-on with practical scenarios. If you are a Network Security engineer, SOC Analyst or Aspirant Security Analyst, this home-lab with help you with Network Analysis, Security Forensics and Malware TRaffic Analysis.

## 🧮Requirements

1. **Attacker**: Kali Linux

2. **Defender**: Windows 11 or Ubuntu with Wireshark

## 🖼️Lab Diagram

Insert a diagram here to visualize the lab architecture.

## </> Setting up Wireshark Home-Lab

📍Download and Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)  
📍Download and import [Kali Linux](https://www.kali.org/get-kali/#kali-virtual-machines) in Virtualbox  
📍Download and import [Windows 11](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines/) in Virtualbox  
📍Download and install [Wireshark](https://www.wireshark.org/download.html) on Windows 11  


## 🧑‍💻Excercise- Network Analysis
📍 **ARP Packet Analysis**: Capture [ARP](https://wiki.wireshark.org/uploads/__moin_import__/attachments/SampleCaptures/arp-storm.pcap) packets to monitor address resolution and detect network mapping activities.

📍 **ICMP Packet Analysis**: Analyze [ICMP](https://wiki.wireshark.org/uploads/df619289f2986680173b8cd3035ca4ac/220614_ip_flags_google.pcapng) packets to troubleshoot network connectivity issues.  

📍 **DHCP Packet Analysis**: Investigate [DHCP](https://wiki.wireshark.org/uploads/__moin_import__/attachments/SampleCaptures/dhcp.pcap) traffic to identify IP address leases and lease durations.  

📍 **SMTP Traffic Analysis**: Monitor [SMTP](https://wiki.wireshark.org/uploads/__moin_import__/attachments/SampleCaptures/smtp.pcap) traffic to detect email communication and extract sender/receiver information.  

📍 **FTP Traffic Analysis**: Capture [FTP](https://wiki.wireshark.org/uploads/__moin_import__/attachments/SampleCaptures/FTPv6-1.cap) packets to analyze file transfers and extract filenames.  

📍 **DNS Traffic Analysis**: Analyze [DNS](https://wiki.wireshark.org/uploads/__moin_import__/attachments/SampleCaptures/dns-remoteshell.pcap) packets to identify domain lookups and resolve IP addresses.    

📍 **HTTP Traffic Analysis**: Capture [HTTP](https://wiki.wireshark.org/uploads/27707187aeb30df68e70c8fb9d614981/http.cap) traffic and extract URLs visited.  


## 🧑‍💻Excercise- Security Forensics
📍 **SYN Scan**: Detect SYN scan by identifying packets with SYN flag set and multiple consecutive SYN-ACK responses.  

📍 **UDP Scan**: Identify UDP scan by analyzing packets with UDP destination ports and absence of corresponding responses or ICMP port unreachable messages.   

📍 **TCP Connect Scan**: Recognize TCP connect scan by observing TCP three-way handshake sequences.  

📍 **ACK Scan**: Detect ACK scan by analyzing packets with only ACK flag set and no SYN or FIN flags.

📍 **FIN Scan**: Identify FIN scan by observing packets with only FIN flag set and absence of response packets or ICMP unreachable messages.  

📍 **XMAS Scan**: Detect XMAS scan by analyzing packets with FIN, PSH, and URG flags set simultaneously and absence of corresponding responses.   

📍 **NULL Scan**: Recognize NULL scan by analyzing packets with no TCP flags set and absence of response packets or ICMP unreachable messages.  

📍 **TCP Window Scan**: Detect TCP Window scan by analyzing packets with varying TCP window sizes indicating potential reconnaissance.  

📍 **IDLE Scan**: Identify Idle scan by analyzing packets from a seemingly unrelated zombie host, observing indirect communication patterns.  

📍 **FTP Traffic Analysis**: Capture FTP packets to analyze file transfers and extract filenames.  

📍 **DNS Traffic Analysis**: Analyze DNS packets to identify domain lookups and resolve IP addresses.    

📍 **Version Scan**: Recognize version detection scan by analyzing packets containing service banners or responses with version information.  

📍 **DDoS attack**: Detect DDoS attacks by analyzing abnormal traffic patterns, such as a sudden surge in incoming packets from multiple sources targeting specific ports or services.  




## 🔴Build and Learn with us
- Live Home-Lab Set up and Exercises
- Day: 1st and 3rd Saturday
- Duration: 2 hours
- Recording available
