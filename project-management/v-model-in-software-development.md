# V-model in software development

- [What Is the V-Model? (Definition, Examples) | Built In](https://builtin.com/software-engineering-perspectives/v-model)
- [SDLC - V-Model](https://www.tutorialspoint.com/sdlc/sdlc_v_model.htm)
- [SDLC V-Model - Software Engineering - GeeksforGeeks](https://www.geeksforgeeks.org/software-engineering-sdlc-v-model/)

## The V-model

Each design phase on the left arm of the "V" produces the test design that is verified by the matching testing phase on the right arm.

```mermaid
flowchart TB
    RA["Requirement Analysis"] --> SD["System Design"]
    SD --> AD["Architecture Design"]
    AD --> MD["Module Design"]
    MD --> C["Coding"]
    C --> UT["Unit Testing"]
    UT --> IT["Integration Testing"]
    IT --> ST["System Testing"]
    ST --> AT["Acceptance Testing"]

    RA -. "Acceptance Test Design" .-> AT
    SD -. "System Test Design" .-> ST
    AD -. "Integration Test Design" .-> IT
    MD -. "Unit Test Design" .-> UT
```

The same model, with the test-design artifacts drawn explicitly in the middle of the "V":

```mermaid
flowchart TB
    subgraph verification [" "]
        direction TB
        RA["Requirement Analysis"] --> SD["System Design"] --> AD["Architecture Design"] --> MD["Module Design"]
    end
    subgraph testdesign [" "]
        direction TB
        ATD["Acceptance Test Design"]
        STD["System Test Design"]
        ITD["Integration Test Design"]
        UTD["Unit Test Design"]
    end
    subgraph validation [" "]
        direction BT
        UT["Unit Testing"] --> IT["Integration Testing"] --> ST["System Testing"] --> AT["Acceptance Testing"]
    end
    MD --> C["Coding"] --> UT
    RA -.-> ATD -.-> AT
    SD -.-> STD -.-> ST
    AD -.-> ITD -.-> IT
    MD -.-> UTD -.-> UT
```

## Role and responsibility

```mermaid
flowchart TB
    subgraph TL ["Technical Lead (reviews)"]
        SD["System Design"] --> AD["Architecture Design"] --> MD["Module Design"]
    end
    subgraph IC ["Individual Contributors"]
        MD --> C["Coding"] --> UT["Unit Testing"]
        UT --> IT["Integration Testing"]
    end
    subgraph QA ["QA Team"]
        IT --> ST["System Testing"] --> AT["Acceptance Testing"]
    end
    RA["Requirement Analysis"] --> SD
    RA -. "Acceptance Test Design" .-> AT
    SD -. "System Test Design" .-> ST
    AD -. "Integration Test Design" .-> IT
    MD -. "Unit Test Design" .-> UT

    style TL stroke:#2c5cff,stroke-width:2px
    style IC stroke:#3cb043,stroke-width:2px
    style QA stroke:#e0301e,stroke-width:2px
```

| V-model phases | Owner (Responsible) | Reviewer (Accountable) |
| --- | --- | --- |
| Requirements analysis | Individual contributors | Technical lead |
| System design | Individual contributors | Technical lead |
| Architecture design | Individual contributors | Technical lead |
| Module design | Individual contributors | Technical lead |
| Unit testing | Individual contributors | Technical lead |
| Integration testing | QA team / Individual contributors | Technical lead |
| System testing | QA team | Product/Project manager |
| Acceptance testing | QA team | Product/Project manager |
