# LaTeX-Source-Files-20

**Adverse Event Response Standard Operating Procedure** -- a single-column LaTeX template (number 20 of 30) in the *Oncology clinical trials* family.

- **Genre / perspective:** SOP (roles + numbered steps).
- **Built on INSPIRATIONS:** 07-humanoid adverse-event paper; VVUQ-05 Table 1; VVUQ-03 back matter.
- **Body style:** Linux Libertine.
- **DOI placeholder:** [`10.5281/zenodo.xxxxxxxx`](https://doi.org/10.5281/zenodo.xxxxxxxx) (replace `xxxxxxxx`).
- **Author:** Kevin Kawchak, CEO ChemicalQDevice, ORCID `0009-0007-5457-8667`.

## Files

```
LaTeX-Source-Files-20/
  main.tex
  tmpl20style.sty
  references.bib
  README.md
  orcid_icon.png
  sections/
    section-a.tex
    section-b.tex
    section-c.tex
    section-d.tex
    section-e.tex
    section-f.tex
```

## One section file per document section

This template uses **one `section-x.tex` file per document section** (rule 9); add a section by adding `sections/section-g.tex` and an `\input` line in `main.tex`.

| Section file | Document section |
|:--|:--|
| `sections/section-a.tex` | Purpose and scope |
| `sections/section-b.tex` | Roles and responsibilities |
| `sections/section-c.tex` | Procedure |
| `sections/section-d.tex` | Escalation and reporting |
| `sections/section-e.tex` | Records |
| `sections/section-f.tex` | Back matter (VVUQ-03) |

## Included per the rules

- One **image placeholder** based on the figure code of `papers/VVUQ-02/final-paper`.
- One **table** modeled on **Table 1** of `papers/VVUQ-05/final-bill`.
- The **back matter** from `papers/VVUQ-03/final-paper` (the parts that fit this genre).
- A **blank Keywords line** on the first page; the **DOI** on the cover and in the citation block.
- The green **ORCID logo** (`orcid_icon.png`) on the cover in place of the green `iD` text.

## Compile (Overleaf, pdfLaTeX)

```
pdflatex main
bibtex   main
pdflatex main
pdflatex main
```

## License

CC BY 4.0. Reproduced public-domain U.S. Government text is used under 17 U.S.C. § 105.
