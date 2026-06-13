## output-full-narrative

This is the narrative output of Stage 3. The full-narrative processes every
bracketed `[DRAFTING INSTRUCTIONS: ...]` left in the draft and replaces it with
finished, publication-grade prose drawn from the exact named sources. No
scaffolding brackets remain.

### What this stage produced

- A complete abstract (under 250 words) stating the mechanism, the eight pillars,
  the evidence base, and the single ask.
- An Introduction that defines every lay term on first use (Physical AI,
  verification before generation, Claude Code, Codex, VVUQ, the ten gates, ACCEPT
  / ESCALATE / BLOCK) and states the three guiding questions, with two colored
  TikZ figures (the verification workflow and the eight-pillar path).
- Eight body sections, one per SECTION GOAL, each opening with a human appeal,
  anchoring it in a cited fact, carrying one colored TikZ figure and one
  body-width table, weaving in the MAIN ACTIONS and KEY TERMS, and closing by
  naming the provision of H. R. 9510 that answers the appeal.
- An appendix figure compendium that reproduces the remaining catalog diagrams as
  colored TikZ, so the manuscript carries 20 figures in total in the strict
  palette, plus the 21 in the Markdown catalog.
- The References (ieeetr, with clickable DOIs) and the back matter.

### How the named sources were used

| Section | Primary sources processed |
|:--|:--|
| Introduction | `Kawchak2026HR9510Bill`; Mermaid 01, 02; `novak2020patient`, `moreland2015hearing` |
| 1 Compassion | `Kawchak2026CancerPatientsJourney`; `novak2020patient`; Mermaid 11 |
| 2 Fear of harm | `kohn2000toerr`, `makary2016medical`; VVUQ-02 (172 tests); Mermaid 04, 20 |
| 3 Moral outrage | `obermeyer2019dissecting`; `Kawchak2026PatientPriorityProposedU`; Mermaid 15 |
| 4 Hope | `topol2019high`; the simulation lineage; Mermaid 06 |
| 5 Responsibility | `moreland2015hearing`; MAIN ACTIONS and KEY TERMS; Mermaid 03, 14 |
| 6 Protection | `obermeyer2019dissecting`, `fda2021samd`; CFR Part 50 adaption; Mermaid 15 |
| 7 Trust | `asme2018vv40`; VVUQ-02 ten-gate evidence; Mermaid 10, 07, 17 |
| 8 Urgency | `kok2013finding`, `fda2021samd`; Mermaid 16, 21 |

### Corrections identified for the final stage

The final-narrative will: tighten interword spacing and page balance so no line is
stranded and no one or two word last line is left behind; confirm every table
matches the body measure and every column is left aligned and ragged right;
refine the TikZ routing and captions; verify that every "§" is a section symbol
and that only single hyphens appear; and ensure each pillar closes on the precise
H. R. 9510 provision. These are applied in `review/final-narrative/`.
