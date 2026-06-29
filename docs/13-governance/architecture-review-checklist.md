# Architecture Review Checklist

# Contexto

- ¿La iniciativa está alineada a una capacidad priorizada?
- ¿Existe sponsor de negocio?
- ¿Se identificaron stakeholders?
- ¿Se definieron NFRs?

# Aplicaciones

- ¿La solución reutiliza capacidades existentes?
- ¿Evita duplicidad funcional?
- ¿Define contratos API/eventos?
- ¿Tiene estrategia de versionado?

# Datos

- ¿Produce o consume datos sensibles?
- ¿Tiene data owner?
- ¿Define retención y clasificación?
- ¿Tiene linaje básico?

# Seguridad

- ¿Se hizo threat modeling?
- ¿Usa OIDC/OAuth2/MFA según criticidad?
- ¿Gestiona secretos correctamente?
- ¿Tiene auditoría de operaciones sensibles?

# Tecnología

- ¿Usa runtime aprobado?
- ¿Tiene pipeline CI/CD?
- ¿Cumple observabilidad mínima?
- ¿Tiene rollback?

# Operación

- ¿Tiene SLO?
- ¿Tiene runbook?
- ¿Tiene alertas?
- ¿Tiene plan de soporte?

# Decisión

| Resultado | Uso |
|---|---|
| Aprobado | Puede continuar |
| Aprobado con condiciones | Debe resolver pendientes antes de producción |
| Requiere rediseño | No cumple criterios mínimos |
| Excepción temporal | Se aprueba con fecha de expiración |
