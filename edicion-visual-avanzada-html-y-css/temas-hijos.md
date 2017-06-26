## Crear un tema hijo

Siguiendo el **ejemplo práctico **del apartado anterior consistente en modificar la altura del menú, otra opción de realizar este cambio sería creando un "tema hijo" del tema **GeneratePress**, y haciendo activo en el Wordpress el nuevo tema hijo. Un tema hijo hereda todas las propiedades del tema padre y añade nuevo CSS con el que se puede añadir, modificar o anular el CSS del tema padre. En caso que el tema visual de Worpress no admitiera añadir CSS, no quedaría más opción que optar por esta opción de crear un tema hijo y subirlo al Wordpress. A continuación veremos cómo realizarlo. Para ello nos ayudaremos del plugin File Manager para gestionar las carpetas y archivos del servidor, para lo cual necesitaremos disponer de un Wordpress que disponga de este plugin o con posibilidad de instalar dicho plugin.

1º Crear la carpeta generatepress-hijo en:

`public_html > wp-content > themes > generatepress-hijo`

2º subir el archivo style.css a la carpeta `public_html > wp-content > themes > generatepress-hijo > style.css`  con este contenido, el cual ha sido extraído en el apartado anterior cambiando en vivo el CSS en el navegador:

![](/assets/generatepress-hijo.png)

Líneas importantes:

* **Theme Name**: nuevo nombre para el tema hijo, que debe ser diferente del nombre del tema padre.
* **Template**: debe ser el nombre exacto de la carpeta del tema padre. Con el plugin File Manager, podemos encontrar el nombre de la carpeta del tema GeneratePress., en concreto el nombre de la carpeta es **generatepress **\(respetar mayúsculas/minúsculas\)
* **@import url\("../generatepress/style.css"\);** Con esta línea se carga todo el tema padre. 
* El resto de líneas serán modificaciones del CSS del tema padre.

3º Por último, habrá que cambiar el tema de nuestro Wordpress y seleccionar GeneratePress-Hijo, momento a partir del cual la altura del menú cambiará de 60px a 40px.



En la siguiente imagen se ve dónde está ubicado el archivo style.css del tema padre.![](/assets/identificar-carpeta-tema.png)

Referencia: [https://www.webempresa.com/blog/crear-temas-hijo-child-themes-en-wordpress.html](https://www.webempresa.com/blog/crear-temas-hijo-child-themes-en-wordpress.html)

