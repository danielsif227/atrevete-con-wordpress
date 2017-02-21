## Embeber archivos de Google Drive en Wordpress

#### Uso

Google Apps Login + Google Drive Embedder: Con la combinación de estos plugins se podrá añadir archivos de Google Drive embebidos en las entradas del Wordpress:

![](/assets/g_embedder_uso.png)

#### Configuración de conexión de Wordpress con Google Drive

Para poder usar Google Drive Embedder, hay que conectar Wordpress con Google API. Para ello hay que ir a la web de Google Analytics [https://analytics.google.com](https://analytics.google.com/) y crear una nueva cuenta desde la zona de ADMINISTRADOR:

![](/assets/g_embedder_paso1.png)

Rellenamos los datos de la cuenta de Universal Analytics:

![](/assets/g_embedder_paso2.png)

Y podemos desactivar las opciones de Compartición de datos, haciendo clic en el botón de Obtener ID de seguimiento:

![](/assets/g_embedder_paso3.png)

En la Configuración de la propiedad, podremos obtener el Id de seguimiento de Universal Analytics:

![](/assets/g_embedder_paso4.png)

![](/assets/g_embedder_paso5.png)

Este ID de seguimiento, es el que tendremos que poner en los plugins de Wordpress para que usen Google Analytics. Los resultados de estadísticas de acceso los podremos ver en la web de Google Analytics \(ejemplo de cómo ver los datos que recopila Google Analytics: [http://www.webempresa20.com/blog/tutorial-google-analytics-guia-seis-pasos-medir-social-media.html\](http://www.webempresa20.com/blog/tutorial-google-analytics-guia-seis-pasos-medir-social-media.html\)\).

Hay que ir a la web de Gestión de Google API:  [https://console.developers.google.com/](https://console.developers.google.com/) y ahí crear un nuevo proyecto y ponerle nombre \(por ejemplo Curso WP\):

![](/assets/paso6.png)

Rellenar los datos de configuración en Credenciales &gt; Pantalla de autorización de OAuth:

![](/assets/g_embedder_paso7.png)

En Credenciales &gt; Credenciales &gt; Crear credenciales, seleccionar “ID de cliente de OAuth”

![](/assets/g_embedder_paso8.png)

En la siguiente pantalla, elegir tipo de aplicación Web e introducir los datos de nuestro Wordpress:

![](/assets/g_embedder_paso9.png)

Y ya tenemos las claves de conexión:

![](/assets/g_embedder_paso10.png)

Estas claves también las podemos consultar en:

![](/assets/g_embedder_paso11.png)

También tenemos que asegurarnos de activar la API de Google Drive:

![](/assets/g_embedder_paso12.png)

Y Habilitarla en la siguiente pantalla:

![](/assets/g_embedder_paso13.png)

Y tendremos que rellenar los datos de ID de Cliente y de Secreto de Cliente en los ajustes del plugin Google Apps Login:

![](/assets/g_embedder_paso14.png)

**¡Ya podemos ir a una entrada e incrustar un documento de Google Drive!**

