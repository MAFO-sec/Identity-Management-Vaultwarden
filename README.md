# 🛡️ Gestión de Identidades: Vaultwarden + Active Directory

Este proyecto presenta la implementación de un sistema de gestión de credenciales autohospedado y seguro, integrado con servicios de directorio empresarial (Active Directory).

## 🚀 Descripción del Proyecto
Implementación de un entorno de seguridad para la gestión de contraseñas utilizando **Vaultwarden** en contenedores Docker. La solución incluye un proxy inverso con **Nginx** para asegurar el tráfico mediante **SSL/TLS** y la integración con **Windows Server** a través de **Bitwarden Connector** para la sincronización automática de identidades.

## 🛠️ Stack Tecnológico
* **Servidor de Contraseñas:** Vaultwarden (Rust implementation).
* **Infraestructura:** Docker & Docker Compose.
* **Servicios de Directorio:** Active Directory (Windows Server 2019).
* **Proxy Inverso:** Nginx con certificados OpenSSL (SAN).
* **Servidor SMTP (Pruebas):** Mailpit.

## 📂 Estructura del Repositorio
* `/docker`: Configuración del despliegue con Docker Compose.
* `/nginx`: Archivos de configuración del servidor web y parámetros SSL.
* `/docs`: Guía técnica detallada paso a paso en formato PDF.

## 🧪 Laboratorios Realizados
1.  **Hardening de Red:** Configuración de Nginx para forzar HTTPS y uso de certificados con nombres alternativos (SAN).
2.  **Sincronización de Usuarios:** Configuración de Bitwarden Connector para mapear Unidades Organizativas (OUs) de AD.
3.  **Gestión de Ciclo de Vida:** Pruebas de alta, baja y cambio de departamento de usuarios, verificando la propagación de permisos en tiempo real.

---
*Desarrollado por **MAFO-sec** como parte de formación en Ciberseguridad.*
