# Estrategia de Copias de Seguridad

Para garantizar la continuidad del negocio de la PYME, se establece una política de backups automáticos con rotación para evitar la pérdida de datos críticos.

## 1. Backup de Bases de Datos (MySQL)
Se utiliza la herramienta **mysqldump** para generar volcados de las bases de datos de la web corporativa y de gestión interna.

### Procedimiento Manual
Para realizar un respaldo de todas las bases de datos desde la consola:
```bash
# Exportación completa
mysqldump -u root -p --all-databases > /backup/db/full_backup_$(date +%F).sql