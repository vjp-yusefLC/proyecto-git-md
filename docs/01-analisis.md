# Análisis de Requisitos - Infraestructura LAMP para PYME

Este documento detalla las necesidades identificadas para la puesta en marcha de la presencia web y el sistema de gestión interna del cliente.

## 1. Objetivos del Proyecto
El cliente, una **pequeña empresa (PYME)**, requiere una solución robusta para:
*   Desplegar su **presencia web corporativa**.
*   Implementar un **sistema de gestión interna**.
*   Garantizar la seguridad de los datos y la disponibilidad del servicio.

## 2. Requisitos Funcionales
Para satisfacer estas necesidades, la infraestructura debe contar con:
*   **Servidor Web:** Capacidad para servir contenido dinámico mediante un servidor **Apache con PHP**.
*   **Gestión de Datos:** Un sistema de base de datos **MySQL/MariaDB** que aloje al menos dos bases de datos (una para el sitio web y otra para la gestión interna).
*   **Acceso Remoto:** Un método de administración segura a través de **SSH**.

## 3. Requisitos No Funcionales y Mantenimiento
La consultora debe asegurar la operatividad mediante:
*   **Seguridad Activa:** Configuración de un firewall básico utilizando **UFW** para filtrar el tráfico.
*   **Monitorización:** Implementación de herramientas (como **Netdata**) para supervisar el estado del sistema en tiempo real.
*   **Respaldo de Información:** Estrategia de **copias de seguridad automáticas** (utilizando `mysqldump` y `rsync`) con un sistema de rotación de archivos.
*   **Plan de Recuperación:** Documentación detallada para actuar ante posibles desastres y# Análisis de Requisitos - Infraestructura LAMP para PYME

Este documento detalla las necesidades identificadas para la puesta en marcha de la presencia web y el sistema de gestión interna del cliente.