# Investigation workflow — Career Simulation 3

**Source:** Original `Career Simulation 3 - Final.mp4` submitted presentation, reviewed through selected visual frames and the prior evidence-grounded career context record.

## Training environment

The video describes:
- A VirtualBox **NAT** network named `Quickstart`.
- An addressing range of `10.0.2.0/24` with DHCP enabled.
- A Kali Linux analysis machine and a Windows CTF target.
- An intentionally vulnerable Windows target configured for the training challenge.

These are lab conditions, not an internet-exposed host or an employer environment.

## Phase 1 — Setup and network identification

The presentation describes bringing both virtual machines into the Quickstart NAT environment and identifying the target system. It shows the NAT network settings and subsequent Kali terminal activity.

## Phase 2 — Reconnaissance

The recorded presentation includes Nmap service enumeration and a vulnerability-script scan. It points to SMB-related exposure as part of the Windows CTF attack path.

**Evidence distinction:** A script report or a likely SMB issue is not, by itself, proof that exploitation will succeed on every version/configuration. The project is scoped to the purposely vulnerable Windows VM.

## Phase 3 — Controlled access exercise

The submission demonstrates a Metasploit workflow involving an EternalBlue/MS17-010-related training path and a Meterpreter session. The video contains Windows shell and identity-check output during post-exploitation investigation.

**Do not generalize:** This is not independently authored exploit code or evidence of access to real systems. Reproducing the exercise is appropriate only inside the intentionally vulnerable, authorized lab.

## Phase 4 — Host-file investigation

The presentation describes navigating with Windows CMD and PowerShell to inspect directories, search for challenge artifacts and locate the hidden flag.

The final submission reports the flag as captured. Exact file contents and challenge secrets are not reproduced in this public-safe case study.

## Phase 5 — Security interpretation

The lab illustrates:
1. Why exposed legacy services and missing patches can create material attack paths.
2. Why detection and remediation are important even when exploitation is only demonstrated in a controlled course setting.
3. Why security findings need clear supporting evidence and should be described without inflating lab experience into employment.
4. How reconnaissance, access validation and post-access investigation connect as one workflow.

## Validation limits

- The original presentation and its embedded screenshots are primary evidence; no new exploitation test was performed for this documentation.
- The source records a reported completed CTF challenge but does not establish independent zero-guidance exercise design.
- This repository intentionally excludes exploit binaries, sensitive outputs, raw video, identifying information and unreviewed screenshots.
