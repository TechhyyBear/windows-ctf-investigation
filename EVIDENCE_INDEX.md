# Evidence index — Career Simulation 3

**Publication format:** Text-only GitHub case study. The original video and screenshots are retained privately and are not required to complete the repository.

**Primary original:** `Career Simulation 3 - Final.mp4` (approximately 11 minutes 7 seconds), the submitted QuickStart / University of New Mexico guided CTF video.

## Evidence categories

- **Shown:** Visible lab configuration, terminal screenshot, or session in sampled original video scenes.
- **Presented:** Narrative, slide, or student-stated result, not independently rerun.
- **Interpretation:** Security lesson derived from the lab without asserting professional attack, defense, or incident response.

| Phase | Original evidence | Supported conclusion |
| --- | --- | --- |
| Approach | Plan includes Kali/Windows setup, Nmap, controlled Metasploit, post-access investigation | Guided, authorized exercise |
| Lab networking | VirtualBox Quickstart NAT network with DHCP and `10.0.2.0/24` | Isolated learning environment |
| Reconnaissance | Kali Nmap service/vulnerability-script output | Scanning of an intentionally vulnerable Windows target |
| Controlled access | Metasploit workflow references SMB/EternalBlue/MS17-010 lab path | Authorized exercise with vulnerable target |
| Session evidence | A Meterpreter session and Windows shell investigation shown in submitted presentation | Lab access documented, not independent exploit engineering |
| Host investigation | Windows directory/file exploration described and shown | Guided host-artifact search |
| Completion | Final slide declares `FLAG CAPTURED!` | Student-reported challenge completion, not independently reproduced in this portfolio update |

## An important outcome limit

A later section of the video shows a Windows `download` command that was not recognized and a Meterpreter operation reported as `skipped`. Do not describe this episode as proof of a newly successful file transfer. The student's reported challenge completion and the result of that particular transfer command are distinct claims.

## Why original media is withheld

The recording includes participant imagery, system identifiers, and potentially sensitive terminal output. It remains in private training/source records. No personal portrait, passwords, raw flag, exploit binaries, or original full-frame terminal output is reproduced here.

This is **guided coursework**. It does not document an unauthorized intrusion, production security incident, paid pentest, independent exploit development or a universally applicable EternalBlue technique.

## Decision: No screenshots

On November 20, 2026, the project operator chose to finish the GitHub repository as a **documentation-only case study**. Earlier screenshot selection/review records in Git history and private Drive are historical, not unresolved required tasks. No media upload or lab rerun is required for the documented-scope portfolio.


## Portfolio presentation decision — optional visuals

**Current presentation choice (supersedes the November 20 'no screenshots' requirement):** Text-first case study is complete at its documented scope. Zero images are required. At most one optional, independently privacy-reviewed technical screenshot may be added later; do not publish recognizable people, credentials, the raw flag, or unreviewed source video. Screenshot sourcing or rerunning is not required for the current portfolio.
