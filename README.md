# Documentación del despliegue LAMP con monitorización en Alta Disponibilidad

Este repositorio contiene la arquitectura técnica definitiva para el despliegue de una infraestructura LAMP escalable. El proyecto ha evolucionado desde una solución básica monolitica hasta un entorno de alta disponibilidad diseñado para entornos de producción reales.

## Autores y Colaboración
- **yuseflc**: Arquitecto de plataforma (Análisis, Diseño y Configuración Crítica).
- **vjp-yuseflc**: Especialista en operaciones (Seguridad, Hardening y DRP).

## Estructura del Repositorio

```text
proyecto-git-md/
├── CHANGELOG.md             # Línea de tiempo de versiones
├── README.md                # Portada y visión general
├── REVISION.md              # Auditoría de documentos
├── tareas.md                # Control de hitos
└── docs/                    # Base de conocimiento
    ├── 01-analisis.md       # Necesidades del negocio
    ├── 02-diseno.md         # Planos técnicos
    ├── 03-planificacion.md  # Roadmap
    ├── 05-operacion.md      # Manual de campo para administradores
    ├── 06-recuperacion.md   # Protocolos de emergencia (DRP)
    └── 04-instalacion/      # Guías de despliegue paso a paso
        ├── backups.md       # Políticas de respaldo
        ├── base-de-datos.md # Hardening de MySQL 8.0
        ├── monitorizacion.md # Netdata y observabilidad
        ├── servidor-web.md   # Balanceo con Nginx + Apache
        └── ssh-firewall.md  # Seguridad perimetral UFW
```

## Resumen de Capacidades
- **Disponibilidad**: ~~Servidor único~~ -> Nodos escalables tras un Proxy Inverso (Nginx).
- **Seguridad**: Filtrado de tráfico estricto y acceso exclusivo mediante llaves criptográficas.
- **Observabilidad**: Telemetría en tiempo real y análisis de logs interactivo.
- **Resiliencia**: Recuperación garantizada ante pérdida de datos en menos de 4 horas.

---

## Reflexión de Cierre

La construcción de este proyecto ha representado un desafío técnico en la integración de múltiples capas de software. Lo que comenzó como un simple servidor web se ha transformado en una infraestructura robusta capaz de resistir fallos en nodos individuales sin interrumpir el servicio. ~~Aprender a configurar un balanceador fue fácil~~ La verdadera dificultad residió en asegurar que la capa de datos y la seguridad perimetral fueran consistentes en todo momento.

Este repositorio no es solo una colección de manuales; es el resultado de un proceso de diseño iterativo donde cada decisión técnica ha sido auditada y documentada para asegurar su escalabilidad a futuro.

*Responsable:* **Yusef Laroussi de la Calle**
