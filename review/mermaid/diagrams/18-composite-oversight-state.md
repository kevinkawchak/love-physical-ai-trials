### 18. Composite Oversight State Machine

The same workflow nested into three super-states, Authoring, Verification, and
Oversight, to show that the model scales to institutional complexity without
clutter. A composite state diagram is correct because the content is nested states
with internal transitions and a clean exit. Reproduced in the compiled LaTeX
narrative as a matching colored TikZ figure (palette: black, grayscales, #EBCB8B,
#D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','lineColor':'#333333','primaryTextColor':'#111111'}}}%%
stateDiagram-v2
  direction LR
  [*] --> Authoring
  state Authoring {
    [*] --> Specify
    Specify --> Generate
    Generate --> [*]
  }
  Authoring --> Verification
  state Verification {
    direction TB
    [*] --> Gates
    Gates --> Review: pass
    Review --> [*]: peer reviewed
  }
  Verification --> Oversight
  state Oversight {
    [*] --> Report
    Report --> Certify
    Certify --> [*]
  }
  Oversight --> [*]: public record
  classDef act fill:#8B2E3F,stroke:#000000,color:#ffffff
  class Verification act
```
