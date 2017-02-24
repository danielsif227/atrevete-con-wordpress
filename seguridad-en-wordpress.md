## Conceptos generales sobre seguridad

El servidor puede configurarse para bloquear algunos ataques:

* Bloqueo de conexiones con patrones de Cross Site Scripting o SQL injection, etc.
* Bloqueo de conexiones por IP

Necesaria la **involucración **de los usuarios del Wordpress:

* Usar **contraseñas complejas**
* No dejarse sesiones abiertas en navegadores
* Mantener **actualizado **Wordpress, Plugins y Temas 
* Responsabilidad en la elección e instalación de Plugins y Temas: realizar búsquedas en Internet sobre posibles vulnerabilidades
* Usar **Plugins de seguridad**.

Hay que tener **copia de seguridad de todo**. _Si de algo no tienes copia de seguridad, quizás sea porque no te importa mucho perderlo..._

---

## Medidas de seguridad

Existen listados de vulnerabilidades conocidas de Wordpress, Plugins y Temas: [https://wpvulndb.com/](https://wpvulndb.com/)

* **Wordfence**: es un plugin completo: Escanea y Cortafuegos
* **Captcha by Bestwebsoft**: Añade un captcha en la página de login: un captcha solicita que se introduzca letras o números, con interacción con el usuario, para evitar múltiples intentos de acceso automáticos. Tiene opción de bloqueo de acceso ante errores de login, lo mismo que en Wordfence: Se pueden tener las dos en paralelo, y se aplicará el bloqueo que se dé en primer caso. 
* **Anti-Malware Security and Brute-Force Firewall**: Escaneo sencillo pero efectivo para detectar hackeos en el Wordpress
* **Plugin Security Scanner:** para revisar vulnerabilidades en tus otros plugins
* **All In One WP Security**: completo plugin de seguridad. Tiene algunas funcionalidades repetidas con Wordfence.

---

## Lo esencial

* No tener un usuario llamado **admin** ni un usuario llamado igual que nuestro Wordpress. Ocultar los nombres de los usuarios haciendo que cada usuario tenga un "alias" para mostrar diferente de su "nombre de usuario", lo cual se configura en el perfil de cada usuario.
* Mantener Wordpress, plugins y temas **actualizados**.
* Instalar y configurar **Wordfence**, para realizar escaneos de posibles ataques \(actúa como medida de detección y limpieza de malware\) y para bloquear conexiones detectadas como maliciosas \(actúa como firewall\). También sería recomendable instalar y configurar All in One WP Security.
* Poner un **captcha** para la página de login \(por ejemplo Captcha by Bestwebsoft\)
* Realizar **copias de seguridad** del Wordpress con UpdraftPlus y guardarlas por ejemplo en Dropbox

---

## Recuperar un Wordpress hackeado \(requiere acceso al alojamiento web\)

[https://codex.wordpress.org/FAQ\_My\_site\_was\_hacked](https://codex.wordpress.org/FAQ_My_site_was_hacked)

[https://www.wordfence.com/docs/how-to-clean-a-hacked-wordpress-site-using-wordfence/](https://www.wordfence.com/docs/how-to-clean-a-hacked-wordpress-site-using-wordfence/)

Herramienta para Administradores informáticos en busca de vulnerabilidades:

* [https://wpscans.com/](https://wpscans.com/)
* [https://wpscan.org/](https://wpscan.org/)



