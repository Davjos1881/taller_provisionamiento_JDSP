Parte web del taller:

Se creó la máquina virtual web con Vagrant usando la IP 192.168.56.10
Se utilizó el script provision-web.sh para instalar automáticamente Apache y **PHP dentro de la máquina

En la carpeta www/ del proyecto se encuentran los archivos del sitio:
- **index.html**
que modifiqué con sudo nano /var/www/html/index.html cambiar el contenido original por una pagina con mi nombre y la palabra "sopas"
- **info.php** 
Con un script en PHP que muestra un mensaje y la información del servidor
Ahora, modificandolo con **sudo nano /var/www/html/info.php** cambié el mensaje inicial para que mostrara mi nombre y la palabra "si" juntos con la informacion del servidor

Luego se ejecutó el comando `vagrant provision web`, lo que copió los archivos al directorio `/var/www/html/` de la máquina web

- Al acceder desde el navegador a **http://192.168.56.10/**, se mostró correctamente la página HTML con el mensaje de bienvenida
- Al acceder a **http://192.168.56.10/info.php**, se visualizó la página de PHP con el mensaje dinámico y la información del entorno PHP


