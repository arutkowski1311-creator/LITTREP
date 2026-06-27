# Clinical Intelligence Report — Surveillance Scan

**Date:** 2026-06-27 · **Mode:** Surveillance (delta) · **Window:** 2026-04-27 → 2026-06-27 (trailing 2 months)
**Counts:** ~14 in-window candidates screened · **6 added** · **1 updated** · 6 skipped (already in database)
**Database now:** 37 findings · [`database.json`](database.json) · [`dashboard.html`](dashboard.html)
**Prior report:** [2026-06-26-baseline.md](2026-06-26-baseline.md)

> Orientation: This is the first surveillance run, one day after the 24-month baseline, so the
> 2-month window sits *inside* the baseline window — the dedup engine correctly **skipped** the
> 31 baseline items and most re-encountered evidence. The LITT-specific, glioma, and
> epilepsy-surgery domains returned **no new in-window items** (an expected, valid result for a
> narrow niche window). All genuinely new findings are adjacent/competitive, clustered around
> **ASCO 2026** (May 29–Jun 2) and a **June 18 Novocure** readout. Egress blocks on publisher
> pages mean most figures are cross-source corroborated rather than masthead-confirmed; those
> items are flagged `partial`.

---

## What changed since the baseline

**1 update to an existing item:**
- **Vorasidenib / INDIGO** — ASCO 2026 extended follow-up (2026-05-31): median PFS deepened to
  **44.1 months**; only 23.8% required next intervention. Reinforces (does not change) the
  drug-first pathway in grade 2 IDH-mutant glioma — a continued mild **headwind** for LITT in
  that subgroup. *(Updated in place; `partial`.)*

**6 new items added:**

| # | Development | Date | Clinical | LITT business |
| --- | --- | --- | --- | --- |
| 1 | **ROADS phase 3** — Cs-131 tiles (GammaTile) vs post-op SRT, resected brain mets | 2026-05-30 | ★4 | **5 ▼ headwind** |
| 2 | **TTFields TRIDENT (EF-32)** phase 3 — earlier TTFields in GBM **misses** OS | 2026-06-18 | ★3 | 4 ▲ tailwind |
| 3 | **NCCN v2.2026** — CSF liquid biopsy for biopsy-infeasible HGG/GBM | 2026-06-17 | ★3 | 5 ▼ headwind |
| 4 | **JCOG1703 (MACS)** — carmustine wafers add no survival benefit (negative) | 2026-05-31 | ★2 | 3 ▲ tailwind |
| 5 | **Zeta Surgical** FDA 510(k) — frameless AI navigation + biopsy instruments | 2026-05-01 | ★1 | 4 ■ neutral |
| 6 | **ClearPoint Neuro** — 10-yr focused-ultrasound / BBB partnership | 2026-05-27 | ★1 | 3 ▼ headwind |

---

## Executive Summary

A quiet but not empty window. The single most strategically weighted item is **ROADS**
(ASCO 2026): a randomized phase 3 showing intraoperative Cs-131 tile brachytherapy (GammaTile)
cut 12-month surgical-bed recurrence from ~12% to ~1% and improved survival vs post-op SRT in
**operable** brain metastases — *with no excess radiation necrosis*. That strengthens a
"treat-locally-at-resection" competitor and blunts part of the post-SRS salvage funnel that
feeds LITT, though LITT's core niche (deep/inoperable lesions, biopsy-proven radiation
necrosis) is not what ROADS addressed.

Offsetting that, **TRIDENT** (TTFields started earlier in newly diagnosed GBM) **missed** its OS
endpoint (17.7 vs 17.5 mo; HR 0.953; p=0.519) — a competing modality failing to expand upfront,
a mild tailwind. **JCOG1703** similarly showed carmustine (Gliadel) wafers add nothing to modern
chemoradiation — another competing *local* therapy stalling.

Two watch-items shade against LITT at the margins: the **NCCN CSF liquid-biopsy expansion**
offers a non-surgical molecular diagnosis for inoperable HGG/GBM (erodes a diagnostic reason to
intervene in a subset overlapping diagnose-and-ablate referrals), and **ClearPoint's
focused-ultrasound partnership** signals a LITT rival diversifying into non-thermal BBB
intervention (long-horizon). **Zeta Surgical's** frameless AI navigation/biopsy clearance is
competitive-adjacent on the targeting layer, direction-neutral.

## Top 5 developments this run
1. ROADS phase 3 (GammaTile vs SRT) — **headwind**, the run's most consequential item.
2. TTFields TRIDENT negative phase 3 — mild **tailwind**.
3. NCCN CSF liquid-biopsy expansion — **headwind** / watch.
4. JCOG1703 carmustine-wafer negative phase 3 — mild **tailwind**.
5. ClearPoint focused-ultrasound partnership — long-horizon **headwind**.

## Most important competitive news
ROADS strengthens an intraoperative-radiation competitor for resectable mets; ClearPoint and
Zeta both extend the device-competitive perimeter around LITT (FUS/BBB; frameless navigation).

## Most important FDA / regulatory activity
Zeta Surgical 510(k) (navigation + biopsy instruments). NCCN CNS v2.2026 guideline expansion
(CSF molecular profiling). No new LITT-platform clearance, label change, or coverage decision
in-window.

## Areas of controversy / things to verify
- ROADS sample size differs across outlets (204 analyzed vs 230 randomized) and OS is immature
  (~13-mo follow-up); peer-reviewed manuscript pending. Flagged `partial`.
- TRIDENT, JCOG1703 figures are topline/abstract-level (no peer-reviewed full data yet).
- Egress blocks left several **epilepsy** leads date-unverifiable (RNS postapproval study in
  *Neurology*; hypothalamic-hamartoma SRT in *Epilepsia*; a laser-callosotomy case report) and a
  LITT+cemiplimab trial registration (NCT07620548) date-unconfirmed — all **omitted** per the
  "verify or omit" rule; re-check next run with publisher access.
- Near-miss excluded: the LITT BBB-permeability mechanistic paper (*Neuro-Oncology*, 2026-04-13)
  fell 14 days before the window.

---

## Per-publication entries (added/updated this run)

Full structured records — citation, source URL, design, results, limitations, both score axes,
indication/strategy mapping, business levers, and `verified` flags — are in
[`database.json`](database.json) (filter the dashboard by **status = "new this run"**). Item IDs:
`roads-cs131-tiles-vs-srt-brainmets-asco2026`, `ttfields-trident-ef32-negative-2026`,
`nccn-csf-liquid-biopsy-biopsy-infeasible-hgg-2026`, `jcog1703-macs-carmustine-wafer-negative-asco2026`,
`zeta-surgical-navigation-510k-2026`, `clearpoint-focused-ultrasound-partnership-2026`; updated:
`vorasidenib-indigo-fda-2024`.

## References
See per-item `url` fields in [`database.json`](database.json). Primary sources include ASCO 2026
(LBA2000; abstracts #2001), Novocure investor relations (TRIDENT topline), NCCN CNS v2.2026
(via Belay Diagnostics), FDA 510(k) (Zeta Surgical), and ClearPoint Neuro / BioSpace.

---

*Integrity: balanced and non-promotional; established vs. promising vs. speculative distinguished.
Items flagged `partial` rely on cross-source corroboration (publisher/proxy blocks prevented
masthead confirmation) and should be verified before external use. Internal medical-affairs
reference only — not medical advice.*
