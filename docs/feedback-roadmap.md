# Feedback roadmap

Running list of requested changes to `index.html`, captured from review notes.

## Indications & clinical content
1. **Newly diagnosed glioma** — confirm/extend indications. (Note: a *Newly diagnosed
   glioblastoma* option already exists; open question is whether a separate
   newly-diagnosed / lower-grade glioma indication is wanted.)
2. **More epilepsy foci** — beyond MTLE and "drug-resistant epilepsy (other)," support
   additional/explicit seizure foci.
3. **Anatomical target(s)** — let the report state the brain region(s) being treated
   (location + anatomical reference, e.g. "left posterior + mid corpus callosum") and what
   the issue is. Example case: entire left posterior and mid corpus callosum ablated for
   epilepsy.

## Device / procedure capture
4. **Trajectories** — replace the single "single trajectory" checkbox with a real choice of
   the **number of trajectories** and the **direction** of each.
5. **Robotic probe driver** — stop rendering it as a standalone pill; make it a normal
   metadata box like Indication, Probe, and Date.

## Report
6. **Imaging in PDF export** — print/export must include **all** images, not just the
   currently selected (yellow/blue line) view.
7. **Post-LITT follow-up** — make it a list of **optional, selectable** items the surgeon
   can toggle, **defaulted based on the indication**.
8. **Patient presentation** — single image set only, **no video**.

## Physician edition (currently unprofessional — restructure)
9. Sections should be:
   - **Procedural Notes** (replaces "From the performing surgeon"), in the surgeon's own
     words.
   - The list of bullets — **no subtitles**.
   - **Recommended follow-up** — keep this subtitle.
   - A **free-text** spot that adds one or more bullets.
10. Physician edition should have **everything the regular report builder has**, just
    **mobile-optimized**.

## Builder UX
11. Remove the "Read this as" switch from the report level. The builder should already
    contain everything; add a row of audience buttons —
    **Performing Physician · Referring Physician · Presentation Deck · Patient** —
    then a second row: **Export PDF · Save Case** (save the file to the local
    computer/phone).
12. **Cross-platform** — must work on both laptop and phone.

## Distribution (open question)
- How to get this tool into physicians' hands so they can use it.
