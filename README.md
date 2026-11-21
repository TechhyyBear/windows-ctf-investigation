# Capture the Flag — Windows/Kali Security Investigation

**QuickStart / University of New Mexico Cybersecurity Bootcamp — Guided Career Simulation 3**

**Focus:** Lab configuration · Host reconnaissance · Service/vulnerability inspection · Controlled Metasploit exercise · Windows investigation · Evidence documentation

## Portfolio snapshot

| | |
| --- | --- |
| **Challenge** | Locate a hidden flag on an intentionally vulnerable Windows machine in an authorized guided lab. |
| **My documented work** | VirtualBox NAT setup, Nmap reconnaissance, controlled Metasploit session work and Windows file investigation. |
| **Observed / reported result** | The submitted video shows a Meterpreter session; the student presentation reports that the challenge flag was found. |
| **Security takeaway** | Distinguish enumeration, successful controlled access and actual post-access results; document outcomes without exaggerating them. |

**Also see:** [Linux Authentication Monitor](https://github.com/TechhyyBear/Linux-authentication-monitor) — a separately developed independent Linux security lab.

## Overview

This repository documents an **authorized Windows/Kali capture-the-flag exercise** completed as part of the QuickStart cybersecurity bootcamp. The student submission shows a VirtualBox NAT lab named **Quickstart**, Kali Linux as the testing workstation, and a deliberately vulnerable Windows CTF target. The objective was to identify the target, examine its exposed services, use the authorized lab exploitation workflow and investigate the Windows filesystem to find a hidden challenge flag.

The submitted video reports that the flag was captured. This is a guided coursework exercise—not a real intrusion, paid penetration test or production incident response.

## Lab environment

| Component | Role |
| --- | --- |
| Oracle VirtualBox | Virtualize the lab systems |
| Quickstart NAT network | Isolated training network; submission describes `10.0.2.0/24` with DHCP |
| Kali Linux | Authorized scanning and controlled testing workstation |
| Windows CTF VM | Intentionally vulnerable target |
| Nmap | Host, service and vulnerability-script reconnaissance |
| Metasploit / Meterpreter | Controlled exploitation and post-exploitation exercise |
| Windows CMD / PowerShell | Navigate and inspect files on the training target |

## Documented investigation

1. Created or configured the Quickstart NAT environment and placed Kali and Windows systems into the exercise network.
2. Identified the target and inspected visible services and reported vulnerabilities with Nmap.
3. Used the Metasploit framework in the authorized lab; the presentation identifies an SMB/EternalBlue-related exercise.
4. Obtained a Meterpreter session as shown in the recorded presentation and used the Windows shell for further inspection.
5. Navigated directories and files to look for the challenge artifacts; the presentation concludes with a reported captured flag.

The original presentation documents the workflow, but does not establish independent exploit development, full vulnerability validation on patched systems, or professional penetration-testing experience.

## Findings and lessons

- Vulnerable or intentionally misconfigured services in a training target can enable access beyond the initial network scan.
- Reconnaissance results must be interpreted carefully: a scanner's vulnerability indication and successful exploitation are separate evidence categories.
- Post-exploitation analysis involves identifying the host, investigating file locations and documenting access without unnecessarily disclosing confidential material.
- Repeatable investigation notes and explicit evidence boundaries make lab actions understandable without disclosing the source recording.

## Project documentation

- [Investigation workflow](INVESTIGATION_WORKFLOW.md) — stages, tools, documented outcomes and evidence limits.
- [Evidence index](EVIDENCE_INDEX.md) — map back to the submitted video, documented outcomes and limitations.

The original approximately 11-minute submission video is retained privately. This is intentionally a **text-only case study**: no video, screenshots, credentials, payloads, host identifiers or final flag content are uploaded.

**Portfolio presentation:** This repository intentionally uses source-grounded text documentation rather than published source media.

## Skills demonstrated

Kali Linux, Windows lab investigation, VirtualBox NAT networking, Nmap, Metasploit fundamentals in an authorized scenario, Meterpreter session navigation, evidence review and technical presentation.

## Scope limitations

This was instructor-demonstrated coursework followed by student task execution. The presentation is the source of the documented results; the lab was not independently rerun for this repository. The environment is deliberately vulnerable and is not representative of an ordinary secured Windows endpoint.

**Original source:** `Career Simulation 3 - Final.mp4`, retained privately. Project 3 is independent of the later `Linux-authentication-monitor` home-lab repository.
