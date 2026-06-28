# LITT Procedure Summary Builder

A single-file web app for generating **NeuroBlate® LITT (Laser Interstitial Thermal
Therapy)** procedure summaries for the clinical team. Everything runs in the browser —
no server, no data leaves the device. Built to work on both laptop and phone.

## What it does

`index.html` is a self-contained builder + report:

- **Builder** (left panel): facility/team directory, case + indication, device/console
  parameters, procedure insights, case factors, the performing surgeon's notes, imaging
  drop zones, thermometry clip, and sign-off. The directory and saved cases persist in
  the browser via `localStorage`.
- **Report** (right): a clinician-facing procedure summary that re-frames itself for four
  audiences — **Referring**, **Performing**, **Tumor board**, and **Patient** — with an
  imaging viewer, thermometry replay, clinical context, post-LITT follow-up, and
  indication-specific literature.
- **Tumor board deck**: exports a `.pptx` (via PptxGenJS) framing the case and evidence.
- **Physician edition**: a mobile-optimized HTML export the physician can complete and
  share.

The clinical reasoning, references, and follow-up content are driven by the selected
**indication** (recurrent glioma, newly diagnosed GBM, progressive brain metastasis,
radiation necrosis after SRS, mesial temporal lobe epilepsy, and other drug-resistant
epilepsy).

`samples/LITT_TumorBoard_Sample.pptx` is an example of the generated deck.

## Status

This is an iterating prototype. A running list of requested changes lives in
[`docs/feedback-roadmap.md`](docs/feedback-roadmap.md).

## Clinical Intelligence Engine

> **Canonical home: the [LITTLibrary](https://github.com/arutkowski1311-creator/LITTLibrary)
> repo.** The "LIT Library — Clinical Intelligence Hub" dashboard, its database, and the
> recurring scan now live there. The files under `reports/` and
> `docs/clinical-intelligence-engine.md` in this repo are the origin/working copy; ongoing
> updates should target LITTLibrary.

A companion specification — [`docs/clinical-intelligence-engine.md`](docs/clinical-intelligence-engine.md) —
defines a portable, model-agnostic workflow for generating recurring Medical Affairs
intelligence briefings across neuro-oncology, epilepsy, and LITT. It runs in two stages
(a baseline scan since 2020, then a trailing-2-month surveillance scan for what's new) and
standardizes how each finding is mapped to indications and scored on two axes
(clinical impact + LITT business impact) before being rolled up into an executive report.

## Important

The NeuroBlate System is a surgical tool and is not a treatment for any specific disease
state or condition. This tool produces process documentation for clinician reference only —
it does not replace the formal operative report and does not describe clinical outcomes.
Rx Only.
