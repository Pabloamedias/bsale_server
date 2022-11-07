#Documentación para el server
La siguiente documentación corresponde a una postulación para el cargo de desarrollador Junior de Bsale

Setup:
Comenzamos dividiendo el projecto en dos partes. Una que hará de cliente y otra como un servidor REST.
#Esta parte corresponde al Servidor
-Ejecutamos git init para iniciar un repositorio
-Ejecutamos npm init -y para crear nuestro package.json
-Creamos un archivo .gitignore donde agregaremos la carpeta de node_modules
-Ejecutamos npm i express mysql2 morgan, que seran las librerías que utilizaremos del lado del backend

-Agregamos la línea "type" : "module" en nuestro package.json, de esta forma podremos importar las librerías en los archivos

-Ejecutamos npm i nodemon -D, (El parametro 

-D es para que la librería solo este en desarrollo y no en produccion) adicionalmente agregaremos "dev":"nodemon server/index.js" en nuestro package.json, de esta forma al ejecutar el comando el servidor se ejecutara con Nodemon, de esta forma no tendremos que reiniciar nosotros el server a cada cambio.

-Creamos un archivo config.js, donde guardaremos el puerto

-Creamos un archivo db.js donde guardaremos las configuraciones sobre la base de datos

-Creamos la carpeta de routes, que contendra index.routes.js, archivo donde inicialmente configuraremos las primeras rutas

-De momento en routes ejecutaremos una peticion muy sencilla, que usaremos para comprobar que la configuracion y la conexion a la bbdd esta funcionando de forma correcta.
