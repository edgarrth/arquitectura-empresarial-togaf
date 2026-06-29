# Business Capability Map

# Nivel 1

```mermaid
mindmap
  root((Financial Services Enterprise))
    Clientes
      Onboarding
      Identidad
      Atención
      Fidelización
    Productos
      Tarjetas
      Crédito
      Seguros asociados
      Beneficios
    Pagos
      Autorización
      Captura
      Reversas
      Disputas
    Comercios
      Afiliación
      Liquidación
      Portal comercio
      Riesgo comercio
    Riesgo
      Riesgo crediticio
      Riesgo transaccional
      Antifraude
      Cobranza
    Operaciones
      Conciliación
      Contabilidad
      Backoffice
      Reclamos
    Datos
      Gobierno de datos
      Analítica
      Modelos IA
      Reportería regulatoria
    Plataforma
      APIs
      Eventos
      Observabilidad
      CI/CD
```

# Capacidades priorizadas

| Capacidad | Madurez actual | Madurez objetivo | Prioridad | Justificación |
|---|---:|---:|---:|---|
| Identidad digital | 2 | 4 | Alta | Habilita canales, seguridad y experiencia omnicanal |
| API Management | 2 | 4 | Alta | Reduce integraciones punto a punto |
| Antifraude transaccional | 3 | 4 | Alta | Reduce pérdidas y mejora control |
| Conciliación automática | 2 | 4 | Alta | Reduce reprocesos operativos |
| Gobierno de datos | 2 | 4 | Alta | Base para analítica, IA y cumplimiento |
| Observabilidad | 2 | 4 | Alta | Reduce MTTR y mejora confiabilidad |
| DevEx / Golden Paths | 1 | 4 | Media | Acelera delivery y estandariza calidad |
| Fidelización | 3 | 4 | Media | Diferenciación comercial |

# Gaps principales

- No existe ownership claro por dominio de datos.
- APIs críticas no tienen catálogo ni versionado uniforme.
- Los flujos de pagos y conciliación dependen de procesos batch.
- Los equipos duplican lógica de cliente, riesgo y parámetros.
- La trazabilidad end-to-end es insuficiente para auditoría y soporte.
