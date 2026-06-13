### 01. Verification Before Generation Workflow

The core idea of H. R. 9510 in one figure: human investigators write the
specification, Claude Code generates candidate code, Codex performs independent
peer review, and a ten-gate VVUQ check decides ACCEPT, ESCALATE, or BLOCK before
anything executes on a patient. A flowchart is correct here because the content is
a directed control flow with a decision node. Reproduced in the compiled LaTeX
narrative as a matching colored TikZ figure (palette: black, grayscales, #EBCB8B,
#D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'},'flowchart':{'curve':'basis','nodeSpacing':40,'rankSpacing':55,'htmlLabels':true}}}%%
flowchart TB
  SPEC["Clinical specification<br/>human investigators"]:::n1
  GEN["Claude Code<br/>generates candidate code"]:::n2
  REV["Codex<br/>independent peer review"]:::n2
  VVUQ{"VVUQ verification<br/>ten gates"}:::act
  ACC["ACCEPT<br/>execute under audit"]:::hope
  ESC["ESCALATE<br/>return to a qualified human"]:::n3
  BLK["BLOCK<br/>stop before execution"]:::risk
  SPEC --> GEN
  GEN --> REV
  REV --> VVUQ
  VVUQ -->|all gates pass| ACC
  VVUQ -->|uncertain| ESC
  VVUQ -->|catastrophe predicate| BLK
  ESC -.->|human revises| GEN
  classDef act fill:#8B2E3F,stroke:#000000,stroke-width:1.4px,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,stroke-width:1.2px,color:#1A1505
  classDef risk fill:#D08770,stroke:#000000,stroke-width:1.2px,color:#1A0A04
  classDef n1 fill:#F2F2F2,stroke:#333333,stroke-width:1.1px,color:#111111
  classDef n2 fill:#D9D9D9,stroke:#222222,stroke-width:1.1px,color:#111111
  classDef n3 fill:#BFBFBF,stroke:#000000,stroke-width:1.2px,color:#111111
```
