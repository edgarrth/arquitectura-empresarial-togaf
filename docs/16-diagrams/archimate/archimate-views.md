# Vistas ArchiMate

# Propósito

Estas vistas complementan los diagramas Mermaid y PlantUML existentes con una notación más alineada a TOGAF y Arquitectura Empresarial.

ArchiMate encaja mejor para representar:

- capacidades de negocio;
- value streams;
- servicios de negocio;
- aplicaciones y servicios de aplicación;
- objetos de datos;
- infraestructura tecnológica;
- seguridad e identidad;
- paquetes de trabajo y roadmap de transición.

# Qué diagramas conviene mantener fuera de ArchiMate

No todo debe convertirse a ArchiMate. Para algunos casos es mejor conservar otros tipos de diagramas:

| Tipo de diagrama | Mejor notación | Motivo |
|---|---|---|
| Secuencia de autorización de pago | UML Sequence / PlantUML | Muestra orden temporal de llamadas |
| Gantt de roadmap | Mermaid Gantt | Muestra fechas y duración |
| Matriz stakeholder poder/interés | Mermaid Quadrant | Muestra clasificación visual |
| Flujo técnico request/response | UML Sequence | Más claro para comportamiento runtime |

# Vistas incluidas

| Vista | Archivo fuente | Uso |
|---|---|---|
| Business Capability View | `01-business-capability-view.puml` | Phase B |
| Payment Value Stream View | `02-payment-value-stream-view.puml` | Phase B |
| Application Cooperation View | `03-application-cooperation-view.puml` | Phase C Application |
| Data Architecture View | `04-data-architecture-view.puml` | Phase C Data |
| Technology Platform View | `05-technology-platform-view.puml` | Phase D |
| Security & IAM View | `06-security-iam-view.puml` | Security Architecture |
| Migration Roadmap View | `07-migration-roadmap-view.puml` | Phase E/F |

# Diagramas renderizados

!!! note
    El workflow de GitHub Actions renderiza los `.puml` a SVG antes de publicar GitHub Pages.

## Business Capability View

![Business Capability View](../../assets/diagrams/archimate/01-business-capability-view.svg)

## Payment Value Stream View

![Payment Value Stream View](../../assets/diagrams/archimate/02-payment-value-stream-view.svg)

## Application Cooperation View

![Application Cooperation View](../../assets/diagrams/archimate/03-application-cooperation-view.svg)

## Data Architecture View

![Data Architecture View](../../assets/diagrams/archimate/04-data-architecture-view.svg)

## Technology Platform View

![Technology Platform View](../../assets/diagrams/archimate/05-technology-platform-view.svg)

## Security & IAM View

![Security & IAM View](../../assets/diagrams/archimate/06-security-iam-view.svg)

## Migration Roadmap View

![Migration Roadmap View](../../assets/diagrams/archimate/07-migration-roadmap-view.svg)
