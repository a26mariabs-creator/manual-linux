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
``