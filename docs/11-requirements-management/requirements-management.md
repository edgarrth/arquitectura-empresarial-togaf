# Requirements Management

# Enfoque

Los requerimientos arquitectónicos se gestionan de forma continua durante todo el ADM.

# Categorías

| Categoría | Ejemplos |
|---|---|
| Negocio | Aumentar conversión digital, reducir tiempos de afiliación |
| Seguridad | MFA, cifrado, segregación, auditoría |
| Datos | Linaje, calidad, retención, clasificación |
| Integración | APIs, eventos, batch, terceros |
| Operación | SLO, monitoreo, soporte, DR |
| Cumplimiento | Evidencias, trazabilidad, reportes |
| Plataforma | CI/CD, autoservicio, políticas |

# Formato de requerimiento

| Campo | Descripción |
|---|---|
| ID | Código único |
| Descripción | Necesidad expresada de forma verificable |
| Fuente | Stakeholder, regulación, riesgo, iniciativa |
| Prioridad | Alta, media, baja |
| Criterio de aceptación | Cómo se verifica |
| Estado | Propuesto, aprobado, implementado, descartado |
| Trazabilidad | Fase ADM, solución, ADR o control asociado |

# Ejemplos reales de requerimientos base

| ID | Requerimiento | Criterio |
|---|---|---|
| REQ-001 | Todo servicio expuesto a clientes debe usar OIDC/OAuth2 | Validación en API Gateway y token introspection/JWKS |
| REQ-002 | Toda transacción financiera debe tener correlation ID | Correlation ID visible en logs, trazas y eventos |
| REQ-003 | Todo dato sensible debe clasificarse | Data catalog con clasificación aprobada |
| REQ-004 | Todo evento de negocio debe tener contrato versionado | Schema registrado y compatible |
| REQ-005 | Toda integración crítica debe definir retry, timeout y DLQ | Evidencia en diseño y pruebas |
