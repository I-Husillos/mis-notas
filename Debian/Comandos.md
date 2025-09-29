### Gestión de paquetes y privilegios
- **`apt update`** → Actualiza la lista de repositorios del sistema.

- **`apt upgrade -y`** → Instala las actualizaciones disponibles (con `-y` acepta automáticamente).

- **`su root`** → Cambia al usuario superadministrador (root).

- **`apt install openssh-server -y`** → Instala el servidor SSH.

- **`apt install apache2 -y`** → Instala el servidor web Apache.


### Servicios (systemd)
- **`systemctl start ssh`** → Inicia el servicio SSH.

- **`systemctl start apache2`** → " " " Apache.

- **`systemctl enable ssh`** → Activa SSH para que arranque automáticamente.

- **`systemctl enable apache2`** → " " " Apache.

- **`systemctl restart ssh`** → Reinicia el servicio SSH.

- **`systemctl restart apache2`** → → " " " Apache.

- **`systemctl status apache2`** → Muestra el estado del servicio Apache (`q` para salir).

- **`systemctl status ssh`** → " " " SSH (`q` para salir).

### Red y conexión SSH
- **`ip a`** → Muestra configuración de red e IP de la máquina.
    
- **`ssh usuario@IP`** → Conectar vía SSH (ejemplo: `ssh debian@10.179.26.37`).


### Archivos y directorios

- **`ls`** → Lista archivos del directorio actual.
    
- **`pwd`** → Muestra la ruta en la que estás.
    
- **`whoami`** → Muestra el usuario actual.
    
- **`nano archivo`** → Editor de texto en terminal.
    
- **`cat archivo`** → Muestra el contenido de un archivo.
    
- **`mkdir carpeta`** → Crea un nuevo directorio.



### Permisos y usuario web

- **Usuario `www-data`** → Usuario por defecto de Apache/Nginx para ejecutar procesos web.
    
- **`chown www-data:www-data archivo`** → Cambia propietario de un archivo a `www-data`.
    
- **`chown -R www-data:www-data carpeta`** → Cambia propietario de forma recursiva.

