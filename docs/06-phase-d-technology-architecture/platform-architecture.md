# Platform Architecture

# Plataforma como producto

La plataforma interna debe ofrecer capacidades reutilizables para que los squads entreguen software seguro, observable y gobernado sin reinventar infraestructura.

# Capacidades de plataforma

| Capacidad | Descripción |
|---|---|
| Developer Portal | Catálogo de servicios, APIs, owners, documentación y scorecards |
| Golden Paths | Plantillas listas para microservicios, workers, APIs y jobs |
| CI/CD | Build, test, security scanning, artifact publishing |
| GitOps | Despliegue declarativo y auditable |
| Observability | Métricas, logs, trazas, alertas y SLOs |
| Secrets | Gestión centralizada de secretos y rotación |
| Policy as Code | Validación de estándares antes del despliegue |
| Runtime | Kubernetes, service mesh y autoscaling |
| FinOps | Cost visibility y tagging obligatorio |

# Vista tecnológica de plataforma

Esta vista ArchiMate muestra la relación entre developer portal, repositorios, CI/CD, GitOps, Kubernetes, observabilidad, secretos, políticas y servicios administrados.

![Technology Platform View](../assets/diagrams/archimate/05-technology-platform-view.svg)

# Golden path de microservicio

1. El desarrollador selecciona un template en el Developer Portal.
2. El portal crea el repositorio con estructura estándar.
3. El pipeline ejecuta build, tests y security scanning.
4. El artefacto se publica en el registry.
5. GitOps sincroniza manifiestos con Kubernetes.
6. El servicio queda desplegado, observable y registrado en el catálogo.

# Scorecard mínimo

- Owner definido.
- README actualizado.
- API/eventos registrados.
- Pipeline activo.
- Tests mínimos.
- Vulnerabilidades críticas bloqueantes.
- Logs estructurados.
- Métricas técnicas y de negocio.
- Dashboards y alertas.
- Runbook operativo.
