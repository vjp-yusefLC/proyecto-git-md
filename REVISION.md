# Historial de Revisiones del Proyecto

Este documento registra las revisiones del proyecto, el estado de cada sección y los responsables de la validación de la documentación.

---

## 1. Estado de la Documentación

| Documento | Estado | Última Revisión | Revisor | Observaciones |
| :--- | :---: | :---: | :---: | :--- |
| [01-analisis.md](./docs/01-analisis.md) | Completo | 2026-05-28 | yuseflc | - |
| [02-diseno.md](./docs/02-diseno.md) | Completo | 2026-05-28 | yuseflc | - |
| [03-planificacion.md](./docs/03-planificacion.md) | Completo | 2026-05-28 | yuseflc | - |
| [04-instalacion/](./docs/04-instalacion/) | Completo | 2026-05-28 | vjp-yuseflc | Servidor Web y Balanceador finalizados |
| [05-operacion.md](./docs/05-operacion.md) | Completo | 2026-05-28 | vjp-yuseflc | Añadidas tareas de balanceo |
| [06-recuperacion.md](./docs/06-recuperacion.md) | Completo | 2026-05-28 | vjp-yuseflc | Plan DRP aprobado |

---

## 2. Registro de Revisiones

### Revisión v1.1.0 (2026-05-28)
- **Responsable:** vjp-yuseflc (Documentalista de operaciones)
- **Cambios realizados:**
    - Se ha completado la sección de operaciones con procedimientos de mantenimiento preventivo.
    - Se ha diseñado el Plan de Recuperación ante Desastres (DRP) con protocolos técnicos de restauración.
    - Actualización de enlaces transversales entre documentos de instalación y operación.
    - Integración de diagrama de arquitectura y tabla de componentes en el diseño.
    - Refactorización del diagrama de Gantt para mejorar la legibilidad y cronología.
- **Resultado:** Aprobado para pruebas de concepto.
    - Se ha incorporado la arquitectura de alta disponibilidad con Nginx.
    - Actualización de `servidor-web.md` con configuración de Proxy Inverso.
    - Inclusión de manual de operación para balanceadores en `05-operacion.md`.
    - Revisión de errores críticos (502 Bad Gateway).
- **Resultado:** Aprobado para despliegue en producción.

### Revisión v1.2.0 (2026-05-28)
- **Responsable:** vjp-yuseflc
- **Cambios realizados:** Versión inicial completa con LAMP, Monitorización y DRP.

---

## 3. Control de Versiones de Documentación

| Versión | Fecha | Autor | Descripción |
| :---: | :---: | :--- | :--- |
| **0.1.0** | 2026-05-20 | yuseflc | Estructura inicial |
| **1.0.0** | 2026-05-28 | vjp-yuseflc | Operación y recuperación completa |
| **1.1.0** | 2026-05-28 | yuseflc | **Versión Actual:** Balanceador y Alta Disponibilidad |
