# ADR-002: Plataforma de eventos empresarial

# Estado

Aceptado como decisión de referencia.

# Contexto

La organización necesita desacoplar dominios, reducir dependencia de batch, habilitar integración near real-time y mejorar trazabilidad de eventos de negocio.

# Alternativas

| Alternativa | Descripción |
|---|---|
| Event streaming Kafka-compatible | Alto throughput, ecosistema maduro |
| Broker tradicional de mensajería | Bueno para colas y comandos |
| Integración batch/files | Compatible con legado, baja inmediatez |

# Decisión

Adoptar una plataforma de event streaming para eventos de negocio, manteniendo mensajería tradicional y batch solo donde el caso lo requiera.

# Consecuencias

- Se requiere catálogo de eventos.
- Se requiere schema registry.
- Los consumidores deben ser idempotentes.
- Se implementa DLQ y replay para flujos críticos.
- Se define política de retención por dominio.
