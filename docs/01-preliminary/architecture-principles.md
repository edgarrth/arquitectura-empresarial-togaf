# Principios de arquitectura

# Principios corporativos

| ID | Principio | Declaración | Implicación |
|---|---|---|---|
| P-01 | Negocio primero | Toda decisión tecnológica debe mapearse a una capacidad, riesgo o resultado de negocio | No se aprueban tecnologías sin caso de uso claro |
| P-02 | Seguridad por diseño | Seguridad, privacidad y cumplimiento se incorporan desde el diseño | Todo servicio crítico requiere threat modeling |
| P-03 | APIs como producto | Las APIs son contratos empresariales versionados y gobernados | Toda API debe estar documentada, versionada y registrada |
| P-04 | Datos como activo | Los datos tienen ownership, clasificación, linaje y calidad | Cada dominio de datos requiere data owner |
| P-05 | Plataforma como producto | La plataforma interna debe reducir fricción a los equipos | Se priorizan golden paths y autoservicio |
| P-06 | Desacoplamiento progresivo | Los sistemas críticos deben evolucionar reduciendo acoplamiento | Nuevas integraciones deben evitar punto a punto no gobernado |
| P-07 | Observabilidad obligatoria | No se despliega software crítico sin logs, métricas, trazas y alertas | Observabilidad es criterio de salida |
| P-08 | Automatización sobre manualidad | Procesos repetitivos deben automatizarse | Cambios manuales en producción deben ser excepción |
| P-09 | Resiliencia explícita | Los sistemas financieros deben tolerar fallas parciales | Se requieren timeouts, retries, circuit breakers e idempotencia |
| P-10 | Cumplimiento trazable | Controles regulatorios deben evidenciarse | Las evidencias deben ser auditables |


