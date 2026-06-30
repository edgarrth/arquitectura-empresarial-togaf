# Vistas ArchiMate

# Propósito

Estas vistas complementan la documentación TOGAF con una notación más alineada a Arquitectura Empresarial.

ArchiMate se usa aquí para representar:

- capacidades y servicios de negocio;
- value streams;
- cooperación entre aplicaciones;
- objetos de datos;
- plataforma tecnológica;
- seguridad e identidad;
- plateaus, gaps, work packages y roadmap de transición.

# Qué diagramas conviene mantener fuera de ArchiMate

No todo debe convertirse a ArchiMate. Para algunos casos es mejor conservar otros tipos de diagramas:

| Tipo de diagrama | Mejor notación | Motivo |
|---|---|---|
| Secuencia de autorización de pago | UML Sequence / PlantUML | Muestra orden temporal de llamadas |
| Mapa ADM | Imagen / SVG explicativo | Representa método, no arquitectura de empresa |
| Matriz stakeholder poder/interés | Mermaid Quadrant | Muestra clasificación visual |
| Flujo técnico request/response | UML Sequence | Más claro para comportamiento runtime |
| Operating model / organigrama | Mermaid / draw.io | No requiere semántica ArchiMate |

# Vistas incluidas

| Vista | Archivo fuente | Uso principal |
|---|---|---|
| Business Capability View | `01-business-capability-view.puml` | Phase B - Capability Map |
| Payment Value Stream View | `02-payment-value-stream-view.puml` | Phase B - Business Architecture |
| Application Cooperation View | `03-application-cooperation-view.puml` | Phase C Application |
| Data Architecture View | `04-data-architecture-view.puml` | Phase C Data |
| Technology Platform View | `05-technology-platform-view.puml` | Phase D - Vista general de plataforma |
| Security & IAM View | `06-security-iam-view.puml` | Security Architecture |
| Migration Roadmap View | `07-migration-roadmap-view.puml` | Phase F - Migration Planning |
| Architecture Vision View | `08-architecture-vision-view.puml` | Phase A - Architecture Vision |
| Integration Architecture View | `09-integration-architecture-view.puml` | Phase C Application - Integration |

# Regla de uso para Platform Architecture

En `platform-architecture.md` se usan dos notaciones:

| Diagrama | Notación | Razón |
|---|---|---|
| Vista general de plataforma | ArchiMate | Muestra componentes, servicios y nodos tecnológicos |
| Golden path de microservicio | Mermaid sequence | Muestra una secuencia temporal de pasos |

El golden path no debe migrarse a ArchiMate porque no describe una estructura empresarial estable, sino un flujo operativo.

# Diagramas renderizados

!!! note
    El workflow de GitHub Actions renderiza los `.puml` a SVG antes de publicar GitHub Pages. Estas imágenes SVG se generan durante el pipeline; por eso no necesariamente existirán en el repositorio antes de ejecutar el Action.

## Architecture Vision View

![Architecture Vision View](../../assets/diagrams/archimate/08-architecture-vision-view.svg)

## Business Capability View

![Business Capability View](../../assets/diagrams/archimate/01-business-capability-view.svg)

## Payment Value Stream View

![Payment Value Stream View](../../assets/diagrams/archimate/02-payment-value-stream-view.svg)

## Application Cooperation View

![Application Cooperation View](../../assets/diagrams/archimate/03-application-cooperation-view.svg)

## Integration Architecture View

![Integration Architecture View](../../assets/diagrams/archimate/09-integration-architecture-view.svg)

## Data Architecture View

![Data Architecture View](../../assets/diagrams/archimate/04-data-architecture-view.svg)

## Technology Platform View

![Technology Platform View](../../assets/diagrams/archimate/05-technology-platform-view.svg)

## Security & IAM View

![Security & IAM View](../../assets/diagrams/archimate/06-security-iam-view.svg)

## Migration Roadmap View

![Migration Roadmap View](../../assets/diagrams/archimate/07-migration-roadmap-view.svg)
