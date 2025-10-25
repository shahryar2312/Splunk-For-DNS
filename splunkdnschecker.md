# Analyzing DNS Log Files Using Splunk SIEM

## Introduction
DNS logs help reveal network activity and detect threats such as tunneling, DGA, and exfiltration, which Splunk can uncover with search and visualizations. 

## Prerequisites
- A running Splunk instance (Enterprise or Cloud) with access to Splunk Web. 
- DNS logs (sample Zeek/Bro-style logs work well) ready to upload or forward. 

## Steps to Upload Sample DNS Log Files to Splunk SIEM

### 1. Prepare Sample DNS Log Files
- Obtain a sample DNS dataset (for example, a Zeek dns.log.gz). 
- Ensure events include IPs, queries, types, and response info. 
- Store the file where your Splunk UI can reach it. 

### 2. Upload Log Files to Splunk
- In Splunk Web, go to Settings > Add Data > Upload. 

### 3. Choose File
- Select the sample dns.log.gz file.

### 4. Set Source Type
- Set sourcetype to CustomDNS (custom sourcetype for this project).

### 5. Review Settings
- Confirm index, host, and sourcetype before submitting.

### 6. Click Upload
- Review, then Submit to index the file.

### 7. Verify Upload
- Run a basic search:
