## Rutas importantes
- **`/var/www/html/`** → Carpeta principal de documentos web (DocumentRoot por defecto).
- **`/etc/apache2/sites-available/000-default.conf`** → Configuración del sitio web por defecto.
- **`/etc/apache2/sites-enabled/`** → Sitios activados en Apache.
- **`.htaccess`** → Archivo de configuración por directorio.

---

## Configuración básica

### DocumentRoot
Define el directorio donde Apache buscará los archivos a servir.

Ejemplo en `000-default.conf`:
```apache
<VirtualHost *:80>
    ServerAdmin webmaster@localhost
    DocumentRoot /var/www/html
</VirtualHost>
### Directorio principal

Configuración típica para permitir `.htaccess`:

```apache
<Directory /var/www/html>
    Options Indexes FollowSymLinks
    AllowOverride All
    Require all granted
</Directory>
```

---

## Archivos `.htaccess`

Permiten configurar reglas específicas sin editar la configuración principal.  
Ejemplo para redirigir errores y proteger archivos:

```apache
ErrorDocument 403 /error.html

<Files "secretito.html">
    Require all denied
</Files>
```

Explicación:

- **`ErrorDocument 403 /error.html`** → Redirige accesos prohibidos (403) a `error.html`.
    
- **`<Files "secretito.html"> Require all denied </Files>`** → Bloquea acceso al archivo `secretito.html`.
    

---
