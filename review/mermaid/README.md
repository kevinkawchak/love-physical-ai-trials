# mermaid - Stage 1: colored Mermaid figures

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-EBCB8B.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Figures](https://img.shields.io/badge/Figures-21-8B2E3F.svg)](diagrams/)
[![Palette](https://img.shields.io/badge/Palette-black%20%2B%20gray%20%2B%203%20theme-D08770.svg)](.)
[![Media](https://img.shields.io/badge/Media-Mermaid%20%E2%86%92%20colored%20TikZ-8B2E3F.svg)](.)

This directory is the output of **Stage 1** (sub-prompt
[`../sub-prompts/prompt-1-mermaid.md`](../sub-prompts/prompt-1-mermaid.md)). It
holds 21 professional, colored Mermaid figures that illustrate the narrative
review's eight emotional-pillar sections and its legislative argument. The
schedule requires 20+ figures and 20+ commits; this stage delivers 21, one commit
per figure file.

## Palette (strict)

Only black, grayscales, and the three theme colors are used, which keeps the
existing `#8B2E3F` paper template theme:

| Class | Fill | Text | Meaning |
|:--|:--|:--|:--|
| `act` | `#8B2E3F` | white | the Act, verification, human protection |
| `hope` | `#EBCB8B` | black | hope, benefit, accepted outcome |
| `risk` | `#D08770` | black | harm, risk, the legacy path |
| `n1` `n2` `n3` | `#F2F2F2` `#D9D9D9` `#BFBFBF` | black | inputs, steps, gates |

## Files

```
mermaid/
  README.md            (this file)
  output-mermaid.md    (catalog: all 21 figures embedded for GitHub rendering)
  diagrams/
    01-verification-before-generation.md   12-legislative-timeline.md
    02-eight-emotional-pillars.md          13-effort-impact-quadrant.md
    03-bill-to-law-process.md              14-reconciliation-gitgraph.md
    04-compounding-human-error.md          15-vulnerable-population-safeguards.md
    05-coalition-map.md                    16-urgency-capability-gap.md
    06-evidence-to-law-lineage.md          17-system-context.md
    07-ten-vvuq-gates.md                   18-composite-oversight-state.md
    08-annual-reporting-sequence.md        19-markup-testimony.md
    09-verification-decision-state.md      20-patient-throughput-flow.md
    10-trust-scaffolding.md                21-national-platform-capstone.md
    11-patient-journey.md
```

## Figure-to-section map

Each figure is reproduced as a colored TikZ figure in the compiled LaTeX
narrative, distributed across the manuscript as follows.

| Figure | Narrative slot |
|:--|:--|
| 01, 07, 09 | Introduction and trust (the verification mechanism) |
| 02 | Introduction (the reader's path) |
| 03, 14, 19 | Responsibility, urgency (the legislative process) |
| 04, 20 | Fear of preventable harm |
| 05, 13 | Coalition building and strategy |
| 06, 12 | Evidence-to-law lineage and timeline |
| 10, 17 | Trust and reassurance |
| 11 | Compassion and empathy |
| 15 | Protection of vulnerable people |
| 16 | Urgency |
| 08, 18, 21 | Framework and appendices |

## Sources used from other directories (Rule 6)

- Diagram families, spline and box discipline, and the professional-palette
  method: `Clinical-AI-Demos/tree/main/ai-outputs/output-01`.
- Subject matter (verification before generation, ten gates, the bill lineage):
  `../references/author_works.bib` and `cancer-automated/.../papers/VVUQ-02`.
- Build method and one-commit-per-file schedule:
  `single-prompt-bill/.../auto-bill-02`.

## License

Released under CC BY 4.0. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
