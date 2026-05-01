# IR War Room — Incident Command Centre

A single-file, browser-based incident response command dashboard for cybersecurity teams. No server, no install, no dependencies — open `ir_cc.html` and you're live.

![Version](https://img.shields.io/badge/version-4.0-blueviolet) ![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg) ![Zero Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)

---

## What it does

IR War Room gives your incident response team a shared command interface during a live incident. Configure the incident in 60 seconds, then run through structured playbooks with your full bridge team — tracking actions, IOCs, blockers, decisions, and regulatory clocks in one place.

---

## Features

### Setup
- **8 threat type playbooks** — Ransomware, Data Leakage, Malware/Trojan, BEC/Email Fraud, Insider Threat, DDoS, Phishing/Credentials, Unauthorised Access
- **Incident details** — IR reference, severity (P1/P2/P3), discovery method, affected systems, data at risk
- **Bridge team assembly** — quick-add buttons for IC, SOC, IT Ops, CISO, Legal/DPO, Finance, HR, Comms, NOC
- **Logo upload** — add your company and customer logos (PNG/SVG/JPG)

### War Room Dashboard
- **Live elapsed timer** — tracks total incident duration from activation
- **Severity adjuster** — escalate or de-escalate P1/P2/P3 mid-incident, updates UI theming
- **Phase tracker** — 5-phase IR lifecycle (Detect → Contain → Eradicate → Recover → Post-Incident) with click-to-jump navigation

### Action Management
- Pre-loaded, owner-assigned actions for each phase and threat type
- Mark actions as done, waiting, or critical
- Add custom actions at any time
- Advance to the next phase with one click

### IOC Tracker
- 10 IOC types: IP Address, Domain, URL, File Hash, Email, File/Path, Registry Key, CVE, BTC Wallet, Other
- Confirmed / Unconfirmed confidence tagging
- Source attribution per IOC
- Filter by type; running count in header

### Team & Coordination
- Bridge team status cycling (Online / Away / Offline)
- Blockers / Waiting For list
- Decisions Needed list
- All items individually resolvable and removable

### Regulatory Clocks
Threat-specific countdown timers appear automatically:
- **Ransomware / Data Leakage** — ICO 72-hour GDPR breach notification window
- **BEC** — 2-hour bank wire recall golden window + ICO 72hr if ATO with personal data

### Activity Log
- Timestamped live log auto-populated by all actions (phase changes, action completions, etc.)
- Manual free-text log entries

### Export
- **HTML report** — full formatted incident report, ready to share or archive
- **CSV export** — structured incident data for ticketing systems or post-incident review

---

## Usage

1. Download `ir_cc.html`
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari)
3. Fill in the setup screen — threat type, incident details, initial team
4. Click **INITIATE INCIDENT RESPONSE**
5. Work through the phases with your team

Everything runs locally in the browser. No data leaves the machine.

---

## Threat Playbooks

| Threat Type | Regulatory Clock | Notes |
|---|---|---|
| Ransomware | ICO 72hr (if personal data) | Includes payment decision workflow |
| Data Leakage | ICO 72hr | GDPR Article 33 breach register step |
| Malware / Trojan | — | Banking trojan variant included |
| BEC / Email Fraud | 2hr bank recall + ICO 72hr | Finance Director bridge mandatory |
| Insider Threat | ICO 72hr (if personal data) | HR/Legal covert monitoring guidance |
| DDoS / DoS | — | ISP upstream null-route workflow |
| Phishing / Credentials | ICO 72hr (if ATO with personal data) | AiTM session hijack steps |
| Unauthorised Access | ICO 72hr (if personal data accessed) | Dwell time, SIEM gap analysis |

Each playbook covers 5 phases with pre-loaded actions, owner assignments, default blockers, and decisions.

---

## Browser Support

Any modern browser with ES6 support. No polyfills required.

---

## License

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This project is licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

You are free to:
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose

Under the following terms:
- **Attribution** — You must give appropriate credit to **Jestie**, provide a link to the license, and indicate if changes were made. You may not imply that Jestie endorses you or your use.
- **No false ownership** — You may not present this work as your own without crediting the original author.

See the full license text in [LICENSE](LICENSE) or at [creativecommons.org/licenses/by/4.0](https://creativecommons.org/licenses/by/4.0/).

---

## ☕ Support

If this tool saves you time during an incident, consider buying me a coffee!

**[☕ Buy me a coffee](https://paypal.me/jestie129)**

Designed by **Jestie**
