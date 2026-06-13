### 20. Patient Throughput: Legacy Versus Verified

How a cohort of patients flows to outcomes under the legacy path and under the
verified path, with the edge labels carrying the volume at each split. A weighted
flowchart is correct because it shows how work divides and converges while keeping
every color under the strict palette. Reproduced in the compiled LaTeX narrative
as a matching colored TikZ figure (palette: black, grayscales, #EBCB8B, #D08770,
#8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'},'flowchart':{'curve':'basis','nodeSpacing':30,'rankSpacing':52,'htmlLabels':true}}}%%
flowchart LR
  COH["Patient cohort"]:::n1
  LEG["Legacy path"]:::risk
  VER["Verified path"]:::act
  HARM["Preventable harm"]:::risk
  GOOD["Protected outcome"]:::hope
  COH -->|"share A"| LEG
  COH -->|"share B"| VER
  LEG -->|"higher error"| HARM
  LEG -->|"residual"| GOOD
  VER -->|"contained at gates"| GOOD
  VER -->|"rare, escalated"| HARM
  classDef act fill:#8B2E3F,stroke:#000000,stroke-width:1.4px,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,stroke-width:1.2px,color:#1A1505
  classDef risk fill:#D08770,stroke:#000000,stroke-width:1.2px,color:#1A0A04
  classDef n1 fill:#F2F2F2,stroke:#333333,stroke-width:1.1px,color:#111111
```
