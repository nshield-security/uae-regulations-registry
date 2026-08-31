# Changelog

All notable changes to the UAE Regulations Registry are logged here. Dates are validation dates, not commit dates.

Format based loosely on [Keep a Changelog](https://keepachangelog.com). Registry versioning is semantic at the *data* level: MAJOR = new mandate added/removed, MINOR = row-level factual fix, PATCH = metadata or formatting.

---

## v4.2 — 31 August 2026 (ERRATA)

**Out-of-cycle errata release. Not a re-validation.** Two factual errors were found in v4.1 during an independent review of content built on this registry, verified against primary sources, and corrected. No mandate added or removed; no other row re-checked. `as_of` deliberately remains **2026-07-25** — it records the last full validation sweep, not this correction. Full re-validation remains scheduled for **20 October 2026**.

### Corrected

- **DIFC DPL — Autonomous Systems Officer was placed at the wrong regulation.** v4.1 stated that Consultation Paper 3/2026 puts "certification schemes and the Autonomous Systems Officer role" at **Regulation 11**. It does not. The **new Regulation 11** empowers the Commissioner to recognise accreditation and certification schemes. The **ASO sits at Regulation 10** — Reg 10.3.3 requires appointment for high-risk commercial autonomous systems — which CP3 strengthens. Corrected in `mandates/master-registry.md`, `verticals/finance.md` and `data/regulations.json`. Sources: DIFC press release 18 June 2026; Mayer Brown; Lexology; Waystone.
- **NCAP — the accreditation policy is published, not awaited.** v4.1's watch list said the formal policy was "awaited on csc.gov.ae". The UAE government portal (u.ae, updated **2 July 2026**) carries the framework and links the full policy, *Cyber Accreditation Program_V2.0.pdf*. Corrected in `README.md`.
- **NCAP — wording aligned to the official source.** v4.1 described NCAP as "restricting critical-infrastructure operators to accredited cybersecurity providers". The published wording is that it grants entities "the ability to work with provider entities who also conform to baseline cyber security requirements". Our phrasing was stronger than the instrument. Corrected in `mandates/master-registry.md` and `data/regulations.json`.

### Why released out of cycle

The changelog convention allows out-of-cycle updates when a governing instrument materially changes. A **factual error in a published asset** is a stronger trigger than that: the registry's value rests on being the source a reader can trust, and the machine-readable layer was wrong. Holding known-wrong facts for seven weeks to preserve a release cadence would be the wrong trade.

### Layers updated

`data/regulations.json` (v4.2, `errata_released` 2026-08-31), `mandates/master-registry.md`, `verticals/finance.md`, `README.md` (header + watch list), `CITATION.cff`, `CITATION.md`, `AGENTS.md`. The `.xlsx` source remains un-regenerated (outstanding since v4.0).

---

## v4.1 — 25 July 2026

Quarterly re-validation of all 14 mandates, run via three parallel primary-source research sweeps (federal / financial / health clusters) across the Apr–Jul 2026 window. Nine mandates unchanged; ten rows received factual additions. No mandate added or removed — per the data-semantics convention (MINOR = row-level factual fix), a minor bump. Metadata: version → v4.1, `as_of` 2026-07-25, `next_revalidation` 2026-10-20.

### Changed
- **PDPL** — regulator transition noted: the UAE Data Office is being absorbed into the new **Federal Authority for Artificial Intelligence and Data** (Cabinet decision announced 14 June 2026). Confirmed Executive Regulations still not issued as of 25 July 2026.
- **National Cybersecurity Strategy 2025–2031** — 2026 implementation note added: National Cyber Accreditation Programme (NCAP) rollout (policy published v2.0; see the 31 Aug 2026 correction note), Secure Supply Chain (SBOM) Program, Quantum Secure Program.
- **DIFC DPL** — flagged amended DP Regulations proposed via **Consultation Paper 3/2026** (18 Jun 2026; consultation closed 18 Jul 2026): AI-systems safety (Reg 10), new Reg 11 = Commissioner may recognise accreditation/certification schemes; ASO sits at Reg 10.3.3; enactment expected H2 2026.
- **DFSA GEN 5.5** — 2026 supervision notes added: mandatory Cyber Risk Self-Assessment via ePortal (Dear SEO letter 30 Jun 2026, due 24 Jul 2026); Dear SEO AI risk-management letter (4 Jun 2026); operational-resilience GEN section proposed via CP170 (final rules expected late 2026). Also added the DFSA GEN 5.5 row to the Deadline Tracker (previously in the Master Registry and Finance vertical but missing from the tracker).
- **ADGM Cyber Risk Management (GEN 3.5)** — noted FSRA Cyber Threat Notice to VASPs (30 Apr 2026) reiterating the 24-hour material-incident notification.
- **VARA** — 2026 enforcement wave noted: June 2026 actions against MX Global, CoinMENA, and Peken Global (KuCoin).
- **Child Digital Safety Law** — first implementing instrument added: Cabinet Resolution on children's social-media access (approved 18 Jun 2026): minimum age 15, enhanced safeguards for ages 15–16, personalized-advertising ban for minors, 12-month platform transition to mandatory age verification.
- **NABIDH** — enriched with related DHA standards: ST-11 (Health Information Assets Management During Facility Closure, Jul 2025) and ST-12 (Human Genetic and Genomic Data Governance, 28 Aug 2025).
- **TDRA** — scope note added: TDRA's Information and Digital Government Sector moved into the Federal Authority for Artificial Intelligence and Data (14 Jun 2026); telecom/spectrum regulation and residency requirements remain with TDRA.
- **CBUAE DL 6/2025** — 16 September 2026 reconciliation deadline confirmed as of 25 July 2026, no extension announced; no dedicated cyber/technology-risk regulation issued under the new law yet (pre-existing regulations remain in force via Art. 183).

### Added
- **README "Pending & watch (as of 25 July 2026)" section** — Federal Authority for AI and Data, PDPL Executive Regulations status, DIFC CP3/2026, DFSA CP170, NCAP, and the Riayati/NUMR integration mandate. Also fixed the stale README header (was v3.1 / 19 Apr) and corrected the mandate count to 14.
- **SOURCES.md "Known-unreliable sources" note** — naming SEO farms (itsecnow.com, eshieldconsulting.com, vesta-solutions.ae, bshsoft.com, muhami.ae) that publish fabricated PDPL Executive-Regulations claims, plus the additional primary sources checked this cycle.

### Validation method
Three parallel primary-source research sweeps (federal / financial / health), 25 July 2026, primary-source-first against regulator sites and rulebooks (difc.com, dfsaen.thomsonreuters.com, rulebook.centralbank.ae, rulebooks.vara.ae, alusra.gov.ae, uaelegislation.gov.ae, doh.gov.ae, dha.gov.ae, mohap.gov.ae, u.ae). See [`SOURCES.md`](SOURCES.md).

### Data layers updated
- Markdown tables (Master Registry, Deadline Tracker, Finance / Healthcare / Education / Retail / Telecom verticals) + `data/regulations.json` (bumped to v4.1, `as_of` 2026-07-25). README, SOURCES.md, CITATION.cff, and CITATION.md restamped. The `.xlsx` source not regenerated this cycle.

---

## v4.0 — 4 June 2026

ADGM Cyber Risk Management Framework added after live-source validation. The registry previously held only ADGM DPR 2021 (data protection) — the FSRA **cyber** framework was missing. Surfaced during a content fact-check. Per the data-semantics convention (MAJOR = new mandate added), this is a major bump.

### Added
- **ADGM Cyber Risk Management Framework (GEN Rule 3.5)** — added to Master Registry, Finance vertical, and Deadline Tracker. FSRA framework, binding since Jul 2025, full compliance from **31 Jan 2026**. Requires: a Cyber Risk Management Framework; ICT asset inventory classified by confidentiality & business criticality (incl. third-party); board/governing-body + senior-management accountability; cyber-risk assessment reviewed at least annually; technical controls (anti-malware auto-scanning, network security, least-privilege access); IT-service-provider/technology-contract requirements; **material cyber incident notification to FSRA within 24 hours**. Distinct from ADGM DPR 2021.

### Sources
- https://www.adgm.com/media/announcements/adgms-fsra-issues-cyber-risk-management-framework
- https://en.adgm.thomsonreuters.com/rulebook/gen-35-cyber-risk-management
- https://www.nortonrosefulbright.com/en/knowledge/publications/55179310/cyber-risk-management-in-the-adgm-an-analysis-of-the-new-regulatory-framework
- https://www.dts-solution.com/adgm-cyber-risk-management-what-firms-need-to-know-before-january-31-2026/

### Validation method
Web research 4 Jun 2026 against ADGM/FSRA primary announcement + ADGM Rulebook GEN 3.5 + independent legal analyses. The 24-hour notification, asset-classification, governance, third-party, and technical-control requirements were each cross-checked across multiple sources.

### Data layers updated
- Markdown tables (Master Registry, Finance, Deadline Tracker) + `data/regulations.json` (bumped to v4.0, `as_of` 2026-06-04). The `.xlsx` source (`UAE_Cybersecurity_Compliance_SMB_v2.xlsx`) not yet regenerated — refresh on next pass.

---

## v3.2 — 12 May 2026

VARA row corrections after primary-source re-validation against VARA Technology & Information Rulebook (rulebooks.vara.ae) and VARA Enforcement Rulebook.

### Changed
- **VARA breach notification** — now correctly specifies BOTH timeframes from Section H of the Technology & Information Rulebook:
  - 72 hours from detection for material cybersecurity events ("as soon as reasonably practicable and no later than 72 hours from detection")
  - 24 hours for personal data incidents (separate clause, triggered when data regulator or data subject is notified)
  - Previous v3.1 entry only cited 72-hour window.
- **VARA custody requirements** — corrected from "secure crypto wallets (MPC / cold storage)" (which read as if MPC or cold storage was mandatory) to "HSMs for critical key storage; risk-based hot/cold custody decisions; multi-sig where appropriate or VARA-mandated case-by-case." The actual rulebook (Section C, VA Wallet Management) requires risk-based analysis between hot/cold, mandatory HSM use for critical keys, and considers multi-sig case-by-case.
- **VARA testing requirements** — corrected from "annual TLPT" (which read as if TLPT was always required annually) to "annual third-party penetration testing required; TLPT (Threat-Led Penetration Testing / Red Team) may be mandated by VARA when necessary and proportionate." Annual third-party pentest is the baseline; TLPT is a separate uplift VARA can require.
- **VARA enforcement / penalty** — corrected from "License revocation" / "License revocation + fines" (which understated the toolset) to full Enforcement Rulebook spectrum: written reprimands, enforcement notices, cease-and-desist, scope limits, fines, suspension, AND revocation. Revocation is one tool among many, not the sole consequence.

### Sources
- https://rulebooks.vara.ae/rulebook/h-business-continuity-cybersecurity-events-and-risk
- https://rulebooks.vara.ae/sites/default/files/en_net_file_store/VARA_EN_169_VER20250519.pdf
- https://rulebooks.vara.ae/entiresection/493 (Enforcement)
- https://rulebooks.vara.ae/rulebook/c-va-wallet-management

### Validation method
Cross-referenced via Tavily research May 11–12, 2026, with quoted exact language from VARA primary sources. Earlier v3.1 wording was inherited from secondary summaries that compressed VARA's language unfaithfully.

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

- **Next full re-validation:** 20 October 2026
- **Cadence:** quarterly
- **Trigger for out-of-cycle updates:** publication of PDPL Executive Regulations, or any other governing instrument that materially changes a registry row

Intermediate primary-source checks are welcomed from the community — open an issue.
