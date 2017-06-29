## Conceptos generales sobre seguridad

Desde la responsabilidad del servidor de alojamiento web, lo cual está fuera del alcance del administrador de Wordpress, se puede configurar para bloquear algunos ataques:

* Bloqueo de conexiones con patrones de Cross Site Scripting o SQL injection, etc.
* Bloqueo de conexiones por IP

Pero es necesaria la **involucración **de los usuarios del Wordpress:

* Usar **contraseñas complejas** en los usuarios.
* No dejarse sesiones abiertas en navegadores.
* Mantener **actualizado **Wordpress, Plugins y Temas.
* Responsabilidad en la elección e instalación de Plugins y Temas: Conviene encarecidamente realizar búsquedas en Internet sobre posibles vulnerabilidades
* Usar y configurar adecuadamente **Plugins de seguridad**.

Y sobre todo, hay que tener **copia de seguridad de todo**. _Si de algo no tienes copia de seguridad, quizás sea porque no te importa mucho perderlo..._

---

## Medidas de seguridad esenciales para Wordpress

* No tener un usuario llamado **admin** ni un usuario llamado igual que nuestro Wordpress. Ocultar los nombres de los usuarios haciendo que cada usuario tenga un "alias" para mostrar diferente de su "nombre de usuario", lo cual se configura en el perfil de cada usuario.
* Instalar y configurar **Wordfence** \(es un plugin completo: escaner y cortafuegos\), para realizar escaneos de posibles ataques \(actúa como medida de detección y limpieza de malware\) y para bloquear conexiones detectadas como maliciosas \(actúa como cortafuegos\).

* El plugin **Captcha by Bestwebsoft **añade un captcha en la página de login. Un captcha solicita que se introduzca letras o números, con interacción con el usuario, para evitar múltiples intentos de acceso automáticos. Tiene opción de bloqueo de acceso ante errores de login, lo mismo que en Wordfence: Se pueden tener las dos en paralelo, y se aplicará el bloqueo que se dé en primer caso.

* Realizar **copias de seguridad **del Wordpress con UpdraftPlus y guardarlas por ejemplo en Dropbox.

#### Recomendable:

* También sería recomendable instalar y configurar** All in One WP Security**, que es un completo plugin de seguridad. Tiene algunas funcionalidades repetidas con Wordfence.
* **Anti-Malware Security and Brute-Force Firewall**: Escaneo sencillo pero efectivo para detectar hackeos en el Wordpress
* **Plugin Security Scanner:** para revisar vulnerabilidades en tus otros plugins.

---

## Recuperar un Wordpress hackeado \(requiere acceso al alojamiento web\)

Aun con todo, existen listados de vulnerabilidades conocidas de Wordpress, Plugins y Temas: [https://wpvulndb.com/](https://wpvulndb.com/), y cada día van saliendo nuevas vulnerabilidades. En los siguientes enlaces encontraremos más información sobre qué hacer con un Wordpress hackeado:

[https://codex.wordpress.org/FAQ\_My\_site\_was\_hacked](https://codex.wordpress.org/FAQ_My_site_was_hacked)

[https://www.wordfence.com/docs/how-to-clean-a-hacked-wordpress-site-using-wordfence/](https://www.wordfence.com/docs/how-to-clean-a-hacked-wordpress-site-using-wordfence/)

A modo de prevención, estas webs serán muy útiles para Administradores informáticos en busca de vulnerabilidades:

* [https://wpscans.com/](https://wpscans.com/)
* [https://wpscan.org/](https://wpscan.org/)



