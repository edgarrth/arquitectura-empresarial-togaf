# ADR-001: Selección de plataforma CIAM

# Estado

Aceptado como decisión de referencia.

# Contexto

La organización requiere una plataforma de identidad para clientes y comercios que soporte autenticación moderna, OAuth2/OIDC, MFA, consentimientos, sesiones seguras, auditoría e integración con canales digitales.

# Alternativas

| Alternativa | Descripción |
|---|---|
| Plataforma CIAM SaaS | Servicio gestionado con capacidades avanzadas |
| Plataforma open source autogestionada | Mayor control y menor lock-in |
| Desarrollo interno | Construcción propia de identidad |

# Criterios

| Criterio | Peso |
|---|---:|
| Seguridad y cumplimiento | 25 |
| Time-to-market | 20 |
| OIDC/OAuth2/FAPI readiness | 20 |
| Operabilidad | 15 |
| Costo total | 10 |
| Flexibilidad | 10 |

# Decisión

Usar una plataforma CIAM especializada. La elección final puede ser SaaS u open source según restricciones de cumplimiento, operación y costos, pero se descarta construir identidad desde cero.

# Consecuencias

- Se centraliza autenticación y autorización.
- Los canales dejan de gestionar credenciales directamente.
- Se requiere gobierno de scopes, claims y políticas.
- Se deben definir patrones para apps públicas, APIs internas y terceros.
