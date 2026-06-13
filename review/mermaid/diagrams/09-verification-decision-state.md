### 09. The Verification Decision State Machine

At runtime the system is always in one of a few states: it detects an event,
verifies against the gates, and resolves to ACCEPT, ESCALATE to a qualified human,
or BLOCK before execution. A state diagram is correct because the content is a set
of discrete states with guarded transitions and a choice. Reproduced in the
compiled LaTeX narrative as a matching colored TikZ figure (palette: black,
grayscales, #EBCB8B, #D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'}}}%%
stateDiagram-v2
  direction LR
  [*] --> Detect
  Detect --> Verify: event flagged
  Verify --> Decision
  state Decision <<choice>>
  Decision --> Accept: all gates pass
  Decision --> Escalate: uncertain
  Decision --> Block: catastrophe predicate
  Escalate --> Verify: human revises
  Accept --> [*]
  Block --> [*]
  classDef act fill:#8B2E3F,stroke:#000000,color:#ffffff
  classDef hope fill:#EBCB8B,stroke:#000000,color:#1A1505
  classDef risk fill:#D08770,stroke:#000000,color:#1A0A04
  class Verify act
  class Accept hope
  class Block risk
```
