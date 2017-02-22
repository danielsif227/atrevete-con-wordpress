## Crear un tema hijo

Si el Tema no admite añadir CSS, habrá que crear un tema hijo y subirlo al Wordpress. Nos ayudaremos del plugin File Manager para gestionar las carpetas y archivos del servidor.

1º Crear la carpeta generatepress-hijo en:

`public_html > wp-content > themes > generatepress-hijo`

2º subir el archivo style.css a la carpeta `public_html > wp-content > themes > generatepress-hijo > style.css`  con este contenido:

![](/assets/generatepress-hijo.png)

Líneas importantes:

* **Theme Name**: nuevo nombre para el tema hijo, diferente del nombre del tema padre.
* **Template**: debe ser el nombre exacto de la carpeta del tema padre. Con el plugin File Manager, podemos encontrar el nombre de la carpeta del tema GeneratePress., en concreto el nombre de la carpeta es **generatepress **\(respetar mayúsculas/minúsculas\)
* **@import url\("../generatepress/style.css"\);** Con esta línea se carga todo el tema padre. Las siguientes líneas serán modificaciones sobre el tema padre.

![](/assets/identificar-carpeta-tema.png)

Referencia: [https://www.webempresa.com/blog/crear-temas-hijo-child-themes-en-wordpress.html](https://www.webempresa.com/blog/crear-temas-hijo-child-themes-en-wordpress.html)

