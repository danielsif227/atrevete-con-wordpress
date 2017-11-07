## Instalar Wordpress en 000webhost \(powered by Hostinger\)

Esta es la opción recomendada para este curso, porque con ella se podrán probar todos los plugins que se quieran. Notar que este servicio es gratuito y en la zona de administración siempre hay que esperar varios segundos hasta que las operaciones se terminen, por lo tanto habrá que tener un poco de paciencia con la velocidad de carga de las páginas.

En primer lugar, habrá que ir a la página principal de 000webhost entrando en [https://es.000webhost.com](https://es.000webhost.com) y clic en “Registro gratis” para iniciar el proceso de creación de una nueva cuenta de usuario, lo cual te llevará a una página con un formulario para rellenar tu correo electrónico, una contraseña, y el nombre para tu sitio Web \(Website Name\). Lo que pongas como Website Name se utilizará en la dirección de acceso a tu curso. Por ejemplo si se pone _**cursowpaularagon**_, la dirección de acceso sería [https://_cursowpaularagon_.000webhostapp.com](https://cursowpaularagon.000webhostapp.com)

![](/assets/hosting0-alta.png)

![](/assets/hosting1-bienvenida.png)

Te enviarán un correo electrónico, que tendrás que abrir y hacer clic en el enlace de validación que recibas por email, para validar y finalizar la creación de usuario. Si no has recibido ningún email de validación, revisa la carpeta Spam, y si tampoco lo has recibido, en la web de haz clic en el “Menú de usuario - My Profile” \(se encuentra arriba a la derecha\) y luego clic en “Reenviar confirmación”.

![](/assets/hosting2-email.png)

Una vez que hayas confirmado el emal, en el sitio web [https://es.000webhost.com/](https://es.000webhost.com/) entra en el “Menú de usuario – My Profile”, que se encuentra en la esquina superior derecha, y cambia el idioma \(Language\) a español \(Spanish\).

![](/assets/hosting3-myprofile.png)

![](/assets/hosting4-es-es.png)

Para crear el sitio Wordpress, hay dos opciones: una opción automática, que resulta rápida y fácil pero que sólo está disponible en algunos servidores de alojamiento. Y otra opción manual, más lenta y costosa, pero más estándar, ya que los servidores de alojamiento web ofrecerán siempre una forma similar para instalar Wordpress.  
**Se recomienda optar por la opción 1 automática, por resultar rápida y fácil.**

_Adelanto el siguiente comentario una vez que hayas creado tu Wordpress: 000webhost.com ofrece servicio gratuito, por ello, durante 1h al día tu sitio web estará inactivo. Podráss elegir la hora de inactividad que prefieras en la siguiente opción:  
_

```
Menú de usuario - Mis sitios web - Ajustes (del sitio web) - General - Website sleeping time frame
```

#### OPCION 1 - AUTOMÁTICA \(rápida y fácil\)

Clic en el botón de la barra superior “Crear sitio web” y clic en "Instalar ahora" en “Build Wordpress Website”

![](/assets/hosting5-boton-crear.png)

![](/assets/hosting6-boton-crear-wp.png)

Te pedirá nombre de usuario Administrador. Por defecto pone admin, ¡¡¡pero cámbialo por cualquier otro nombre de usuario que desees!!! porque el hecho que el usuario Administrador se llame admin es un problema de seguridad. Por ejemplo, puedes poner tu apellido seguido de un guión y seguido de admin, pero siéntete libre de escoger el nombre de usuario que desees. Ponle una contraseña segura \(una contraseña segura puede tener las siguientes características: 8 dígitos o más, incluyendo mayúsculas, minúsculas, números, y otros caracteres\), y selecciona el idioma Spanish.

![](/assets/hosting7-crear-wp.png)

Posteriormente haz clic en el botón “Ve a la página de configuración” y entrarás en el panel de Administración de Wordpress.

![](/assets/hosting8-wp-creado.png)

La próxima vez que desees entrar a este panel, tendrás que escribir esta dirección web:

* [https://cursowpaularagon.000webhostapp.com/wp-admin/](https://cursowpaularagon.000webhostapp.com/wp-admin/) \(notar que deberás cambiar cursowpaularagon pro el nombre de tu sitio web\).

o también en esta dirección:

* [https://cursowpaularagon.000webhostapp.com/wp-login.php](https://cursowpaularagon.000webhostapp.com/wp-login.php) \(notar que deberás cambiar cursowpaularagon pro el nombre de tu sitio web\).

Es decir, es la dirección principal de tu sitio web seguido por /wp-admin/ o por /wp-login.php, y ahí intorudicr el nombre de usuario y contraseña.

La dirección web pública de tu blog será [https://cursowpaularagon.000webhostapp.com](https://cursowpaularagon.000webhostapp.com) \(notar que deberás cambiar cursowpaularagon pro el nombre de tu sitio web\).

#### OPCION 2 - MANUAL \(más lenta y costosa\)

Esta opción es más laboriosa, pero con mayor control y aprendizaje sobre la instalación de un sitio Wordpress desde cero. La idea de los pasos a realizar son similares en caso de instalar Wordpress manualmente en otro servidor. A modo de visión general, y teniendo en cuenta que este proceso puede realizarse de diversas formas, los pasos a realizar son:

1. Crear una base de datos en el servidor de hosting
2. Descargar y descomprimir el código fuente de Wordpress en nuestro PC
3. Subir el código fuente al servidor de hosting
4. Modificar la configuración de Wordpress para que se conecte con la Base de Datos

#### 1º Crear una base de datos en el servidor de hosting

Acceder al “Menú de usuario – Mis sitios web”

![](/assets/hosting10-acceder-listado-sitios-web.png)

Clic en “Administrar sitio web”

![](/assets/hosting11-admin-sitio-web.png)

Clic en “Administrar bases de datos”

![](/assets/hosting12-acceso-bd.png)

Clic en “Nueva Base de Datos”

![](/assets/hosting13-nueva-bd.png)

La Base de Datos \(para simplificar se denomina BD\) es el almacén donde se guardarán todas las entradas de texto que escribamos en nuestro blog. Cada Wordpress necesita disponer de una BD, junto con su usuario de BD y contraseña. Para evitar problemas, el nombre de la BD y el usuario de la BD convienen que estén en minúsculas, sin espacios ni caracteres extraños.

![](/assets/hosting14-crear-bd.png)

En este ejemplo se han introducido los siguientes datos, aunque puedes escoger los que quieras:

* Nombre de la BD: wordpressbd
* Nombre de usuario de la base de datos: usuariobd
* Contraseña: passwordbd

Una vez termine el proceso, la web nos muestra el nombre de Base de Datos y el nombre de Usuario definitivos, ya que el sistema de 000webhost modifica nuestros datos y les añade un número identificativo delante. En el caso del ejemplo, la web muestra los siguientes datos:

![](/assets/hosting14bis-datos-bd-reales.png)

Por lo tanto los datos finales que obtenemos son los siguientes:

* Nombre de la BD: id3443825\_wordpressbd
* Nombre de usuario de la base de datos: id3443825\_usuariobd
* Contraseña: passwordbd

Apúntate estos últimos datos que aparezcan en tu proceso de creación de la BD ya que se necesitarán posteriormente.

##### 2º Descargar y descomprimir el código fuente de Wordpress e nuestro PC

Ir a la web de Wordpress en castellano [https://es.wordpress.org/](https://es.wordpress.org/) y descargar el código fuente de Wordpress.

![](/assets/hosting15-descargaWP.png)

Descomprimir el archivo ZIP que hemos descargado. Para ello se recomienda tener descargado e instalado el programa 7-Zip, el cual puede descargarse en [http://www.7-zip.org](http://www.7-zip.org). También se podría utilizar WinZIP, WinRAR, etc. Una vez que tengas instalado 7-Zip, clic con el botón derecho del ratón en “wordpress-4.8.2-es\_ES.zip” - Extraer aquí. Como resultado aparecerá en nuestro PC una carpeta llamada wordpress  
.

![](/assets/hosting16-descomprimir.png)

##### 3º Subir el código fuente al servidor de hosting

El objetivo de estos pasos es conseguir **desplegar **el contenido del código fuente de Wordpress en la carpeta **public\_html** del servidor.  
 Para ello, accede a la zona de administración del sitio web en la página de 000webhost.com en “Menú de usuario -&gt; Mis sitios web -&gt; Administrar sitio web -&gt; Administrador de Archivos -&gt; Carga archivos ahora”

![](/assets/hosting17-acceso-archivos.png)

Seleccionar la carpeta /  y luego clic en el icono para subir ficheros que tiene forma de nube con una flecha, en nuestro PC seleccionar el fichero wordpress-4.8.2-es\_ES.ZIP que hemos descargado de [https://es.wordpress.org/](https://es.wordpress.org/) y subirlo con el botón Upload.

![](/assets/hosting18-uploadfile.png)

Descomprimir el archivo wordpress-4.8.2-es\_ES.ZIP que acabamos de subir al servidor con "botón derecho del ratón - Extract" y se creará una carpeta llamada wordpress.

![](/assets/hosting19-descomprimir.png)

Entrar en la carpeta wordpress que se ha creado y seleccionar todos los archivos. Para seleccionar todos:

1. Seleccionar el primero de todos haciendo clic sobre él.
2. Deslizarse hasta visualizar el último de todos los archivos.
3. Presionar y mantener presionada la tecla “shift” \(la tecla de mayúsculas, cuyo dibujo es una flecha que apunta hacia arriba, y que está en el teclado a la izquierda de la tecla Z, y también debajo de la tecla Intro\) y hacer clic sobre el último archivo. Y quedarán seleccionados todos los archivos
   .

Una vez que estén todos seleccionados, clic sobre la selección con el "botón derecho del ratón", y opción “Move”

![](/assets/hosting20-mover.png)

Haciendo clic en Change, cambiaremos la carpeta de destino a mover y seleccionaremos la carpeta **public\_html**, y finalmente clic en el botón "Select This".  
".

![](/assets/hosting21-cambiar carpeta destino.png)

![](/assets/hosting22-cambiar-carpeta.png)

![](/assets/hosting23-carpeta-public_html.png)

Ahora podremos borrar el archivo wordpress-4.8.2-es\_ES.ZIP y también podremos borrar la carpeta wordpress-4.8.2-es\_ES  
 haciendo clic con el botón derecho del ratón - Delete.

![](/assets/hosting25-delete.png)

##### 4º Modificar la configuración de Wordpress para que se conecte con la Base de Datos

Entrar en la carpeta **public\_html**, y ahí cambiar el nombre del archivo **wp-config-sample.php** por** wp-config.php**, dándole al “botón derecho del ratón – Rename”

![](/assets/hosting26-rename.png)

![](/assets/hosting27-rename2.png)

Clic en wp-config.php con el “botón derecho del ratón – Edit”

![](/assets/hosting28-edit.png)

Habrá que modificar en el archivo el nombre de la Base de Datos, el usuario de la Base de Datos y su password con los datos que nos habíamos apuntado en uno de los pasos anteriores. Siguiendo los datos de este paso a paso, las líneas a modificar quedarían así:

`define('DB_NAME', 'id3443825_wordpressbd');`

`define('DB_USER', 'id3443825_usuariobd');`

`define('DB_PASSWORD', ' passwordbd');`

**¡POR FIN!      
**

Si hemos realizado todo correctamente, ahora ya podemos acceder a la dirección web de nuestro sitio, que en el caso de este ejemplo sería [http://cursowpaularagon.000webhostapp.com](http://cursowpaularagon.000webhostapp.com) y veremos la página de instalación de Wordpress, en la cual vamos a poner el título principal de nuestro blog \(más tarde podremos cambiarlo\) y a crear un usuario ADMINISTRADOR de nuestro sitio web, con una contraseña y nuestro email. Evitaremos que el nombre de usuario sea admin, ya que es un problema de seguridad.

![](/assets/hosting29-instalar-wp.png)

Ahora podremos entrar al Escritorio de Administración de nuestro blog Wordpress a través de esta dirección:

[https://cursowpaularagon.000webhostapp.com/wp-login.php  ](https://cursowpaularagon.000webhostapp.com/wp-login.php)

o de esta otra:

[https://cursowpaularagon.000webhostapp.com/wp-admin/](https://cursowpaularagon.000webhostapp.com/wp-admin/)

#### ¿Cómo dar de baja la cuenta de usuario?

Una última anotación acerca de 000webhost: cuando termines el curso, si deseas cerrar definitivamente la cuenta que has creado en 000webhost.com y todos sus blog, en el “Menú de usuario – Mi Perfil”, la última opción es “**Cerrar cuenta**”.

