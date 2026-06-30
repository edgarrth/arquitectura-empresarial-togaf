# Implementation Governance

# Objetivo

Asegurar que las iniciativas implementen la arquitectura aprobada, gestionen excepciones y mantengan trazabilidad de decisiones.

# Puntos de control

| Momento | Control |
|---|---|
| Inicio iniciativa | Validar alineamiento con capacidades y roadmap |
| Diseño solución | Revisar NFRs, seguridad, integración y datos |
| Antes de build | Aprobar ADRs relevantes |
| Antes de producción | Validar observabilidad, seguridad y operación |
| Post go-live | Revisar métricas, incidentes y deuda pendiente |

# Architecture Contract

Cada iniciativa crítica debe documentar:

- alcance
- capacidades impactadas
- arquitectura target
- decisiones ADR
- riesgos aceptados
- excepciones
- NFRs
- owners
- plan de operación
- criterios de salida

# Compliance checklist

| Control | Obligatorio |
|---|---|
| API/evento registrado | Sí |
| Data owner definido | Sí, si produce datos |
| Threat model | Sí, si maneja datos sensibles |
| Observabilidad | Sí |
| Runbook | Sí |
| SLO definido | Sí para servicios críticos |
| Evidencia de pruebas | Sí |
| Plan rollback | Sí |
