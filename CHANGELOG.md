# Changelog

All notable changes to the UAE Regulations Registry are logged here. Dates are validation dates, not commit dates.

Format based loosely on [Keep a Changelog](https://keepachangelog.com). Registry versioning is semantic at the *data* level: MAJOR = new mandate added/removed, MINOR = row-level factual fix, PATCH = metadata or formatting.

---

## v3.1 — 19 April 2026

Baseline published on GitHub.

### Added
- **DFSA Cyber Risk Management** (GEN Module 5.5, effective 1 Jan 2024) — added to Master Registry and Finance vertical. Previously missing.
- **Professional Services** vertical — law firms, audit, consulting, marketing agencies.
- **Machine-readable data:** `data/regulations.json`.
- **Convention files** for AI agents: `AGENTS.md`, `CITATION.cff`.

### Changed
- **PDPL** — reframed from "deadline 1 Jan 2027" to "in force since 2 Jan 2022; 6-month compliance window when Executive Regulations publish (per Art. 56)". The 2027 framing was a misreading; PDPL has been enforceable since 2022.
- **Federal Cybercrime Law penalties** — corrected from "up to AED 5M" to accurate range "AED 100K–3M per offense + imprisonment; up to AED 2M for paid content dissemination".
- **DIFC DPL penalties** — specified correctly as "USD 25K (annual assessment) / USD 50K (DPIA / data sharing violations) + Art. 62 fines" rather than generic "USD 25K–50K per violation".
- **VARA Rulebook detail** — updated to cite T&I Rulebook (effective 19 Jun 2025): 72-hour breach (Rule H), annual TLPT, quarterly vulnerability scans, continuous monitoring.
- **NABIDH breach-notification window** — corrected to 24–48 hours (was previously cited as 72 hours in some places). ADHICS 72-hour references remain accurate.
- **CBUAE DL 6/2025** — reconciliation deadline explicitly called out as 16 Sep 2026.

### Data-integrity pass
99 cell-level fixes applied across the underlying Excel source (`UAE_Cybersecurity_Compliance_SMB_v2.xlsx`) in the run-up to this v3.1 release, covering every row of the Master Registry and all vertical tabs. Factual review by **Mujahid Hassan** (Sales Director, nshield.io).

---

## Revalidation schedule

- **Next full re-validation:** 20 July 2026
- **Cadence:** quarterly
- **Trigger for out-of-cycle updates:** publication of PDPL Executive Regulations, or any other governing instrument that materially changes a registry row

Intermediate primary-source checks are welcomed from the community — open an issue.
