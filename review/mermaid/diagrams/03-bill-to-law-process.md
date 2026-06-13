### 03. The Bill-to-Law Process

How H. R. 9510 becomes law: introduction, committee referral and markup, hearings
with expert and patient testimony, floor passage in each chamber, reconciliation
of any differences, and enactment. A top-down flowchart is correct because the
legislative path is a staged process with a feedback loop at markup. Reproduced in
the compiled LaTeX narrative as a matching colored TikZ figure (palette: black,
grayscales, #EBCB8B, #D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'},'flowchart':{'curve':'monotoneY','nodeSpacing':34,'rankSpacing':40,'htmlLabels':true}}}%%
flowchart TB
  INTRO["Introduction<br/>H. R. 9510"]:::n1
  REFER["Committee referral"]:::n2
  HEAR["Hearings<br/>expert and patient testimony"]:::n2
  MARK{"Markup<br/>debate and amend"}:::act
  FLOOR["Floor passage<br/>House and Senate"]:::n3
  RECON["Reconciliation<br/>one final text"]:::n3
  LAW["Enacted Federal law"]:::hope
  INTRO --> REFER --> HEAR --> MARK
  MARK -->|reported| FLOOR --> RECON --> LAW
  MARK -.->|revise| HEAR
  classDef act fill:#8B2E3F,stroke:#000000,stroke-width:1.4px,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,stroke-width:1.2px,color:#1A1505
  classDef n1 fill:#F2F2F2,stroke:#333333,stroke-width:1.1px,color:#111111
  classDef n2 fill:#D9D9D9,stroke:#222222,stroke-width:1.1px,color:#111111
  classDef n3 fill:#BFBFBF,stroke:#000000,stroke-width:1.2px,color:#111111
```
