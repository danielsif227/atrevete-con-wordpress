## Embeber archivos de Google Drive en Wordpress

#### USO

**Google Apps Login + Google Drive Embedder**: Con la combinación de estos plugins se podrá añadir archivos de Google Drive embebidos en las entradas del Wordpress:

![](/assets/g_embedder_uso.png)

#### CONFIGURACIÓN

Es necesario instalar, activar y configurar el plugin **Google Apps Login**: En el `Wordpress > Escritorio > Ajustes > Google Apps Login`, necesitamos obtener un ID y un Secreto de cliente.

Para ello, hay que ir a la web de Gestión de Google API:  [https://console.developers.google.com/](https://console.developers.google.com/) y ahí crear un nuevo proyecto y ponerle nombre \(por ejemplo _Curso WP_\):

![](/assets/google-api-proyecto.png)

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

