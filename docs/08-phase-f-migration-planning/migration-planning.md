# Migration Planning

# Roadmap por oleadas

```mermaid
gantt
    title Enterprise Architecture Migration Roadmap
    dateFormat  YYYY-MM-DD
    section Foundation
    Architecture governance        :a1, 2026-07-01, 45d
    API management foundation      :a2, 2026-07-15, 60d
    Observability foundation       :a3, 2026-07-15, 60d
    section Security
    CIAM implementation            :b1, 2026-08-01, 90d
    Secrets and key management     :b2, 2026-08-15, 60d
    section Modernization
    Event platform                 :c1, 2026-09-01, 90d
    Customer domain services       :c2, 2026-10-01, 120d
    Payment domain services        :c3, 2026-10-15, 150d
    section Data
    Data governance foundation     :d1, 2026-09-15, 120d
    Operational data store         :d2, 2026-11-01, 120d
```

# Priorización

| Criterio | Peso |
|---|---:|
| Reducción de riesgo operativo | 25 |
| Impacto en negocio | 25 |
| Habilitación de capacidades futuras | 20 |
| Cumplimiento / seguridad | 15 |
| Complejidad y dependencias | 15 |

# Dependencias críticas

- CIAM debe preceder a rediseño de canales.
- API Management debe preceder a exposición externa masiva.
- Observabilidad debe preceder a migraciones críticas.
- Event Platform debe preceder a desacoplamiento de core.
- Data Governance debe preceder a modelos analíticos críticos.

# Estrategia de migración

- Evitar big bang.
- Usar strangler pattern para dominios críticos.
- Priorizar nuevas capacidades en arquitectura target.
- Mantener coexistencia controlada con legado.
- Medir reducción de deuda técnica por oleada.
