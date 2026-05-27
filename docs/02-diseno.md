# Diseño de la Infraestructura

Este documento describe la arquitectura técnica, las versiones de software y el diseño de red para la implementación de la pila **LAMP**.

## 1. Especificaciones de Software (Versiones)
Para garantizar la compatibilidad y seguridad del sistema, se han definido las siguientes versiones de los componentes principales:

| Componente | Versión | Descripción |
| :--- | :--- | :--- |
| **Apache** | 2.4.57 | Servidor web (versión actualizada) |
| **MySQL** | 8.0 | Sistema de gestión de bases de datos |
| **PHP** | 8.1+ | Lenguaje de programación de servidor |
| **Certbot** | 2.9 | Herramienta para SSL/TLS automático |

## 2. Diseño de Red y Seguridad
La infraestructura se organiza para proteger los datos de la PYME mediante el filtrado de tráfico con **UFW**.

### Puertos y Accesos
| Servicio | Puerto | Protocolo | Descripción |
| :--- | :--- | :--- | :--- |
| **SSH** | 22 | TCP | Administración remota segura |
| **HTTP** | 80 | TCP | Tráfico web (redirección a HTTPS) |
| **HTTPS** | 443 | TCP | Tráfico web cifrado (SSL/TLS) |

## 3. Arquitectura del Sistema
1.  **Capa de Aplicación:** El servidor **Apache** procesa las peticiones externas. Los archivos de configuración se gestionan en `/etc/apache2/`.
2.  **Capa de Datos:** **MySQL** aloja las bases de datos para la web corporativa y la gestión interna.
3.  **Seguridad:** Se implementan reglas de "denegación por defecto" en el firewall, permitiendo solo los puertos de la tabla anterior.
Notas sobre los cambios realizados: