### 17. System Context

The whole arrangement seen from a distance: the people (patient, legislator,
sponsor, independent reviewer) and the systems (the verified platform and the
public registry) and how they relate. Distinct node shapes carry the system
context lens without leaving the strict palette. Reproduced in the compiled LaTeX
narrative as a matching colored TikZ figure (palette: black, grayscales, #EBCB8B,
#D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'},'flowchart':{'curve':'cardinal','nodeSpacing':34,'rankSpacing':52,'htmlLabels':true}}}%%
flowchart LR
  PAT([Patient]):::n1
  LEG([Legislator]):::n1
  REV([Independent reviewer]):::n2
  subgraph PLAT["Verified Physical AI platform"]
    SPON["Sponsor operations"]:::n2
    GATE{"VVUQ gates"}:::act
    REG[("Public registry")]:::hope
  end
  PAT -->|enrolls, consents| SPON
  SPON -->|submits for checks| GATE
  GATE -->|certified record| REG
  REV -.->|peer review| GATE
  REG -->|transparent report| LEG
  LEG -->|enacts and funds| PLAT
  classDef act fill:#8B2E3F,stroke:#000000,stroke-width:1.3px,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,stroke-width:1.2px,color:#1A1505
  classDef n1 fill:#F2F2F2,stroke:#333333,stroke-width:1.1px,color:#111111
  classDef n2 fill:#D9D9D9,stroke:#222222,stroke-width:1.1px,color:#111111
```
