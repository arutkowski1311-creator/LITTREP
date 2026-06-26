# Feedback roadmap

Review notes on `index.html` and their status.

## Indications & clinical content
1. ✅ **Newly diagnosed glioma** — added a separate *Newly diagnosed glioma (lower-grade)*
   indication (distinct from the existing *Newly diagnosed glioblastoma*), with its own
   clinical context, evidence, refs, and follow-up.
2. ✅ **More epilepsy foci** — handled via the new anatomical-target field (decision: keep
   MTLE + "drug-resistant epilepsy (other)" and let the target capture name the focus,
   e.g. corpus callosum).
3. ✅ **Anatomical target(s)** — new builder section: repeatable **Side + Region** rows plus
   a free-text "anatomical detail / approach" box. Renders as an "Anatomical target(s)"
   metadata box on the report and a line on the deck.

## Device / procedure capture
4. ✅ **Trajectories** — replaced the single-trajectory checkbox with a repeatable
   **count + per-trajectory direction** list. Flows into the leadstrip (`targets·traj`),
   narrative, procedure insights, and the deck.
5. ✅ **Robotic probe driver** — now a normal metadata box alongside Indication / Probe /
   Date, not a standalone pill.

## Report
6. ✅ **Imaging in PDF export** — a print-only gallery renders **all** images (pre/intra/post)
   with captions; the interactive viewer is hidden in print.
7. ✅ **Post-LITT follow-up** — now a builder checklist, pre-checked per indication; the
   report and deck render only the checked items. Case-factor triggers still add
   case-specific points.
8. ✅ **Patient presentation** — single image set; thermometry video hidden in patient view.

## Physician edition (restructured)
9. ✅ **Procedural Notes** — renamed from "From the performing surgeon"; flat bullets (no
   subtitles), a kept **Recommended follow-up** subtitle, and a free-text box where each
   line becomes a bullet. Visible to performing + referring audiences.
10. ✅ **Full parity, mobile-optimized** — the stripped-down "physician mode" was removed.
    *Save Case* now downloads a self-contained copy of the whole app with the case
    embedded; it opens as the full, responsive builder on any phone or laptop.

## Builder UX
11. ✅ Removed the "Read this as" switch from the report. Builder bottom bar is now two rows:
    **Performing Physician · Referring Physician · Presentation Deck · Patient**, then
    **Export PDF · Save Case**. The `.pptx` deck export is a contextual button shown in the
    Presentation Deck view. *Save* (to this browser) lives in the Saved cases group.
12. ✅ **Cross-platform** — responsive layout for phone + laptop; smoke-tested headless.

## Round 3 — structure overhaul
- ✅ **Indications** replaced with the 12-item list (newly/recurrent glioblastoma,
  newly/recurrent lower-grade glioma, brain metastasis, radiation necrosis, meningioma,
  other intracranial tumor, MTLE, hypothalamic hamartoma, focal epilepsy, corpus callosotomy).
- ✅ **Target location** rebuilt: multi-select **Region** (20, grouped), single **Side**
  (Left/Right/Bilateral/Midline), multi **Orientation** (18), multi **Functional descriptor**
  (8). Renders as a 4-line block on the report + deck.
- ✅ **Removed** Procedure insights, Emerging science, Post-LITT follow-up watch list, and
  Case factors (builder, report, deck).
- ✅ **Procedure summary** added: Procedure (one of three), Technical highlights (checkboxes),
  Immediate outcome (checkboxes) — on report + deck.
- ✅ **Additional observations** replaces Procedural notes: free text, each line a bullet.

## Distribution — options (see README / discussion)
- Host `index.html` as a static page (GitHub Pages, Netlify, internal server) — it's a
  single self-contained file, so this is the lowest-friction path.
- Share the self-contained HTML directly (email / file) — *Save Case* produces exactly this.
- Optionally wrap as an installable PWA later for an app-like home-screen experience.
