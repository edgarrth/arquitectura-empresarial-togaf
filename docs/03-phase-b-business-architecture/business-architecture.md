# Business Architecture

# Value streams principales

La arquitectura de negocio se estructura alrededor de tres value streams principales: adquirir cliente, procesar pago y afiliar comercio. La siguiente vista ArchiMate representa el value stream de pagos porque es el flujo más crítico para una organización financiera de tarjetas, comercios y pagos digitales.

![Payment Value Stream View](../assets/diagrams/archimate/02-payment-value-stream-view.svg)

# Value streams cubiertos

## 1. Adquirir cliente

Objetivo: convertir un prospecto en cliente activo mediante registro digital, validación de identidad, evaluación de riesgo, aprobación y activación de producto.

## 2. Procesar pago

Objetivo: autorizar, evaluar riesgo/fraude, procesar, confirmar, conciliar y liquidar una transacción financiera.

## 3. Afiliar comercio

Objetivo: registrar, validar, evaluar, configurar y habilitar un comercio para operar dentro del ecosistema financiero.

# Modelo operativo objetivo

| Dominio | Owner de negocio | Owner tecnológico | KPIs |
|---|---|---|---|
| Cliente | Producto digital | Squad identidad/canales | Conversión, NPS, éxito login |
| Pagos | Operaciones pagos | Squad pagos | Autorizaciones exitosas, latencia |
| Comercio | Negocio comercios | Squad merchant platform | Alta comercio, volumen procesado |
| Riesgo | Riesgos | Squad risk platform | Precisión score, fraude evitado |
| Datos | Data Office | Data Platform | Calidad, linaje, disponibilidad |
| Plataforma | Tecnología | Platform Engineering | Lead time, disponibilidad, adopción |

# Reglas de negocio transversales

- Toda decisión de originación debe ser trazable.
- Toda transacción financiera debe ser idempotente.
- Todo evento de negocio relevante debe tener identificador único y timestamp.
- Toda operación sensible debe tener auditoría.
- Todo cambio contractual de API debe ser versionado.
