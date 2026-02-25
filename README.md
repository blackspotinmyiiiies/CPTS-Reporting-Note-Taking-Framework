# HTB CPTS & Professional Pentest Reporting Framework

A tactical bash script designed to automate the creation of a professional, HTB CPTS-compliant reporting structure. This tool streamlines the transition from **Exploitation** to **Post-Exploitation** and **Reporting**, ensuring zero data loss and high-signal documentation.

## Tactical Overview

The `pentest.sh` script generates a complete Markdown-based ecosystem for an engagement, including:

* **Executive Reporting:** CPTS-standard template with CVSS 3.1 scoring and risk assessment.
* **Technical Findings:** Granular, template-driven finding files (CWE, Root Cause, Impact).
* **Attack Chain Walkthroughs:** 5-Phase breakdown (External Access to Domain Compromise).
* **Evidence Management:** Organized directory structure for screenshots, logs, and raw tool outputs.
* **Credential Tracking:** Centralized summary for AD, local, and application-level credentials.

## Directory Structure

```text
Project_Name/
├── 00-QUICK-START.md        # Immediate operator guidance
├── 01-Executive-Report.md   # Final deliverable template
├── Credentials-Summary.md   # Tactical credential tracking
├── 02-Technical-Findings/   # Individual vulnerability reports
├── 03-Attack-Chains/        # Phase 1-5 walkthroughs
├── 04-Evidence/             # Proof-of-concept storage
├── 05-Tools-Output/         # Raw nmap, gobuster, etc.
└── 06-Flags/                # HTB-specific flag tracking
```
## Usage

    Download pentest.sh to your attack host (Pwnbox or Kali).

    Execute the script to initialize the mission:
    ```bash
    chmod +x pentest.sh
    ./pentest.sh <Project_Name> <Client_Name>
    ```
Example:
./pentest.sh "HTB_Omniscient" "HackTheBox"
