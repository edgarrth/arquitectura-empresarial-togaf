# Data Governance

# Modelo de gobierno

| Rol | Responsabilidad |
|---|---|
| Data Owner | Define reglas de uso, calidad y acceso del dominio |
| Data Steward | Mantiene definiciones, glosario y calidad |
| Data Custodian | Administra plataforma y controles técnicos |
| Data Consumer | Usa datos bajo políticas aprobadas |
| Data Governance Council | Prioriza dominios, políticas y conflictos |

# Clasificación de datos

| Clasificación | Ejemplos | Control mínimo |
|---|---|---|
| Público | Información institucional | Integridad |
| Interno | Catálogos, parámetros no sensibles | Acceso corporativo |
| Confidencial | Datos cliente, scoring, contratos | Cifrado, RBAC, auditoría |
| Restringido | PAN, credenciales, secretos, biometría | Tokenización, segregación, monitoreo |

# Reglas de calidad

| Dimensión | Ejemplo de regla |
|---|---|
| Completitud | Cliente activo debe tener documento, estado y fecha de alta |
| Unicidad | Documento de identidad no debe duplicarse para clientes activos |
| Validez | Estado de transacción debe pertenecer a catálogo aprobado |
| Consistencia | Monto liquidado debe reconciliar con monto autorizado y comisiones |
| Oportunidad | Eventos críticos deben estar disponibles en menos de 5 minutos |

# Glosario mínimo

| Término | Definición |
|---|---|
| Autorización | Evaluación de una transacción para aprobarla, denegarla o derivarla |
| Conciliación | Comparación entre registros internos y externos para identificar diferencias |
| Liquidación | Proceso de cálculo y pago de fondos a comercios o contrapartes |
| Score | Resultado numérico de un modelo o regla de riesgo |
| Tokenización | Sustitución de un dato sensible por un token no explotable fuera del sistema autorizado |
