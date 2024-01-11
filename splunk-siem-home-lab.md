# Splunk Home Lab

## Overview

This is the most powerful home-lab focused on setting up Splunk SIEM and real-world use cases. If you’re interested to become SOC Analyst(Tier 1/2) , this lab will help you with SOC tools, rules, queries, apps and integration.

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

## Setting up Splunk 

1. **Download Splunk Enterprise [FREE TRIAL 60 days] **
   - Follow the [official installation guide](https://www.splunk.com/en_us/download/splunk-enterprise.html ).

2. **Download Splunk Security Essentials App [FREE] **
   - Follow the [official installation guide](https://splunkbase.splunk.com/app/3435 ).


## Sample Queries

Include sample Splunk queries to showcase the functionality of your lab.

```spl
index=your_index sourcetype=your_sourcetype | stats count by field_name
