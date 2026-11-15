# SOC HTTP Log Investigation using Splunk

## Project Overview

This project focuses on investigating HTTP traffic using Splunk from a Security Operations Center (SOC) perspective.

The investigation analyses HTTP event patterns, source and destination IP addresses, status codes, automated scanning activity, suspicious HTTP methods, and potential web application attack behaviour.

## Objectives

- Analyse large volumes of HTTP logs using Splunk.
- Identify high-volume source IP addresses and targeted systems.
- Investigate HTTP status-code distributions.
- Detect automated scanning and directory enumeration.
- Identify suspicious HTTP methods such as PUT, DELETE, TRACE and PROPFIND.
- Investigate unusual request patterns and potential web attack activity.
- Develop SOC investigation findings and recommended actions.

## Tools and Technologies

- **Splunk:** Log analysis, searching, filtering and visualisation.
- **HTTP:** Web traffic investigation.
- **SPL:** Splunk Search Processing Language.
- **SOC Analysis:** Security event investigation and threat hunting.

## Investigation Areas

| Area | Investigation |
|---|---|
| HTTP Traffic Analysis | Event volume, methods and status codes |
| Source IP Analysis | High-volume clients and suspicious sources |
| Destination Analysis | Targeted internal web servers |
| Automated Scanning | Nmap, DirBuster, Nikto and Skipfish activity |
| Directory Enumeration | High URI diversity and repeated HTTP 404 responses |
| WebDAV Investigation | PUT requests and uploaded file retrieval |
| Suspicious HTTP Methods | PUT, DELETE, TRACE and PROPFIND |
| Timeline Analysis | Traffic spikes and suspicious activity periods |

## Key Findings

- Analysed approximately 2 million HTTP events.
- Identified 71 unique source IP addresses and 88 destination IP addresses.
- Observed a high volume of HTTP 404 responses.
- Identified extensive automated directory enumeration associated with DirBuster.
- Investigated scanner-related User-Agent activity.
- Identified suspicious WebDAV PUT requests receiving HTTP 201 Created responses, followed by retrieval requests.
- Investigated unusual POST activity and requests targeting administrative and phpMyAdmin resources.

**Important:** These findings indicate suspicious activity and potential security concerns. The available HTTP logs do not independently establish successful exploitation or code execution.

## Project Documentation

### 1. Main Investigation Report

Contains the investigation methodology, traffic analysis, findings, and SOC recommendations.

[View HTTP Log Investigation Report](HTTP_Log_Investigation_Report.pdf)

### 2. Splunk Evidence Screenshots

Contains supporting Splunk screenshots and visual evidence from the investigation.

[View Splunk Evidence Screenshots](Evidence%20screenshot.pdf)

## Learning Outcomes

Through this project, I gained practical experience in:

- Security log analysis using Splunk.
- Writing and understanding SPL searches.
- Identifying suspicious HTTP traffic patterns.
- Investigating automated web scanning.
- Analysing source-to-destination relationships.
- Interpreting HTTP methods and response codes.
- Developing SOC investigation findings.

## Disclaimer

This project is intended for educational and defensive cybersecurity purposes. Findings are based on the HTTP log dataset provided for the investigation and should not be treated as confirmation of a successful security compromise without further evidence.
