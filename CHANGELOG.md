# Changelog

Todos los cambios notables en este proyecto serán documentados en este archivo.

El formato se basa en [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
y este proyecto se adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-05-28

### Added
- Implementación de arquitectura de **Alta Disponibilidad** con balanceador de carga Nginx.
- Nueva sección de configuración de Nginx Reverse Proxy en `docs/04-instalacion/servidor-web.md`.
- Diagramas Mermaid actualizados para mostrar la infraestructura con múltiples nodos web.
- Protocolo de mantenimiento sin caída del servicio en `docs/05-operacion.md`.
- Checklist de operación para el balanceador y salud de nodos esclavos.
- Gestión de incidentes comunes como "Error 502 Bad Gateway" y persistencia de sesiones.

### Changed
- Refactorización de `docs/04-instalacion/servidor-web.md` para incluir el rol de Nginx como terminador SSL.
- Actualización de `docs/05-operacion.md` con flujos operativos de balanceo.

## [1.0.0] - 2026-05-28

### Added
- Documento `docs/05-operacion.md` con la guía de mantenimiento diario, incluyendo diagramas Mermaid y tablas de checklist.
- Documento `docs/06-recuperacion.md` con el Plan de Recuperación ante Desastres (DRP), definiendo RTO, RPO y procedimientos de restauración.
- Procedimientos técnicos detallados para restauración de bases de datos y archivos web.
- Matriz de gravedad de incidentes y protocolos de actuación técnica.
- Diagrama de arquitectura técnica en `docs/02-diseno.md` con el flujo de tráfico y componentes.
- Diagrama de Gantt optimizado en `docs/03-planificacion.md` con el cronograma de fases del proyecto.
