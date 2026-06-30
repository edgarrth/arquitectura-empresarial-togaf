# Technology Architecture

# Plataforma objetivo

| Capa | Decisión base                                |
|---|----------------------------------------------|
| Runtime aplicaciones | Kubernetes administrado o plataforma equivalente |
| APIs | API Manager + Developer Portal               |
| Eventos | Kafka-compatible event streaming             |
| Datos transaccionales | Base relacional administrada para consistencia |
| Datos documentales | Base documental para agregados flexibles     |
| Cache | Redis-compatible                             |
| Observabilidad | OpenTelemetry, Prometheus, Loki, Tempo/Grafana |
| Secrets | Vault/KMS/Secret Manager                     |
| CI/CD | GitHub Actions/GitLab CI + GitOps            |
| Seguridad | OIDC, OAuth2, mTLS interno donde aplique     |
| IaC | Terraform y Ansible                          |
| Policy as Code | Kyverno                                      |

# Diagrama tecnológico

![Technology Platform View](../assets/diagrams/archimate/05-technology-platform-view.svg)

# NFR base

| NFR | Estándar |
|---|---|
| Disponibilidad servicios críticos | 99.9% mínimo, superior según criticidad |
| Latencia APIs críticas | P95 definido por dominio |
| Observabilidad | Logs, métricas, trazas y health checks |
| Seguridad | Cifrado en tránsito y reposo |
| Resiliencia | Timeouts, retries, circuit breakers |
| Continuidad | Backups probados y DR plan |
| Escalabilidad | Horizontal cuando sea posible |
| Auditabilidad | Correlation ID y evidencias de cambios |
