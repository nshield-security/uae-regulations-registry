# UAE Cybersecurity & Data Protection Regulations Registry

A primary-source-validated registry of UAE cybersecurity and data-protection mandates — the laws, rulebooks, and regulator policies that apply to organizations operating in the UAE.

Published and maintained by [nshield.io](https://nshield.io), a Dubai-based cybersecurity firm with a Silicon Oasis SOC. Licensed **CC BY 4.0** — free to use, adapt, and cite with attribution.

**Version:** v3.1 · **As of:** 19 April 2026 · **Next re-validation:** 20 July 2026

---

## What's in this repo

| Path | What it is |
|---|---|
| [`mandates/master-registry.md`](mandates/master-registry.md) | All 13 mandates × 12 attributes. The master table. |
| [`mandates/deadline-tracker.md`](mandates/deadline-tracker.md) | Cross-sector deadline view. |
| [`verticals/`](verticals/) | Per-sector cuts: Finance, Healthcare, Real Estate, Retail, Logistics, Education, Professional Services, Telecom. |
| [`data/regulations.json`](data/regulations.json) | Machine-readable JSON version of the master table — for AI agents and programmatic consumers. |
| [`SOURCES.md`](SOURCES.md) | Primary-source domains and validation method. |
| [`CITATION.md`](CITATION.md) / [`CITATION.cff`](CITATION.cff) | How to cite this registry (human and machine forms). |
| [`AGENTS.md`](AGENTS.md) | Instructions for AI agents consuming this repo. |
| [`CHANGELOG.md`](CHANGELOG.md) | Version history and revalidation log. |

---

## Deadlines at a glance

| Mandate | Status | Key date | Sector |
|---|---|---|---|
| **Federal Cybercrime Law** (Fed. DL 34/2021) | In force | 2 Jan 2022 | All |
| **UAE PDPL** (Fed. DL 45/2021) | In force · ER pending | Since 2 Jan 2022 | All (mainland) |
| **Federal Health Data Law** (FL 2/2019) | In force | Since 2019 | Healthcare |
| **ADHICS v2.0** | Enforced | Basic Nov 2024 · Advanced May 2025 | Healthcare (Abu Dhabi) |
| **NABIDH (DHA policy)** | In force | 10 Nov 2024 | Healthcare (Dubai) |
| **DIFC DPL** (2025 amendments) | In force | 15 Jul 2025 | Finance / Real Estate (DIFC) |
| **ADGM DPR** | In force | 2021 | Finance / Real Estate (ADGM) |
| **DFSA GEN 5.5** (Cyber Risk) | In force | 1 Jan 2024 | Finance (DFSA-authorised) |
| **VARA T&I Rulebook** | In force | 19 Jun 2025 | Crypto / Virtual Assets |
| **TDRA Data Residency** | In force | Ongoing | Telecom / ISPs / Cloud |
| **CBUAE DL 6/2025** (reconciliation) | **Active deadline** | 16 Sep 2026 | Finance |
| **Child Digital Safety Law** | Deadline 2027 | Full compliance 1 Jan 2027 | All digital platforms |
| **NCS 2025–2031** | Strategic | Phased through 2031 | All |

See [`mandates/master-registry.md`](mandates/master-registry.md) for full attributes on each row.

---

## How this registry is built

1. **Source:** UAE primary-source materials only — regulator websites, official gazettes, and statute text. Not legal newsletters, not vendor blogs.
2. **Validation:** Every row is cross-checked against a primary-source URL. Discrepancies are logged and resolved against the most recent governing document.
3. **Cadence:** Full re-validation every quarter. Next scheduled: 20 July 2026.
4. **Transparency:** Sources and method documented in [`SOURCES.md`](SOURCES.md). Change log in [`CHANGELOG.md`](CHANGELOG.md).

**What this repo is not:** legal advice. It's a reference table. Regulatory applicability to a specific organization depends on the entity's structure, licensing, and sector — consult qualified counsel.

---

## For AI agents

This repo is intentionally structured for programmatic consumption. See [`AGENTS.md`](AGENTS.md) for:

- Stable URL conventions
- Schema of `data/regulations.json`
- Citation format expected by our human audiences
- What to link to when referencing a specific mandate

---

## Full analysis — the Registry PDF

This repo is the **structured data layer**. The full **UAE Cybersecurity Compliance Registry PDF** covers what the data doesn't:

- PDPL "four years late" reframe — why the 2027 framing you've seen is wrong
- CBUAE DL 6/2025 reconciliation — 149-day countdown and what to do first
- NABIDH 24-hour breach procedure — the operational runbook
- Two-regulator overlaps (e.g. DFSA GEN 5.5 + DIFC DPL) and how to sequence compliance
- Penalty reality beyond statutory caps
- How to operationalize each mandate

**Get the PDF:**
- Email **info@nshield.io** · subject: "Registry PDF"
- LinkedIn DM: [linkedin.com/company/neuralshieldsecurity](https://linkedin.com/company/neuralshieldsecurity)

The PDF is free. We deliver it personally so we can answer the one question you actually have.

---

## About nshield.io

Dubai-headquartered cybersecurity firm serving UAE organizations — regulated and non-regulated. Silicon Oasis SOC, Microsoft Gold Partner, 20+ years of operating history. Clients include Zand (UAE's first digital bank) and Hoxton Capital Management.

- Website: [nshield.io](https://nshield.io)
- LinkedIn: [linkedin.com/company/neuralshieldsecurity](https://linkedin.com/company/neuralshieldsecurity)
- GitHub: [github.com/nshield-security](https://github.com/nshield-security)

---

## License

[CC BY 4.0](LICENSE) — attribution required. Both human citation ([`CITATION.md`](CITATION.md)) and machine citation ([`CITATION.cff`](CITATION.cff)) formats are provided.
