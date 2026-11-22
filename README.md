# Week 5 — Phishing, Malware Triage, Threat Intelligence & Incident Response

**Internship Program:** SOC Tier 1 / Tier 2 Analyst Track — DG Interns Hub  
**Submission Date:** November 2026  

---

## Repository & Folder Structure

```text
DG Interns Hub/
└── Week 5/
    ├── Notes/                  # 8 separate documents answering all Theoretical Part questions (Q1–Q8)
    ├── Writeups/               # Separate writeups for TryHackMe rooms & MTA / Blue Team challenges
    ├── Findings/               # Screenshots & JSON exports for Hands-On Tasks 1–4
    ├── Incident Report/        # 2–3 page Incident Response Report (INC-2026-W5-001)
    ├── Cheat Sheet/            # 12-entry IOC Triage Table & 1-Page Phishing Red-Flag Checklist
    ├── Week5_Report.pdf        # Consolidated Weekly PDF Report
    ├── Week5_Presentation_Report.pptx  # Weekly Summary Slide Deck
    └── README.md               # Structured overview of Week 5 work
```

---

## Summary of Completed Work

### 1. Theoretical Foundations (`Notes/`)
- **Q1:** NIST SP 800-61 Four-Phase Incident Response Lifecycle action matrix.
- **Q2:** Phishing taxonomy (Bulk, Spear, Whaling, Smishing, Vishing, BEC) and red-flag indicators.
- **Q3:** Deep dive into SPF, DKIM, and DMARC with real `Authentication-Results` pass/fail examples.
- **Q4:** Email header forensics (`Received` chain, `Return-Path`, `Reply-To`, `Message-ID`, `Authentication-Results`).
- **Q5:** IOC vs. IOA comparison and David Bianco's Pyramid of Pain.
- **Q6:** MITRE ATT&CK vs. Cyber Kill Chain comparison and mapping of 5 attacks from Weeks 2–4.
- **Q7:** Static vs. dynamic malware analysis, sandbox mechanics, and sample handling safety rules.
- **Q8:** Incident report architecture, P1–P4 severity tiers, and escalation SLAs.

### 2. Hands-On Labs & Threat Hunting (`Findings/` & `Writeups/`)
- **Task 1 — Phishing Analysis:** Inspected headers, authentication results, and defanged URLs across 3 `phishing_pot` samples (`sample-1.eml`, `sample-10.eml`, `sample-12.eml`) using MXToolbox, Python, urlscan.io, VirusTotal, and AlienVault OTX.
- **Task 2 — Safe Malware Triage:** Validated Windows Defender quarantine (`Virus:DOS/EICAR_Test_File`) and Sysmon `Event ID 11` telemetry using the EICAR test string; analyzed process trees, network IOCs, and ATT&CK mappings from 2 public sandbox reports.
- **Task 3 — MITRE ATT&CK Navigator:** Mapped 7 techniques observed across Weeks 2–5 (`T1046`, `T1110`, `T1190`, `T1566.002`, `T1059.001`, `T1136.001`, `T1053.005`) and exported both PNG screenshot and `week5_attack_layer.json`.
- **Task 4 — Atomic Red Team Emulation:** Snapshotted Windows VM, executed `T1059.001`, `T1136.001`, and `T1053.005`, verified Sysmon `Event ID 1` telemetry, documented detection gaps, and eradicated all test artifacts.

### 3. Reporting & Analyst Resources (`Incident Report/` & `Cheat Sheet/`)
- **Incident Report (`INC-2026-W5-001`):** Full timeline, ATT&CK mapping, IOCs, severity justification, and detection engineering recommendations.
- **Cheat Sheets:** 12-item *IOC Type – Where to Find It – Tool to Check It* reference table and a 1-page *Phishing Red-Flag Checklist*.
