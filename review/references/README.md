# references - shared bibliography for the narrative review

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-EBCB8B.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Author works](https://img.shields.io/badge/Author%20works-40%2B%20entries-8B2E3F.svg)](.)
[![Supporting refs](https://img.shields.io/badge/Supporting%20refs-12-D08770.svg)](.)

This folder holds the two bibliographies that every narrative stage draws from.
The per-stage `references.bib` files in `../draft-narrative/`,
`../full-narrative/`, and `../final-narrative/` are assembled from these two
master files so that the same DOIs, URLs, and note fields are used consistently.

## Files

| File | Contents | Used by |
|:--|:--|:--|
| `author_works.bib` | 40+ prior works by Kevin Kawchak, including every H. R. 9510 bill version (v5.0 DOI 10.5281/zenodo.20619762) and the verification, platform, and simulation lineage. | All three narrative stages; the evidence-to-law lineage figure. |
| `narrative_refs.bib` | The five advocacy-science references carried verbatim from the prompt BACKGROUND block, plus accurate external evidence (To Err Is Human, Makary 2016, Obermeyer 2019, Topol 2019, the FDA AI/ML SaMD Action Plan, ASME V&V 40-2018, the Statutory PAYGO Act). | All three narrative stages; the emotion-and-evidence pairings. |

## How each emotional pillar is anchored

The narrative pairs every felt appeal with a credible citation, following the
BACKGROUND "balancing act" of emotion and evidence:

| Section | Emotional pillar | Anchoring evidence |
|:--|:--|:--|
| 1 | Compassion and empathy | `novak2020patient`, the author's patient-journey work |
| 2 | Fear of preventable harm | `kohn2000toerr`, `makary2016medical` |
| 3 | Moral outrage | `obermeyer2019dissecting` (unequal access and bias) |
| 4 | Hope | `topol2019high`, the author's simulation lineage |
| 5 | Responsibility and duty | `moreland2015hearing` (testimony and the legislative record) |
| 6 | Protection of vulnerable people | `obermeyer2019dissecting`, `fda2021samd` |
| 7 | Trust and reassurance | `asme2018vv40`, the VVUQ-02 ten-gate evidence |
| 8 | Urgency | `kok2013finding` (fear plus self-efficacy), `fda2021samd` |

## Sources used from other directories (Rule 6)

- `author_works.bib` is the repository's existing master list of the author's
  Zenodo and preprint records; it is consumed unchanged.
- `narrative_refs.bib` reproduces the BibTeX block of
  `../prompts/prompt-narrative.md` (BACKGROUND references) and adds the external
  sources named above from their public DOIs.

## License

Released under CC BY 4.0. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
