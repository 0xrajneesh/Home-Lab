# Splunk Home Lab

## Overview

This repository contains the documentation and configuration files for my Splunk Home Lab.

## Lab Architecture

### Components

1. **Splunk Enterprise**: Version X.X.X
    - [Download Splunk](https://www.splunk.com/en_us/download.html)

2. **Forwarder**: Version X.X.X
    - [Download Splunk Universal Forwarder](https://www.splunk.com/en_us/download/universal-forwarder.html)

3. **Additional Components**:
    - Component 1
    - Component 2

### Diagram

Insert a diagram here to visualize the lab architecture.

## Setup Instructions

1. **Install Splunk Enterprise**
   - Follow the [official installation guide](https://docs.splunk.com/Documentation/Splunk/latest/Installation/InstallonLinux).

2. **Install Universal Forwarder**
   - Follow the [official installation guide](https://docs.splunk.com/Documentation/Forwarder/latest/Forwarder/Installtheuniversalforwarder).

3. **Configure Forwarder to Send Data**
   - Edit `inputs.conf` to specify the data you want to forward.

4. **Additional Configurations**
   - Any other configurations needed for your specific use case.

## Sample Queries

Include sample Splunk queries to showcase the functionality of your lab.

```spl
index=your_index sourcetype=your_sourcetype | stats count by field_name
