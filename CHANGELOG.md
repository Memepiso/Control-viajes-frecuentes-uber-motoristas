# Changelog - ⚡ Delivery S.O.S (MotoTaxi Pro)

All notable changes to this project will be documented in this file.

## [v0.4.0] - 2026-11-23
### Added
- **Columna dedicada "DÍA"**: Añadida una columna específica para la inicial del día de la semana (L, M, Mi, J, V, S, D) junto a la fecha en la tabla de reportes.
- **Cobro en Lote de Pendientes**: Botón "Marcar pendientes visibles como Cobrados" en la sección de Reportes y Cobros para actualizar instantáneamente todos los viajes pendientes filtrados a estado Cobrado.
- **Cuatro Estados de Viaje Detallados**: Incorporación de los estados *Agendado*, *Pendiente*, *Cobrado* y *Cancelado*.

### Changed
- **Nombre de Marca Optimizado**: Cambio a "⚡ Delivery S.O.S" (evitando caracteres combinados o raros que puedan cortarse en la interfaz o mostrarse como cuadros en WhatsApp).
- **Contenedor de Logo Nítido**: Logo ubicado en un contenedor circular/pastilla de fondo claro contrastado en la barra superior.
- **Resumen Financiero Mejorado**: Separación clara entre viajes *Agendados*, *Pendientes* y *Cobrados*. El saldo por cobrar suma exclusivamente los *Pendientes* (y el acumulado de realizados suma Pendientes + Cobrados, sin mezclar Cancelados ni Agendados futuros).
- **Migración Automática de Datos**: Conversión segura de estados antiguos ("Completado" -> "Pendiente") al cargar desde `localStorage`.
- **Documentación**: Actualización del registro de versiones en comentarios de `index.html` y en `CHANGELOG.md`.

## [v0.3.0] - 2026-11-23
### Added
- Nueva marca inicial, soporte de logo local `logo-delivery-sos.png`.
- Filtros avanzados en reportes (Quincenas, Mes completo, Rango personalizado y checkbox "Solo pendientes por cobrar").
- Días de la semana entre paréntesis en fechas y WhatsApp (`2026-11-02 (L)`).

### Changed
- Simplificación inicial de estados y cálculo de cuenta acumulada.

## [v0.2.0] - 2026-11-23
### Added
- Selector de pasajero en Resumen Quincenal para estado de cuenta individual.
- Botones "Enviar cuenta por WhatsApp" (`wa.me/504...`) y "Copiar Texto".

### Changed
- Moneda a Lempiras (L) y soporte de teléfonos de Honduras de 8 dígitos con prefijo automático +504.

## [v0.1.0] - 2026-11-23
### Added
- Versión inicial con Calendario interactivo, CRUD de pasajeros y respaldo JSON.
