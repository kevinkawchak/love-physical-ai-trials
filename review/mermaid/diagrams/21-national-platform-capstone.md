### 21. The National Platform Capstone

The capstone shows how the six-step verification baseline extends to a national
Physical AI oncology trial platform, grouped into four phases, define, build,
verify, and govern, with the Act binding the whole. A phase-grouped flowchart is
correct because it scales the model to many connected components while keeping the
flow fluent. Reproduced in the compiled LaTeX narrative as a matching colored TikZ
figure (palette: black, grayscales, #EBCB8B, #D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111','clusterBkg':'#F2F2F2','clusterBorder':'#888888'},'flowchart':{'curve':'basis','nodeSpacing':28,'rankSpacing':46,'htmlLabels':true}}}%%
flowchart LR
  subgraph PH1["Define"]
    direction TB
    REQ["Clinical specification"]:::n1
  end
  subgraph PH2["Build"]
    direction TB
    GEN["Claude Code generation"]:::n2
    REV["Codex peer review"]:::n2
  end
  subgraph PH3["Verify"]
    direction TB
    GATE{"Ten VVUQ gates"}:::act
    SAFE{"Subgroup safeguards"}:::act
  end
  subgraph PH4["Govern"]
    direction TB
    AUD[("Audit trail")]:::n3
    REP["Public report"]:::hope
    FUND["Authorized funding"]:::hope
  end
  ACT["H. R. 9510"]:::act
  REQ --> GEN --> REV --> GATE
  GATE --> SAFE --> AUD --> REP
  REP --> FUND
  ACT -.->|binds| GATE
  ACT -.->|binds| SAFE
  ACT -.->|requires| REP
  classDef act fill:#8B2E3F,stroke:#000000,stroke-width:1.4px,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,stroke-width:1.2px,color:#1A1505
  classDef n1 fill:#F2F2F2,stroke:#333333,stroke-width:1.1px,color:#111111
  classDef n2 fill:#D9D9D9,stroke:#222222,stroke-width:1.1px,color:#111111
  classDef n3 fill:#BFBFBF,stroke:#000000,stroke-width:1.2px,color:#111111
```
