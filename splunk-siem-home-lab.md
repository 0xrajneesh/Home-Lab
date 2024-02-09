# Splunk Home Lab

## ℹ️Overview

This is the most powerful home-lab focused on setting up Splunk SIEM and real-world use cases. If you’re interested to become SOC Analyst(Tier 1/2) , this lab will help you with SOC tools, rules, queries, apps and integration.

## 🧮Requirements

- **Hardware**:
  - Ubuntu Server 22.04(for Splunk Enterprise)
  - Windows 11 Machine

- **Software**:
  - [Splunk Enterprise]((https://www.splunk.com/en_us/download/splunk-enterprise.html )) 
  - Splunk Universal Forwarder
  
  

## 🖼️Lab Diagram

![Home-Lab](https://github.com/0xrajneesh/Home-Lab/assets/40385860/2a1f4e02-3ae9-4d47-8e09-9370548035ed)


## </> Setting up Splunk SIEM on Ubuntu Server
- Install Splunk Enterprise software on Ubuntu server    
- Install Splunk [Security Essentials App]((https://splunkbase.splunk.com/app/3435))  
- Import [BOTS V2 Dataset](https://s3.amazonaws.com/botsdataset/botsv2/botsv2_data_set_attack_only.tgz)  

## 🧑‍💻Excercises
- **SQL Injection**: Analyze web logs to detect potential SQL injection attempts. *Hint: Look for unusual characters or SQL keywords used in URI parameters, such as ' or 1=1.*  
- **Cross-Site Scripting (XSS)**: Monitor web logs for signs of Cross-Site Scripting (XSS) attacks. *Hint: Search for requests containing suspicious JavaScript keywords like "script", "<script>", or "onload".*  
- **Cross-Site Request Forgery**: Identify potential Cross-Site Request Forgery (CSRF) attacks in web logs. *Hint: Look for requests with unexpected or unauthorized actions, such as changes in user settings or profile information*.
- **Directory Traversal**: Search for indications of Directory Traversal attacks in web logs. *Hint:  Check for requests containing "../" or "%2e%2e/" sequences in the URI, attempting to access files outside the web root*.
- **Brute Force**: Monitor access logs for patterns indicative of brute force attacks. *Hint: Look for repeated login attempts from the same IP address or requests with multiple failed authentication attempts*.
- **Session Hijacking**: Detect potential session hijacking attempts by analyzing web logs. *Hint: Look for multiple logins from different IP addresses for the same user account in a short time frame.*
- **Remote Code Execution**: Identify potential Remote Code Execution (RCE) attempts in web logs. *Hint: Look for requests with unusual file extensions or commands that may indicate attempts to execute arbitrary code on the server.*
- **XXL External Entity**: Search for indications of XML External Entity (XXE) attacks in web logs. *Hint: Look for requests with XML payloads containing references to external entities or unusual XML processing instructions.*
- **Insecure Deserialization Detection**: Detect potential Insecure Deserialization attempts in web logs. *Hint: Look for requests with serialized data or references to known serialization libraries vulnerable to exploitation*.
- **SSRF Detection**: Monitor web logs for signs of Server-Side Request Forgery (SSRF) attacks. *Hint: Look for requests with URLs pointing to internal or sensitive resources, or containing unexpected protocols like "file://" or "gopher://"*.


## 🔴Build and Learn with us
- Live Home-Lab Set up and Exercises
- Day: 1st and 3rd Saturday
- Duration: 2 hours
- Recording available
