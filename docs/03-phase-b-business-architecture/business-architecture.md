# Business Architecture

# Value streams principales

## 1. Adquirir cliente

```mermaid
flowchart LR
    A[Prospecto] --> B[Registro digital]
    B --> C[Validación identidad]
    C --> D[Evaluación riesgo]
    D --> E[Aprobación]
    E --> F[Activación producto]
```

## 2. Procesar pago

```mermaid
flowchart LR
    A[Cliente inicia pago] --> B[Autenticación / tokenización]
    B --> C[Autorización]
    C --> D[Antifraude]
    D --> E[Procesamiento]
    E --> F[Confirmación]
    F --> G[Conciliación]
    G --> H[Liquidación]
```

## 3. Afiliar comercio

```mermaid
flowchart LR
    A[Solicitud comercio] --> B[Validación KYC/KYB]
    B --> C[Evaluación riesgo]
    C --> D[Configuración condiciones]
    D --> E[Alta en plataforma]
    E --> F[Operación y liquidación]
```

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
