# Planificación del Proyecto

Este documento detalla el cronograma de implementación de la infraestructura LAMP, siguiendo una metodología de despliegue por fases para asegurar la estabilidad del sistema.

---

## 1. Cronograma de Despliegue (Gantt)

A continuación se muestra el diagrama de Gantt con las fases principales del proyecto:

```mermaid
gantt
    title Planificación del Despliegue LAMP
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m
    
    section Fase 1: Análisis
    Análisis de Requisitos       :done,    des1, 2026-05-20, 2026-05-22
    Diseño de Arquitectura       :done,    des2, 2026-05-22, 2026-05-24
    
    section Fase 2: Impl.
    Instalación SO y Firewall    :done,    ext1, 2026-05-24, 2026-05-25
    Configuración Apache y PHP   :done,    ext2, 2026-05-25, 2026-05-27
    Configuración MySQL          :done,    ext3, 2026-05-27, 2026-05-28
    
    section Fase 3: Oper.
    Monitorización y Logs        :active,  ops1, 2026-05-28, 2026-05-29
    Guía de Mantenimiento        :         ops2, 2026-05-29, 2026-05-30
    
    section Fase 4: Cierre
    Plan de Recuperación         :         fin1, 2026-05-30, 2026-05-31
    Validación Final             :         fin2, 2026-05-31, 1d
```

---

## 2. Desglose de Tareas

| Fase | Tarea Principal | Responsable | Estimación |
| :--- | :--- | :--- | :---: |
| **I** | Análisis y Diseño Técnico | yuseflc | 4 días |
| **II** | Instalación y Configuración LAMP | vjp-yuseflc | 3 días |
| **III** | Seguridad y Backup | yuseflc | 2 días |
| **IV** | Monitorización y Operaciones | vjp-yuseflc | 2 días |
| **V** | Pruebas de Recuperación | yuseflc | 2 días |

---

## 3. Hitos Clave (Milestones)

1.  **Hito 1 (2026-05-24):** Diseño de red y servidor validado.
2.  **Hito 2 (2026-05-27):** Pila LAMP operativa y accesible vía HTTPS.
3.  **Hito 3 (2026-05-30):** Sistema de backups y plan de desastres completado.
