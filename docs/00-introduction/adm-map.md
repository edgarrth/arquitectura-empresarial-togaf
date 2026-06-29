# Mapa ADM adaptado

# Adaptación usada

TOGAF ADM es iterativo. Para una empresa financiera, la implementación práctica debe evitar una ejecución waterfall pesada. Las fases se usan como marco de pensamiento y como checklist de entregables.

```mermaid
flowchart LR
    P[Preliminary] --> A[Phase A: Architecture Vision]
    A --> B[Phase B: Business Architecture]
    B --> C1[Phase C: Data Architecture]
    B --> C2[Phase C: Application Architecture]
    C1 --> D[Phase D: Technology Architecture]
    C2 --> D
    D --> E[Phase E: Opportunities & Solutions]
    E --> F[Phase F: Migration Planning]
    F --> G[Phase G: Implementation Governance]
    G --> H[Phase H: Change Management]
    H --> A
    R[Requirements Management] -.-> A
    R -.-> B
    R -.-> C1
    R -.-> C2
    R -.-> D
    R -.-> E
    R -.-> F
    R -.-> G
    R -.-> H
```

# Entregables mínimos por ciclo

| Fase | Entregable mínimo |
|---|---|
| Preliminary | Principios, modelo de gobierno, metamodelo mínimo |
| A | Architecture Vision, stakeholders, business case |
| B | Capability map, value streams, gaps |
| C Data | Data domains, ownership, governance |
| C App | Application landscape, integration map, APIs |
| D | Technology standards, platform blueprint |
| E | Solution building blocks, transition architectures |
| F | Roadmap, dependency map |
| G | Architecture contract, compliance checklist |
| H | Change control, exceptions, backlog arquitectónico |
