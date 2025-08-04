 Cyber Security Internship – Task 1

Task: Network Port Scanning & Analysis using Nmap & Wireshark

This task involved scanning the local network to identify active devices, open ports, and the services running on them. The scan results were analyzed to evaluate potential security risks. Wireshark was used to capture packets during the scan to understand how a TCP SYN scan works at the packet level.

Tools Used
Nmap – Port scanning tool
Wireshark– Network traffic capture and analysis
Kali Linux – Operating system used for performing the scan
Mobile Hotspot – Used as local network environment

---

Network Info
Local IP Range Scanned: 172.20.10.0/24
Devices Detected: 3
  - 172.20.10.1 – Mobile hotspot/router
  - 172.20.10.3 – IoT/smart device
  - 172.20.10.5 – Kali Linux scanner



Summary of Results
| IP Address      | Open Ports                         |
|------------------|------------------------------------|
| 172.20.10.1      | 21 (FTP), 53 (DNS), 49152, 62078   |
| 172.20.10.3      | 7100 (font-service), 8000 (http-alt) |
| 172.20.10.5      | No open ports                     |

---

Security Risks Identified
FTP (Port 21) is unencrypted — should be disabled or replaced with SFTP.
High-numbered ports(49152, 62078, 8000) may be exposing custom or dynamic services.
Unsecured HTTP (Port 8000)could leak data if used publicly.

---

Files Included in This Repo
- scan_results.txt – Nmap output
- .png – Wireshark screenshots
- syn_packets_filter.png
- syn_ack_response.png
- rst_response_closed_port.png
- initial_syn_packets.png
- Final_CyberSecurity_Task1_Report.docx – Full written report
- README.md – This file


 Key Takeaways
- Learned to perform local network port scanning
- Understood how SYN scans function using TCP handshake
- Practiced traffic filtering and analysis with Wireshark
- Recognized potential vulnerabilities from open ports
