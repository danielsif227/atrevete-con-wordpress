## All In One WP Security

Permite habilitar numerosas medidas de seguridad \(algunas ya están en Wordfence\) para nuestro Wordpress. Se configura en `Listado de Plugins > All In One WP Security > Settings`. Este plugin indica el grado de protección que tenemos con un interesante gráfico en forma de cuentakilómetros.

#### C**ambiar la dirección de acceso al Escritorio de Wordpress**

La opción más interesante a configurar consiste en **cambiar la dirección de acceso al Escritorio de Wordpress**, de forma que ya no sea [http://nombredelwordpress.es/wp-admin/](#), sino que escojamos una dirección diferente a **wp-admin**, para evitar que la gente maliciosa intente acceder a nuestro Wordpress entrando por la dirección por defecto wp-admin que es conocida por todo el mundo. Una vez cambiado, desconocerán cual es la dirección de acceso al Escritorio. Se configura en:

**`Fuerza Bruta> Cambiar el nombre de la página de entrada > Login Page URL: mizonagestion`**

Ahí conviene que cada administrador de Wordpress escoja el nombre que desee, incluso con un nombre diferente a "mizonagestion", para que no sea tan genérico. De esta forma, la nueva dirección de acceso al Escritorio será similar a:

[http://nombredelwordpress.es/mizonagestion/](http://nombredelwordpress.es/mizonagestion/)

#### Otras opciones a revisar de este plugin:

* Opciones &gt; WP Version Info: Eliminar generador WP Meta Info: SI
* Cuentas de usuario &gt; Mostrar nombre: Revisa que los Nombres de usuario estén ocultos y se muestre el alias
* Ingreso de usuarios &gt; Activar característica de bloqueo de inicio de sesión: SI
* Ingreso de usuarios &gt; Cerrar inicio de sesión: múltiples opciones
* Ingreso de usuarios &gt; Forzar salir &gt; Habilitar el cierre de sesión de usuario de Fuerza WP: si
* Ingreso de usuarios &gt; Mostrar mensaje de error genérico: SI
* Seguridad del sistema de archivos: Deshabilitar "Edición archivo PHP".
* Seguridad del sistema de archivos &gt; WP acceso archivo &gt; Impedir el Acceso a Archivos de Instalación Predeterminada de WP: si
* Cortafuegos &gt; Reglas basicas de Cortafuegos &gt; Habilitar proteccion basica de Firewall: SI
* Cortafuegos &gt; Reglas basicas de Cortafuegos &gt; Bloquear el Acceso al Archivo debug.log : SI
* Cortafuegos &gt; Reglas basicas de Cortafuegos &gt; Bots  de Internet &gt; Bloquear falsos Googlebots: SI
* Cortafuegos &gt; Prevenir enlaces activos &gt; Evitar Hotlinking de Una Imagen: SI
* Fuerza Bruta &gt; Login Captcha &gt; Habilitar capcha en pagina de ingreso: SI

* Fuerza Bruta &gt; Login Captcha &gt; Habilitar Captcha en Página de recuperar contraseña: SI

* Fuerza Bruta &gt; Honeypot &gt; Habilitar Honeypot En La Página De Entrada : SI
* Escáner: detección de cambios en los archivos, porque si hay cambios no deseados es probable que sean hackeos.



