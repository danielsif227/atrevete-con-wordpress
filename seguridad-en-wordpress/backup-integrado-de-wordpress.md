## Backup integrado de Wordpress

Sirve para copiar los **contenidos** de un sitio web Wordpress a otro sitio Wordpress.

**NOTA: **no copia la apariencia, configuración, estructura, etc.

El proceso a realizar es el siguiente:

#### 1º exportar:

```
Acceso en: Escritorio > Herramientas > Exportar
```

* Se genera un archivo .xml que se guarda en tu PC, que puede abrirse con un editor de textos \(recomendado usar notepad++\)
* Se guardan: Páginas, Entradas, Comentarios, Menú.
* **No se guarda: imágenes, plugins, temas, etc...**

#### 2º Importar

```
Acceso en: Escritorio > Herramientas > Importar
```

* Se utiliza el archivo .xml que se ha exportado a tu PC con anterioridad
* El sitio Wordpress antiguo **DEBE ESTAR FUNCIONANDO**
* En el proceso de "importación" las imágenes se copiarán desde el sitio Wordpress antiguo al nuevo sitio Wordpress
* Es necesario instalar temas y plugins y activar plugins en el sitio Wordpress destino

**CONCLUSION: **Necesitaremos una herramienta de copia de seguridad más completa: UpdraftPlus o BackWPup, por ejemplo.

