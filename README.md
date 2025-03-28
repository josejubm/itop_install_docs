
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



## Dependecias

# **Dependencias para la Instalación de iTop**  

| **Componente**            | **Descripción**                                                                 |
|---------------------------|---------------------------------------------------------------------------------|
| **PHP**                    | Versión 7.4 o superior. Requiere varias extensiones.                            |
| **Extensiones PHP**        | - `mysqli` (para la base de datos MySQL/MariaDB)                               |
|                           | - `mbstring` (para manejar cadenas multibyte)                                  |
|                           | - `gd` (para manipulación de imágenes, útil para los informes)                |
|                           | - `xml` (para procesamiento de XML)                                           |
|                           | - `json` (para manipulación de datos JSON)                                     |
|                           | - `curl` (para realizar solicitudes HTTP desde PHP)                            |
| **Base de Datos**          | - **MySQL** 5.7 o superior o **MariaDB** 10.3 o superior.                      |
| **Servidor Web**           | - **Apache** (2.4 o superior) o **Nginx**                                        |
| **Servidor de correo**     | - Para enviar correos electrónicos (opcional para notificaciones)               |
| **Comando `composer`**     | Herramienta de gestión de dependencias de PHP. Necesaria para gestionar dependencias de iTop. |
| **Cron**                   | Para programar tareas de mantenimiento y limpieza de la base de datos (opcional). |

---

> [!NOTE]
>### **Importante:**
>- **PHP:** Asegúrate de que todas las extensiones estén habilitadas antes de la instalación. Si alguna falta, iTop podría no funcionar correctamente.
> - **Base de Datos:** La base de datos de iTop debe estar configurada antes de comenzar la instalación.  
> - **Servidor Web:** Se recomienda Apache, ya que es compatible y tiene una configuración más sencilla con iTop.


## Instalacion de Dependencias

### MariaDB

#### Paso 1 instalacion
```bash
sudo dnf install -y mariadb-server mariadb
```
#### Paso 2 configuracion


### MYSQL


### APACHE (HTTPD)


## Instalacion de Itop


## Configuracion


## Conclucion

