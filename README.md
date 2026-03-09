# SOC PCAP Analysis Labs

A collection of hands-on SOC Tier 1 analyst investigations using Wireshark,
VirusTotal, and threat intelligence tools.

---

## Lab 1 — SOC4.pcapng Network Traffic Analysis

### Overview
Full network forensics investigation of a 62,965 packet capture.
Identified a **confirmed C2 beaconing incident** alongside a false positive,
demonstrating real SOC analyst triage methodology.

### Tools Used
- Wireshark (Protocol Hierarchy, Conversations, HTTP/DNS filters)
- VirusTotal (IP and domain reputation)
- Kali Linux terminal (file extraction, sha256sum)

### Key Findings
| Indicator | Verdict |
|---|---|
| 146.190.62.39 (httpforever.com) | ✅ False Positive — normal browsing |
| audienceexposure.com | 🔴 TRUE POSITIVE — DNS C2 beaconing every 5 seconds |

### Skills Demonstrated
- HTTP traffic analysis and TCP stream following
- JavaScript malware analysis
- DNS beaconing pattern detection
- Threat intelligence with VirusTotal
- False positive vs true positive decision making
- IOC extraction and documentation

### Files
| File | Description |
|---|---|
| `SOC4.pcapng` | Original packet capture file |
| `SOC4_Investigation_Report.docx` | Full formal investigation report |

### Investigation Report
Download the full report: [SOC4_Investigation_Report.docx](./SOC4_Investigation_Report.docx)

---

## About
**Analyst:** Paulson K Babu
**Background:** BCA + MCA | Cybersecurity — SOC Analyst Track
**LinkedIn:** [www.linkedin.com/in/paulson-babu-472563215]
