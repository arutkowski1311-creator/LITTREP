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

A companion specification — [`docs/clinical-intelligence-engine.md`](docs/clinical-intelligence-engine.md) —
defines a portable, model-agnostic workflow for generating recurring Medical Affairs
intelligence briefings across neuro-oncology, epilepsy, and LITT. It runs in two stages
(a 6-month baseline scan, then a 4-week surveillance scan for what's new) and standardizes
how each publication is scored, interpreted, and rolled up into an executive report.

## Important

The NeuroBlate System is a surgical tool and is not a treatment for any specific disease
state or condition. This tool produces process documentation for clinician reference only —
it does not replace the formal operative report and does not describe clinical outcomes.
Rx Only.
