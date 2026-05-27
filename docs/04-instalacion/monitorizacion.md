# Monitorización del Sistema

Este documento describe las herramientas y procedimientos para supervisar la salud y el rendimiento de la infraestructura LAMP de la PYME.

## 1. Monitorización en Tiempo Real (Netdata)
Para una supervisión visual y sencilla, se utiliza **Netdata**, que permite controlar el uso de CPU, RAM y tráfico de red desde un panel web.
*   **Estado del servicio:** Se puede verificar con `sudo systemctl status netdata`.

## 2. Análisis de Logs de Apache
Para auditar el tráfico web y detectar errores de acceso, se implementa **GoAccess**, un analizador de logs interactivo.

### Instalación de GoAccess
```bash
# Añadir repositorio oficial e instalar
wget -O - https://deb.goaccess.io/gnugpg.key | sudo apt-key add -
echo "deb http://deb.goaccess.io/ $(lsb_release -cs) main" | sudo tee -a /etc/apt/sources.list.d/goaccess.list
sudo apt-get update
sudo apt-get install goaccess