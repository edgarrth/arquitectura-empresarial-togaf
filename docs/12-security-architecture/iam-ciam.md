# IAM & CIAM

# Alcance

CIAM cubre clientes, usuarios digitales, comercios y terceros externos. IAM corporativo cubre colaboradores, proveedores internos y accesos administrativos.

# Capacidades CIAM

| Capacidad | Descripción |
|---|---|
| Registro | Alta digital de cliente o comercio |
| Autenticación | Passwordless, MFA, biometría delegada, OTP cuando aplique |
| Autorización | Scopes, roles, consentimientos |
| Sesión | Gestión de tokens, refresh, revocación |
| Consentimiento | Registro auditable de consentimientos |
| Riesgo | Evaluación contextual por dispositivo, IP, comportamiento |
| Federación | Integración con partners o identidades externas |
| Auditoría | Eventos de login, fallos, cambios sensibles |

# Reglas

- Usar Authorization Code + PKCE para apps públicas.
- Evitar Resource Owner Password Credentials.
- Access tokens de corta duración.
- Refresh tokens rotables.
- Scopes por capacidad, no por pantalla.
- Claims mínimos necesarios.
- Separar CIAM de IAM administrativo.
- Registrar eventos de autenticación y autorización.
