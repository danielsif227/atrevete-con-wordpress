## Wordfence

#### ESCANEAR EL WORDPRESS

1º **Wordfence **compara lo que tenemos en nuestro servidor con los repositorios oficiales. **Por ello, primero requiere que tengamos todo actualizado.**

2º Hay que configurar las opciones de escaneo en `Wordfence Scan Options > Options`Hay que activar casi todas las opciones para un escaneo más profundo, revisando estas opciones:

* Scan theme files against repository versions for changes: Activar
* Scan plugin files against repository versions for changes: Activar
* Scan files outside your WordPress installation: Probar a activarlo porque realiza una búsqueda más profunda, pero si se activa, puede que el escaneo tarde muchísimo o que no termine nunca porque entre en un bucle.
* Scan images, binary, and other files as if they were executable: Ralentiza mucho pero puede llegar a ser útil en algún ataque muy concreto.
* Enable HIGH SENSITIVITY scanning \(may give false positives\): Habilita un escaneo muy sensible, si se activa puede que dé muchos falsos positivos.
* Use low resource scanning \(reduces server load by lengthening the scan duration\): Requerirá más tiempo para escanear con objeto de no sobrecargar el servidor

3º Se lanza con la opción SCAN:

```
Acceso en: Wordfence > Scan > Botón "Start a Wordfence scan"
```

**Resultados**: Hay veces que salen falsas alarmas, hay que analizarlas en profundidad.

---

#### FIREWALL

Wordfence incluye reglas para cortar conexiones que son detectadas como maliciosas. Hay que destacar la configuración de ataques por fuerza bruta.

```
Acceso en: Wordfence > Firewall > Brute Force Protection
```

* **Enforce strong passwords**: Activado. Exigir uso de passwords fuertes a todos/determinados roles de usuario
* **Lock out after how many login failures**:  Bloquear tu IP después de 20 fallos de login. Mejor reducir a 5.
* **Lock out after how many forgot password attempta:** Bloquear tu IP después de 20 fallos de recuperación de contraseña. Mejor reducir a 5.
* **Count failures over what time period: **Elegir periodo para contabilizar el número de fallos permitidos. por ej en los últimos 5 minotos, en la última hora...
* **Amount of time a user is locked out: **Tiempo en que se bloquea el acceso a un usuario
* **Immediately lock out invalid usernames:** Desactivado, si te equivocas en el login, te bloquea inmediatamente, muy seguro pero cuidado que puedes bloquearte el acceso con un único fallo.
* **Don't let WordPress reveal valid users in login errors**: Activado. No mostrar si el usuario era válido.
* **Prevent users registering 'admin' username if it doesn't exist: **Activado. Evitar que alguien escoja el usuario admin.
* **Immediately block the IP of users who try to sign in as these usernames:** Bloquear la IP de alguien que intenta entrar con esos usuarios. Por ej conviene poner: admin, administrator, wordpress, user, etc. 

---

#### LIMITAR TRÁFICO

Podemos visualizar el tráfico que hay en el instante:

```
Acceso en: Wordfence > Live Traffic
```

Wordfence permite limitar el tráfico de datos que se genera para evitar sobrecargas y caídas.

```
Acceso en: Wordfence > Firewall > Rate Limiting
```

* **Throttle =** regular el acceso: Wordpress responderá error 503 pero se seguirá permitiendo acceso posteriormente
* **Block =** bloquear acceso definitivamente. Poner block si tienes problemas con mucho tráfico de robots

* Immediately block fake Google crawlers: Activar

* How should we treat Google's crawlers: Treat Google like any other Crawler

* If anyone's requests exceed: 240 - throttle

* If a crawler's page views exceed: 240 - throttle
* If a crawler's pages not found \(404s\) exceed: 30 - block, para evitar que escaneen tu sitio ante vulnerabilidades
* If a human's page views exceed: 240 - throttle
* If a human's pages not found \(404s\) exceed: 30 - block
* If 404s for known vulnerable URLs exceed: 15 - block

How long is an IP address blocked when it breaks a rule: 1 hora

Parámetros sugeridos obtenidos de la ayuda de Wordfence: [https://docs.wordfence.com/en/Wordfence\_options?utm\_source=plugin&utm\_medium=pluginUI&utm\_campaign=docsIcon\#Rate\_Limiting\_Rules](https://docs.wordfence.com/en/Wordfence_options?utm_source=plugin&utm_medium=pluginUI&utm_campaign=docsIcon#Rate_Limiting_Rules)

