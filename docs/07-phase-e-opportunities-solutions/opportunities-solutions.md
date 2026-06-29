# Opportunities & Solutions

# Iniciativas candidatas

| ID | Iniciativa | Beneficio | Complejidad | Prioridad |
|---|---|---|---|---|
| OS-01 | CIAM corporativo | Seguridad y experiencia omnicanal | Alta | Alta |
| OS-02 | API Management | Gobierno de integraciones | Media | Alta |
| OS-03 | Event Platform | Desacoplamiento y near real-time | Alta | Alta |
| OS-04 | Observability Foundation | Reducción MTTR | Media | Alta |
| OS-05 | Data Governance Foundation | Calidad y cumplimiento | Alta | Alta |
| OS-06 | Developer Portal | Estandarización y velocidad | Media | Media |
| OS-07 | Conciliación automatizada | Eficiencia operativa | Alta | Alta |
| OS-08 | Merchant Platform Modernization | Crecimiento comercios | Alta | Media |
| OS-09 | Risk Decisioning Modernization | Mejor riesgo y fraude | Alta | Alta |

# Solution Building Blocks

| Building Block | Descripción | Reutilización |
|---|---|---|
| Identity Provider | Autenticación, MFA, OIDC | Todos los canales |
| API Gateway | Seguridad, throttling, publicación | APIs internas/externas |
| Event Broker | Eventos de negocio | Integración y data |
| Observability Stack | Telemetría, alertas, dashboards | Todos los servicios |
| Data Platform | Lakehouse, warehouse, lineage | Analytics, reporting, IA |
| Golden Path Java | Template microservicio | Squads backend |
| Golden Path Frontend | Template web/mobile | Squads canales |
| Policy Engine | Reglas de despliegue | Plataforma |

# Transition architectures

## TA-1 Foundation

- CIAM base.
- API Gateway.
- Observabilidad estándar.
- Catálogo de aplicaciones.
- Primeros dominios de datos.

## TA-2 Domain modernization

- Servicios dominio para cliente, pagos y comercios.
- Event streaming.
- Outbox/CDC para core.
- Developer portal.

## TA-3 Digital operating model

- Autoservicio de plataforma.
- Data products gobernados.
- Conciliación automatizada.
- SLOs por producto.
