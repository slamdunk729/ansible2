```mermaid
%%{init:{'theme':'base'}}%%
  
graph LR
  SPA["Single Page Application"]
  BFF["Backends For Frontends"]
  BE["Backends"]
  subgraph browser
    SPA
  end
  subgraph cloud["Cloud environment"]
    BFF --> BE
  end
  SPA -- port 443 --> BFF
  

  classDef class1 fill:#7BCCAC,fill-opacity:0.5
  classDef class2 fill:#ffa23e

  qemu(QEMU):::class1 --> zircon[ZIRCON]:::class2
  zircon --> fuchsia[FUCHSIA]:::class1
```

```mermaid
%%{init:{'theme':'base'}}%%
 gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
```

```mermaid
%%{init:{'theme':'base'}}%%
pie title Pets adopted by volunteers
    "Dogs" : 386
    "Cats" : 85
    "Rats" : 15
```

```mermaid
%%{init:{'theme':'base'}}%%
  journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 3: Me
```      
