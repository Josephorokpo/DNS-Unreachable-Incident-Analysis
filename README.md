# **DNS Unreachable Incident Analysis**

## **Project Introduction**

This project documents the investigation of a simulated cybersecurity incident where clients reported being unable to access www.yummyrecipesforme.com, receiving a "destination port unreachable" error. As a cybersecurity analyst, I analyzed network traffic data from a tcpdump log to pinpoint the affected network protocol and service, demonstrating skills in incident assessment and network troubleshooting.

## **Methodology and Analysis**

The investigation began by attempting to access the problematic website, which confirmed the "destination port unreachable" error. I then utilized a network protocol analyzer (tcpdump) to capture and examine traffic during an attempt to load the webpage. The provided tcpdump log, detailing DNS (UDP) queries and ICMP error responses, was the primary data source for analysis.

My methodology involved:

1. **Initial Problem Confirmation:** Verifying the reported "destination port unreachable" error.  
2. **Traffic Capture & Review:** Simulating tcpdump capture and systematically reviewing the log entries.  
3. **Protocol Identification:** Distinguishing between normal DNS queries (UDP) and the error responses (ICMP).  
4. **Error Message Interpretation:** Analyzing the "udp port 53 unreachable" message to understand the specific communication failure.  
5. **Trend Analysis:** Identifying patterns in the log, such as repeated failed DNS queries and consistent ICMP error messages, to confirm the nature of the issue.  
6. **Root Cause Suspection:** Formulating a suspected root cause based on the protocol behavior and error messages.

## **Incident Report & Findings**

A comprehensive incident report, detailing the problem summary, analysis, and suspected root cause, is provided in the DNS\_Incident\_Report.md file within this repository.

## **Key Learnings**

This activity reinforced the importance of:

* Understanding the TCP/IP model, particularly the Internet layer and its protocols (IP, ICMP).  
* Analyzing tcpdump (or similar packet capture) logs to diagnose network connectivity issues.  
* Interpreting ICMP error messages to identify specific service or port problems.  
* Recognizing the critical role of DNS in website accessibility.  
* The initial steps in troubleshooting a network-related service outage.