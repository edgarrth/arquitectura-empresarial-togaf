# Stakeholder Map

# Stakeholders clave

| Stakeholder | Interés | Preocupación | Entregable relevante |
|---|---|---|---|
| CEO / Gerencia General | Crecimiento, eficiencia, riesgo | Velocidad sin comprometer control | Architecture Vision, Roadmap |
| CFO | Costos, rentabilidad, CAPEX/OPEX | Retorno de inversión | Business Case, Roadmap |
| COO | Operación estable | Impacto en procesos críticos | Migration Plan, Implementation Governance |
| CISO | Seguridad, cumplimiento | Riesgos de identidad, datos y terceros | Security Architecture |
| CTO / CIO | Plataforma tecnológica | Complejidad, deuda técnica, escalabilidad | Technology Architecture |
| Head de Producto | Time-to-market | Dependencias y cuellos de botella | Capability Map, API Catalog |
| Riesgos | Score, originación, fraude | Trazabilidad y explicabilidad | Data Architecture, Decision Logs |
| Legal / Compliance | Regulación y auditoría | Evidencias y privacidad | Governance Model |
| Squads | Delivery | Estándares demasiado pesados | Golden Paths, Templates |
| Operaciones TI | Estabilidad | Observabilidad y soporte | Runbooks, SLOs |

# Matriz poder/interés

```mermaid
quadrantChart
    title Stakeholder Power / Interest
    x-axis Low Interest --> High Interest
    y-axis Low Power --> High Power
    quadrant-1 Manage closely
    quadrant-2 Keep satisfied
    quadrant-3 Monitor
    quadrant-4 Keep informed
    CEO: [0.85, 0.95]
    CFO: [0.65, 0.85]
    CISO: [0.9, 0.8]
    Product: [0.8, 0.7]
    Squads: [0.75, 0.45]
    Operations: [0.7, 0.6]
    Compliance: [0.8, 0.75]
```
