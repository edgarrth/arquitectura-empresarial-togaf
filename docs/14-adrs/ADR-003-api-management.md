# ADR-003: API Management como punto de gobierno

# Estado

Aceptado como decisión de referencia.

# Contexto

Existen múltiples integraciones internas y externas con criterios inconsistentes de seguridad, versionado, monitoreo y documentación.

# Decisión

Toda API externa y toda API interna reutilizable debe pasar por una capacidad de API Management y registrarse en el catálogo.

# Consecuencias

- Se estandariza seguridad con OAuth2/OIDC.
- Se habilita throttling, analytics y developer onboarding.
- Se reduce integración punto a punto.
- Se requiere gobierno de ciclo de vida API.
