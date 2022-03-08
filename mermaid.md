Mermaid embedded in markdown:


```mermaid
flowchart LR
A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two|E[Result 2]
```

mermaid with theme and stright arrow:
```mermaid
%%{ init : { "theme" : "forest", "flowchart" : { "curve" : "stepBefore" }}}%%
flowchart LR
A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two|E[Result 2]
```


Graph with font awesome (not rendered on Github):
```mermaid
graph TD
    A[Christmas] -->|Get money| B(Go shopping)
    B --> C{Let me think}
    C -->|One| D[Laptop]
    C -->|Two| E[iPhone]
    C -->|Three| F[fa:fa-car Car]
```

- C4 model, haven't native supported by mermaid yet  
Alternative:
    * https://github.com/mermaid-js/mermaid/issues/1276#issuecomment-802139353
    * https://structurizr.com/dsl?example=getting-started

Example:
```mermaid
graph TB
  linkStyle default fill:#ffffff

  1["<div style='font-weight: bold'>User</div><div style='font-size: 70%; margin-top: 0px'>[Person]</div><div style='font-size: 80%; margin-top:10px'>A user of my software system.</div>"]
  style 1 fill:#08427b,stroke:#052e56,color:#ffffff
  2["<div style='font-weight: bold'>Software System</div><div style='font-size: 70%; margin-top: 0px'>[Software System]</div><div style='font-size: 80%; margin-top:10px'>My software system.</div>"]
  style 2 fill:#1168bd,stroke:#0b4884,color:#ffffff

  1-. "<div>Uses</div><div style='font-size: 70%'></div>" .->2
```
