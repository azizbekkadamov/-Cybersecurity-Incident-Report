# Cybersecurity-Incident-Report

🛡️ Cybersecurity Incident Report: DNS & ICMP Traffic Analysis
This project presents a practical cybersecurity incident response scenario focused on diagnosing network-level issues using DNS and ICMP analysis. The incident revolves around failed DNS queries to the domain www.yummyrecipesforme.com, where traffic analysis revealed ICMP errors pointing to an unreachable DNS service on port 53.

The report outlines the detection, investigation, and root cause of the issue, demonstrating how tools like tcpdump are used in real-world troubleshooting.

🧾 Project Overview
The project is divided into two main parts:

🔍 Incident Summary
ICMP error messages indicated “udp port 53 unreachable” when attempting DNS queries.

DNS resolution failed, leading to customer complaints about the website being inaccessible.

The UDP traffic sent to the DNS server did not receive a valid DNS response.

🛠️ Investigation & Findings
IT used tcpdump to capture network traffic.

Analysis confirmed no DNS service was listening on port 53 of the DNS server.

This led to ICMP “Destination Port Unreachable” messages.

The DNS query failure prevented proper IP resolution, halting access to the client website.

📄 Files Included
Cybersecurity_Incident_Report.docx — Full technical report with incident details

README.md — Project overview and documentation

🚀 How to Use This Project
Open the .docx report to review the incident analysis.

Use it as a case study in network traffic analysis and cybersecurity coursework.

Reference the structure for writing your own incident response reports.

🎓 Learning Outcomes
By reviewing this project, you will:

Understand how DNS and ICMP protocols interact in network troubleshooting.

Learn how to interpret ICMP error messages in packet captures.

Develop skills in incident response and documenting technical findings.

Apply critical thinking in diagnosing service outages using low-level traffic tools.

🧰 Tools Used
tcpdump (for packet capture)

Web browser (for simulating DNS queries)

ICMP analysis via traffic logs

📌 Notes
This report was developed for academic purposes as part of a cybersecurity practical project. It is a realistic example of how network issues are diagnosed using protocol-level analysis.
