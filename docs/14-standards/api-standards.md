# API Standards

# Reglas REST

- Usar sustantivos en plural.
- Versionar en path: `/v1`.
- Evitar verbos en recursos.
- Usar kebab-case para paths.
- Usar camelCase para variables y atributos JSON.
- Usar códigos HTTP estándar.
- Usar pagination en colecciones.
- Usar idempotency key en comandos financieros.
- Documentar con OpenAPI.

# Ejemplos

```http
GET /v1/customers/{customerId}/cards
POST /v1/payments
GET /v1/merchants/{merchantId}/settlements
POST /v1/payment-disputes
```

# Respuesta de error estándar

```json
{
  "code": "PAYMENT_DECLINED",
  "message": "Payment could not be approved",
  "correlationId": "7f8e2f7a-0b9a-4e8e-9e29-01a2f9f9c101",
  "details": [
    {
      "field": "amount",
      "reason": "Amount exceeds configured limit"
    }
  ]
}
```

# Headers obligatorios

| Header | Uso |
|---|---|
| Authorization | Token Bearer |
| X-Correlation-Id | Trazabilidad |
| Idempotency-Key | Operaciones financieras no idempotentes por naturaleza |
| X-Channel | Canal origen |
