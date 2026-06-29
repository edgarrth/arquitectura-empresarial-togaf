# Observability Standards

# Señales obligatorias

| Señal | Requerimiento |
|---|---|
| Logs | JSON estructurado, correlationId, level, service, environment |
| Métricas | RED/USE según tipo de servicio |
| Trazas | OpenTelemetry en APIs y workers críticos |
| Health checks | Liveness y readiness |
| Alertas | Basadas en síntomas, no solo recursos |
| Dashboards | Técnico y de negocio para servicios críticos |

# Métricas RED

| Métrica | Descripción |
|---|---|
| Rate | Requests por segundo |
| Errors | Tasa de errores |
| Duration | Latencia p50/p95/p99 |

# Campos mínimos de log

```json
{
  "timestamp": "2026-06-28T10:30:00Z",
  "level": "INFO",
  "service": "payment-authorization-service",
  "environment": "prod",
  "correlationId": "uuid",
  "message": "Payment authorized",
  "customerId": "masked",
  "transactionId": "uuid"
}
```

# Reglas

- No loguear PAN, CVV, secretos ni tokens.
- Enmascarar PII.
- Propagar correlation ID.
- Alertas críticas deben tener runbook.
