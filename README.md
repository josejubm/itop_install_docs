
# ITOP INSTALL & CONFIGURATION

---

## Introduccion

**iTop** (IT Operations Portal) es una solución de gestión de servicios de TI (ITSM) que ayuda a las organizaciones a gestionar su infraestructura de TI, incidentes, problemas, cambios, solicitudes de servicio, y la CMDB (Base de Datos de Gestión de Configuración).  
Es ampliamente utilizado por empresas que desean centralizar su gestión de TI y mejorar el soporte técnico y la administración de activos.  

Algunas de las funcionalidades clave incluyen:  
- Gestión de incidentes y problemas.  
- Gestión de cambios y configuraciones.  
- Base de datos CMDB para activos y dependencias.  
- Informes y paneles personalizables.  

---

## Requisitos Especificos

> [!IMPORTANT]  
> Estos Requisitos de Hardware son Especificos de Esta Implementacion.
>
>| **OS**                      |**vCPUs**| **RAM**  | **FS** |
>|-----------------------------|---------|----------|--------|
>| RedHat Enterprise Linux 9.5 | 4 cores | 12 GB    | 10 GB  |
>
>
>### **Esquema recomendado de Particiones para Servidor Virtual (10 GB)**  
>
> | **Partición** | **Tamaño Sugerido** | **Descripción**                                                                        |
>|----------------|---------------------|----------------------------------------------------------------------------------------|
>| `/` (root)     | **7 GB**            | Contiene el sistema operativo, software principal (como iTop), y archivos esenciales.  |
>| `/home`        | **2 GB**            | Para archivos y configuraciones de usuarios locales.                                   |
>| `/boot/efi`    | **500 MB**          | Partición de arranque EFI necesaria si el servidor usa UEFI en lugar de BIOS.          |
>| `/boot`        | **500 MB**          | Para almacenar el kernel de Linux y archivos de arranque (Grub).                       |



---



## Requisitos Previos Generales 

| **Componente**         | **Requisito Mínimo**                          | **Recomendado**                          |
|------------------------|----------------------------------------------|------------------------------------------|
| **Servidor Web**       | Apache, Nginx                                | Apache 2.4+                              |
| **PHP**                | PHP 7.4 o superior                           | PHP 8.0 o superior                       |
| **Extensiones PHP**    | `mysqli`, `mbstring`, `gd`, `xml`, `json`, `curl` | Igual o más extensiones si necesario    |
| **Base de Datos**      | MySQL 5.7+ o MariaDB 10.3+                   | MySQL 8.0 o MariaDB más reciente         |
| **Espacio en Disco**   | 500 MB                                       | 1 GB (con datos adicionales)             |
| **RAM**                | 2 GB                                         | 4 GB o más, especialmente en producción  |
| **Sistema Operativo**  | Linux (Ubuntu/Debian/CentOS) o Windows       | Linux (Ubuntu 20.04+)                    |

---


## Dependecias



## Instalacion de Dependencias


### MYSQL


### APACHE (HTTPD)


## Instalacion de Itop


## Configuracion


## Conclucion

