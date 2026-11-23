# Changelog - ⚡Delivery 𝗦.𝗢.𝗦̈⃝™ (MotoTaxi Pro)

All notable changes to this project will be documented in this file.

## [v0.3.0] - 2026-11-23
### Added
- **Nueva Marca y Logo**: Actualización de la marca visible en cabecera y mensajes de WhatsApp a "⚡Delivery 𝗦.𝗢.𝗦̈⃝™" con soporte para archivo local `logo-delivery-sos.png` (y respaldo de icono elegante).
- **Filtros Avanzados en Reportes**: Renombrado de pestaña a "Reportes y Cobros" con opciones de filtrado por *1ª Quincena (1–15)*, *2ª Quincena (16–fin)*, *Mes completo* y *Rango personalizado* (con fechas de inicio y fin).
- **Filtro de Pendientes**: Checkbox "Solo pendientes por cobrar" para generar cuentas exclusivas sin incluir lo ya pagado.
- **Días de la Semana en Fechas**: Inclusión automática de la inicial del día de la semana en todas las fechas mostradas y en los mensajes de WhatsApp (ej. `2026-11-02 (L)`).
- **Documentación de Versiones**: Creación de `CHANGELOG.md` y comentarios de historial de versiones en `index.html`.

### Changed
- **Simplificación de Estados de Viaje**: Reducción a tres estados (*Pendiente*, *Cobrado*, *Cancelado*). Migración automática de viajes antiguos con estado "Completado" a "Pendiente" al cargar.
- **Cálculo de Cuenta Acumulada**: El total acumulado suma *Pendiente* + *Cobrado* (excluyendo cancelados), desglosando claramente lo pendiente por cobrar frente a lo ya cobrado.

## [v0.2.0] - 2026-11-23
### Added
- Selector de pasajero en Resumen Quincenal para ver estados de cuenta individuales.
- Botones "Enviar cuenta por WhatsApp" (`wa.me/504...`) y "Copiar Texto" con resumen detallado de fechas, rutas, extras y total.
- Desglose detallado por estado en tarjetas KPI y tabla quincenal.

### Changed
- Adaptación completa de moneda a Lempiras (L).
- Soporte para teléfonos de Honduras de 8 dígitos con prefijo automático +504.

## [v0.1.0] - 2026-11-23
### Added
- Versión inicial de MotoTaxi Pro con Calendario interactivo de viajes, módulo CRUD de pasajeros y resumen quincenal básico.
- Sistema de respaldos y restauración en formato JSON (`localStorage`).
