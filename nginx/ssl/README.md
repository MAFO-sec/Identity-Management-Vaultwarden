# Certificados SSL

En esta carpeta se deben alojar los certificados necesarios para el funcionamiento de Nginx con HTTPS.

### Archivos requeridos:
* `vault.brswindows.lab.crt`: Certificado de la entidad (o autofirmado).
* `vault.brswindows.lab.key`: Llave privada del certificado.

### Instrucciones para entorno de laboratorio:
Si estás en un entorno de pruebas, puedes generar estos certificados usando OpenSSL con el archivo de configuración `openssl-san.conf` (disponible en la documentación de la carpeta `/docs`).
