### 16. The Widening Capability-Regulation Gap

Technology capability is advancing faster than the rules that govern it, and the
distance between the two is where preventable harm accumulates. The Act is the
bridge that closes the gap. A two-track flowchart is correct because it contrasts
two trajectories over time and the single instrument that joins them. Reproduced
in the compiled LaTeX narrative as a matching colored TikZ figure (palette: black,
grayscales, #EBCB8B, #D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'},'flowchart':{'curve':'natural','nodeSpacing':28,'rankSpacing':46,'htmlLabels':true}}}%%
flowchart LR
  subgraph CAP["Capability (rising fast)"]
    direction LR
    C1["Physical AI"]:::n2 --> C2["Surgical humanoids"]:::n2 --> C3["Autonomous pipelines"]:::n2
  end
  subgraph REG["Regulation (lagging)"]
    direction LR
    R1["Legacy CFR"]:::n1 --> R2["Guidance only"]:::n1 --> R3["Gap"]:::risk
  end
  ACT["H. R. 9510<br/>closes the gap"]:::act
  GOAL["Patients protected now"]:::hope
  C3 --> ACT
  R3 --> ACT
  ACT --> GOAL
  classDef act fill:#8B2E3F,stroke:#000000,stroke-width:1.4px,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,stroke-width:1.2px,color:#1A1505
  classDef risk fill:#D08770,stroke:#000000,stroke-width:1.2px,color:#1A0A04
  classDef n1 fill:#F2F2F2,stroke:#333333,stroke-width:1.1px,color:#111111
  classDef n2 fill:#D9D9D9,stroke:#222222,stroke-width:1.1px,color:#111111
```
