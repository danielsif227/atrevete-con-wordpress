#### Configurar que el respaldo de UpdraftPlus se realice en DROPBOX

Inicia sesión en Dropbox en otra pestaña del navegador. Y vuelve al Wordpress en la opción UpdraftPlus &gt; Ajustes:

![](/assets/Selección_026.png)

![](/assets/Selección_034.png)

![](/assets/Selección_027.png)

![](/assets/Selección_028.png)

![](/assets/Selección_029.png)

Podemos elegir si queremos que la copia se haga automáticamente con la periodicidad que digamos, o que la copia haya que hacerla manualmente.

![](/assets/Selección_030.png)

![](/assets/Selección_031.png)

Al terminar el proceso, la copia de respaldo estará en **Dropbox &gt; Aplicaciones &gt; UpdraftPlus.Com**

Si se lanza otra copia de respaldo hacia Dropbox, se guardará en esta misma carpeta UpdraftPlus.Com.

El nombre de los archivos de respaldo incluyen la fecha y la hora del respaldo.

![](/assets/Selección_033.png)

Al terminar el proceso, si no hubiéramos marcado la opción de "Borrar respaldos locales", la copia de respaldo la tendríamos **en el servidor,** ocupando un valioso espacio, y** **podríamos verlo con el plugin **File-Manager** en: `public_html > wp-content > updraft`

![](/assets/backup-en-servidor.png)

---

#### Configurar que el respaldo de UpdraftPlus se realice en GOOGLE DRIVE

Suponemos que ya tenemos creado un Proyecto en Google API. A ese proyecto, vamos a crearle unas nuevas "Credenciales" de "ID de cliente de OAuth" para permitir que UpdraftPlus se conecet a nuestra API de Google

1. Asegurarse que la Drive API está Habilitada: en [https://console.developers.google.com/](https://console.developers.google.com/) &gt; Panel de Control &gt; Habilitar API &gt; Drive API
2. Crear unas "Credenciales" de "ID de cliente de OAuth" tipo "Web" y obtendremos un ID y Secreto de cliente
3. Introducir ID y Secreto de cliente en Wordpress &gt; UpdraftPlus &gt; Ajustes

![](/assets/credenciales-api-gdrive-1.png)

![](/assets/credenciales-api-gdrive-2.png)

![](/assets/listado-credenciales-oauth.png)

![](/assets/cliente-id-updraftplus.png)

