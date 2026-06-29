# Event Standards

# Convención de nombres

```text
<domain>.<subdomain>.<event-name>.v<version>
```

# Ejemplos

```text
payments.authorization.approved.v1
payments.authorization.declined.v1
customers.identity.verified.v1
merchants.settlement.completed.v1
risk.credit-decision.approved.v1
fraud.alert.created.v1
```

# Envelope estándar

```json
{
  "eventId": "uuid",
  "eventType": "payments.authorization.approved.v1",
  "occurredAt": "2026-06-28T10:30:00Z",
  "producer": "payment-authorization-service",
  "correlationId": "uuid",
  "causationId": "uuid",
  "payload": {}
}
```

# Reglas

- Eventos representan hechos, no comandos.
- Todo evento debe tener schema versionado.
- Los cambios deben ser backward compatible siempre que sea posible.
- Los consumidores deben ser idempotentes.
- Los eventos críticos deben tener DLQ y estrategia de replay.
- No publicar datos sensibles salvo justificación aprobada.
