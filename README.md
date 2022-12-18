## Instalar Anaconda 
La forma más simple de ejecutar el proyecto es instalando [Anaconda](https://www.anaconda.com/distribution/).

Con Anaconda instalado de manera correcta, navegar hasta el directorio del proyecto
y ejecutar: 
```
# navegar hasta el directorio del proyecto
cd platzi-mongo
# crear un nuevo ambiente
conda create --name platzi-mongo
# activar el ambiente 
conda activate platzi-mongo
# para desactivar el ambiente
conda deactivate
```
## Instalar dependenias del proyecto
Con el ambiente activado, instalar las dependencias:
```
conda install --file requirements.txt
```
## Variables de entorno necesarias para ejecutar el proyecto
Asegurate de reemplazar el valor de PLATZI_DB_URI por la URI de tu cluster en MongoDB Atlas
```
set FLASK_APP=platzi-api
set FLASK_ENV=development 
set PLATZI_DB_URI="MONGO-URI"
```
## Iniciar el servidor de platzi-mongo
```
flask run
```
