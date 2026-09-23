# SXE_01_CASAL


**GUÍA COMPLETA PARA DESPLEGAR WORDPRESS CON APACHE Y MYSQL.**

![WordPress](https://img.shields.io/badge/WordPress-5.8%2B-blue?style=for-the-badge&logo=wordpress)
![Apache](https://img.shields.io/badge/Apache-2.4-green?style=for-the-badge&logo=apache)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?style=for-the-badge&logo=mysql)

## ⬇️ INFORMACION RELEVANTE ⬇️

| Elemento | Lo que dice la documentación | Lo que necesita la VM | Otros (Comentarios que consideres relevantes) | Fuente de info: |
| :--- | :--- | :--- | :--- | :--- |
| **S.O.** | Sistema operativo basado en Linux compatible con la pila de software (Apache/Nginx, PHP, MySQL/MariaDB). | **Ubuntu 26.04.1 LTS** Server (64-bit) | Arquitectura de 64 bits (`amd64`). Al ser una versión LTS, cuenta con soporte extendido de 5 años. | ISO oficial (`ubuntu-26.04.1-live-server-amd64.iso`) |
| **Servidor web** | Apache o Nginx con el módulo `mod_rewrite` habilitado. | **Apache2** | Se escoge Apache por su conocimiento y uso previo | Documentación Oficial de WordPress |
| **Versión de PHP** | Versión **8.2.x o superior**  | **PHP 8.3**  | WordPress requiere de extensiones (`php-mysql`, `php-xml`, `php-gd`, `php-curl`). | Documentación Oficial de WordPress|
| **Gestor de BBDD** | **MySQL 8.0+** o **MariaDB 10.5+**. | **MySQL 8.0+** | Se elige MySQL por si conocimiento y uso previo | Documentación Oficial de WordPress |
| **Memoria y Disco** | **RAM:** Mínimo 512 MB (1–2 GB recomendados). **Disco:** 1 GB mínimo para WP + espacio para BD y medios. | **RAM:** 2 GB<br>**Disco:** 25 GB (VDI dinámico) | Para la VM se asignan 4 GB de RAM para asegurar fluidez durante el proceso de actualización de paquetes y 100 GB de almacenamiento. | Documentación oficial de Ubuntu Server |


📋 PASOS DE INSTALACIÓN 📋
---

### CREACION DE LA MAQUINA VIRTUAL
![](cap6.png)
---
### INSTALACION DE DEPENDENCIAS
![](cap7.png)
---
### DESCARGA Y EXTRACCION DE ARCHIVOS DE WORDPRESS EN EL DIRECTORIO DEL SERVIDOR
![](cap8.png)
---
### CONFIGURACIOND E APACHE

``nano etc/apache2/sites-available/wordpress.conf``

![](cap9.png)
---
### AÑADIR ``ServerName worpress.local``
![](cap13.png)
---
### INSTALACION DE ``mysql-server``
![](cap17.png)
---
### MYSQL INSTALADO Y FUNCIONAL
![](cap19.png)
---
### ``wordpress.local`` EN EL BUSCADOR DE LA MAQUINA FISICA
![](cap15.png)
![](cap16.png)
---
### CONFIGURACION INICIAL DE WORDPRESS
![](cap21.png)
![](cap23.png)
![](cap24.png)
![](cap25.png)
![](cap26.png)
---
### WORDPRES CONFIGURADO
![](cap27.png)
---

![Completado](https://img.shields.io/badge/Estado-Completado-success?style=for-the-badge)