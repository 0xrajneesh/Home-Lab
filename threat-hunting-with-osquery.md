# Threat Hunting and Investigation using Osquery

## ℹ️Overview

The goal of this home lab is to familiarize yourself with Osquery and its capabilities for threat detection and investigation. By setting up a lab environment, you'll gain hands-on experience with querying system information and using it to identify potential security threats. Osquery is an open-source tool that allows you to query your devices (Windows, macOS, Linux) for various system information in a SQL-like language. It provides deep visibility into your systems, which makes it an excellent tool for threat hunting and investigation. 

## 🧮Requirements

- **Hardware**:
  - Computer with at least 16GB RAM and dual-core processor
- **VM/ISO Image**:
  - Windows 11 OVA image
  - Ubuntu Server 22.04 OVA image
  - Wazuh OVA image

## 🖼️Lab Diagram



## </> Setting up Osquery Home-Lab
- Install [Osquery on Windows 11 machine](https://pkg.osquery.io/windows/osquery-4.8.0.msi)
- Install [Osquery on Ubuntu Server](https://osquery.readthedocs.io/en/stable/installation/install-linux/)



## 🧑‍💻Excercises- Persistence
-  **Registry Run Keys / StartUp Folder**: Examines registry keys and startup folders to identify programs set to run automatically when the system starts up.
-  **RunKeys (with hashvalue)**: Queries registry keys associated with automatic execution and retrieves hash values of the files linked to these keys.
-  **Security Support Provider**: Investigates the Security Support Provider (SSP) configurations, which are crucial for authentication mechanisms in Windows systems.
-  **Service Creation / Modification (auto_start)**: Monitors changes to Windows services, particularly focusing on modifications related to automatic start settings.
-  **Look for suspicious DLLs loaded by any service (with associated username & hash value of the DLL)**: Identifies services loading suspicious DLLs, providing details such as associated usernames and hash values of the DLLs.
-  **WMI Event Consumers (command line & script)**: Investigates Windows Management Instrumentation (WMI) event consumers, which can include command lines or scripts triggered by events.
-  **WMI Process Interrogation**: Queries WMI for information about running processes, allowing investigation into process-related activities.
-  **Application Shimming**: Looks for instances of application shimming, a technique used to intercept calls between applications and the Windows operating system.
-  **Print Processors - Reg Keys**: Examines registry keys related to print processors, which are responsible for converting print data into a format suitable for printing.
-  **Look for suspicious print drivers**: Identifies potentially malicious print drivers installed on the system, which could be used to compromise print services.
-  **Image File Execution Options Injection (IFEO)(debugger/GlobalFlag)**: Investigates Image File Execution Options (IFEO) registry keys for evidence of debugger or GlobalFlag manipulation, commonly used in injection attacks.
-  **PowerShell Process Interrogation**: Queries PowerShell processes to gather information about their execution and potential usage in malicious activities.

## 🧑‍💻Excercises- Memory Analysis
- **pslist equivalent**: Retrieves a list of running processes similar to the pslist command, providing details such as process ID, parent process ID, user, and executable path.
- **pstree equivalent (Parent & Child)**: Generates a hierarchical view of processes, displaying parent and child relationships similar to the pstree command.
- **pstree equivalent (Grandparent, Parent & Child)**: Expands upon the pstree equivalent by including grandparent, parent, and child relationships, offering a more comprehensive view of process ancestry.
- **dlllist equivalent (with a specific PID)**: Lists the dynamic-link libraries (DLLs) loaded by a specific process ID, similar to the dlllist command in memory analysis tools.
- **dlllist - load all the DLLs**: Retrieves a list of all loaded DLLs across all running processes, providing insight into shared libraries in memory.
- **getsids equivalent**: Retrieves security identifiers (SIDs) associated with processes, akin to the getsids command in memory analysis tools, aiding in identifying process ownership.
- **svcscan equivalent**: Scans for Windows services running on the system, akin to the svcscan command, assisting in the identification of services and their configurations.
- **netscan equivalent**: Conducts a scan of network-related information such as open ports, listening sockets, and established connections, similar to the netscan command in memory analysis tools.
- **Code Injection**: Detects instances of code injection, a common technique used by malware to execute arbitrary code within legitimate processes, thereby evading detection.
- **malfind (not exactly) equivalent**:  Although Osquery doesn't have a direct equivalent to malfind, it can be used in combination with other queries to identify suspicious memory regions or artifacts indicative of malware presence.

## 🧑‍💻Excercises- Process Interrogation
- **Parent & Grandparent Process Identification**: Identifies parent and grandparent processes, aiding in the detection of suspicious process relationships.
- **Suspicious Processes with Usernames:**: Associates processes with usernames to detect suspicious activity under unauthorized accounts.
- **Programs Running from "TEMP" Locations**: Identifies processes running executables from temporary locations, often used by malware for evasion.
- **Processes with Open Pipes**: Detects processes with open pipes, indicative of potential inter-process communication or malicious activity.
- **Processes Originating from wow64 Directory**: Monitors processes originating from the wow64 directory, which may indicate compatibility layers or potential threats.
- **Suspicious DLLs Loaded by Services with User Accounts**: Detects services loading suspicious DLLs and associates them with user accounts, aiding in identifying malicious services.
- **Binary Signature Verification**: Checks if binaries are digitally signed, helping to identify potentially malicious or tampered executables.
- **PowerShell & WMI Process Interrogation**: Investigates parent and child processes related to PowerShell and WMI, common targets for malicious activity.
- **Excessive Memory Usage Detection**: Monitors processes for excessive memory usage, which may indicate memory-resident threats.
- **Remote Network Connection Monitoring**: Identifies processes making remote network connections and examines them for suspicious behavior.  



