# TOGAF Financial Enterprise Architecture Blueprint

Repositorio base para implementar una práctica de Arquitectura Empresarial en una organización financiera de tarjetas, pagos, crédito, comercios afiliados y canales digitales.

Este repo adapta el ADM de TOGAF a un contexto financiero regulado. No contiene todos los entregables disponibles de TOGAF, prioriza los documentos que una empresa podria necesitar para gobernar.

## Objetivos

- Crear una base reutilizable para futuras iniciativas de arquitectura empresarial.
- Alinear negocio, datos, aplicaciones, tecnología y seguridad.
- Formalizar decisiones mediante ADRs.
- Definir estándares reutilizables para APIs, eventos, integración, datos, observabilidad y seguridad.
- Facilitar gobierno arquitectónico sin convertirlo en burocracia.
- Publicar documentación con GitHub Pages.

## Contexto empresarial de referencia

Organización financiera con:

- emisión de tarjetas;
- adquirencia y comercios afiliados;
- pagos digitales;
- canales web y mobile;
- originación de crédito;
- motor de riesgo;
- antifraude;
- conciliación y liquidación;
- programas de fidelización;
- atención al cliente;
- integración con procesadores, marcas de tarjeta, bureaus, bancos, fintechs y reguladores.

## Estructura ADM


| Fase                | Propósito                          | Carpeta                                          |
| ------------------- | ----------------------------------- | ------------------------------------------------ |
| Preliminary         | Preparar capacidad de arquitectura  | `docs/01-preliminary`                            |
| Phase A             | Definir visión y alcance           | `docs/02-phase-a-architecture-vision`            |
| Phase B             | Arquitectura de negocio             | `docs/03-phase-b-business-architecture`          |
| Phase C Data        | Arquitectura de datos               | `docs/04-phase-c-data-architecture`              |
| Phase C Application | Arquitectura de aplicaciones        | `docs/05-phase-c-application-architecture`       |
| Phase D             | Arquitectura tecnológica           | `docs/06-phase-d-technology-architecture`        |
| Phase E             | Oportunidades y soluciones          | `docs/07-phase-e-opportunities-solutions`        |
| Phase F             | Plan de migración                  | `docs/08-phase-f-migration-planning`             |
| Phase G             | Gobierno de implementación         | `docs/09-phase-g-implementation-governance`      |
| Phase H             | Gestión del cambio arquitectónico | `docs/10-phase-h-architecture-change-management` |
| Requirements        | Gestión continua de requerimientos | `docs/11-requirements-management`                |

# Principios de diseño

- Cloud-native cuando aporte velocidad, resiliencia y eficiencia.
- Seguridad por diseño.
- APIs y eventos como contratos empresariales.
- Datos gobernados como activo corporativo.
- Plataforma como producto interno.
- Automatización sobre procesos manuales.
- Observabilidad obligatoria para servicios críticos.
- Desacoplamiento progresivo del core legado.

## Quick start

```bash
pip install mkdocs-material
mkdocs serve
```

## Diagramas ArchiMate

El repositorio incluye vistas ArchiMate en `docs/16-diagrams/archimate`. El workflow de GitHub Actions las renderiza a SVG y las publica en GitHub Pages.
