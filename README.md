# Manual básico de Linux

Este repositorio contiene documentación básica
sobre administración de sistemas Linux.

## Contenidos
Gestión de usuarios
Permisos
Redes
Servicios

## Comandos útiles
Para consultar la configuración de red:
```bash
ip addr
```
Para comprobar la conectividad:
```bash
ping 8.8.8.8
```
## Gestión de servicios
Para consultar el estado de un servicio:
```bash
systemctl status nombre-servicio
```
Para reiniciar un servicio y aplicar cambios de configuración (requiere permisos de administrador):
```bash
sudo systemctl restart nombre-servicio
```

## Gestión de usuarios

Para crear un nuevo usuario en el sistema:
```bash
useradd nombre-usuario
```
Para eliminar un usuario del sistema:
```bash
userdel -r nombre-usuario
```

## Información del proyecto

Esta documentación se ha elaborado utilizando Markdown.
El control de versiones se realiza mediante Git
y el repositorio remoto se encuentra alojado en GitHub.

## Próximas mejoras
* Añadir un apartado sobre gestión de permisos y propietarios (`chmod` y `chown`).
* Incluir ejemplos prácticos de copias de seguridad y compresión (`tar` y `gzip`).
* Documentar el análisis de registros del sistema y logs (`journalctl`).

## Recomendaciones de seguridad
* Evitar el uso habitual de la cuenta `root` y emplear `sudo` únicamente para tareas administrativas puntuales.
* Configurar el cortafuegos (`ufw`) para bloquear conexiones entrantes innecesarias y mantener solo abiertos los puertos esenciales.
* Asignar permisos restrictivos (`chmod`) a archivos de configuración críticos y realizar copias de seguridad periódicas.