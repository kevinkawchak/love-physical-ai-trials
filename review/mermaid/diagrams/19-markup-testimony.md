### 19. Markup and Testimony

The committee markup is where the bill is debated, amended, and rewritten on the
strength of testimony from AI experts, physicians, and patients, building the
official public record. A sequence diagram is correct because the content is a
structured exchange between the committee and its witnesses with an amendment
loop. Reproduced in the compiled LaTeX narrative as a matching colored TikZ figure
(palette: black, grayscales, #EBCB8B, #D08770, #8B2E3F).

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Helvetica, Arial, sans-serif','actorBkg':'#D9D9D9','actorBorder':'#000000','actorTextColor':'#111111','actorLineColor':'#888888','signalColor':'#333333','signalTextColor':'#111111','noteBkgColor':'#EBCB8B','noteBorderColor':'#000000','noteTextColor':'#1A1505','labelBoxBkgColor':'#8B2E3F','labelBoxBorderColor':'#000000','labelTextColor':'#ffffff','sequenceNumberColor':'#ffffff','loopTextColor':'#111111'}}}%%
sequenceDiagram
  autonumber
  participant W as Witnesses (experts, doctors, patients)
  participant K as Committee
  participant B as Bill text
  W->>K: Testimony and evidence on record
  loop Markup
    K->>B: Propose amendment
    B-->>K: Revised clause
    W-->>K: Clarifying testimony
  end
  K->>B: Order reported
  Note over B: Strengthened, on the public record
```
