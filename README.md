# Home Lab

A self-hosted lab environment used to practice detection engineering, incident triage, and blue team workflows against simulated attack techniques — built to develop hands-on SOC Analyst skills beyond day-to-day work experience.

## Environment

> _Fill in with your actual setup, e.g.:_
- **Hypervisor:** Proxmox / VMware Workstation / Hyper-V
- **Domain Controller:** Windows Server 2022
- **Endpoints:** 1–2x Windows 10/11 client VMs
- **Network:** pfSense/OPNsense for segmentation and logging
- **SIEM:** Microsoft Sentinel workspace, logs forwarded via AMA / Log Analytics agent
- **EDR:** Microsoft Defender for Endpoint (or SentinelOne, if licensed)

## Goal

Each project below simulates a specific attack technique (mapped to MITRE ATT&CK where applicable), then documents the detection logic, evidence, and analysis — written the way I'd hand off a finding to a team lead.

## Projects

| # | Project | Technique | Status |
|---|---------|-----------|--------|
| 01 | [AD Attack Detection](./projects/01-ad-attack-detection) | TBD (e.g. T1110 Brute Force) | 🚧 In progress |

## Notes

All environments are isolated and sanitized — no data, hostnames, or IPs from client or employer environments are used anywhere in this repo.
