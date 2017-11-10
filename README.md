## Configurar Settings para entornos (pre-producción y produccion en Django).

1. Donde tenemos nuestro archivo settings crear una carpeta settings.
2. Dentro de la carpeta settings, crear archivo __init__.py
3. Crear tres archivos base.py local.py produccion.py
4. Separar las configuraciones, atendiendo a las necesidades de cada entorno.
5. Ahora a tener en cuenta, siempre, hay que indicar la ruta para ejecutar las instrucciones manage.py, 

**Ejemplos:**

_Ejemplo 1_

Arrancar servidor python manage.py runserver --settings=curso.settings.local
Es decir indicamos donde tenemos nuestro archivo de configuraciones a utilizar

_Ejemplo 2 _
Arrancar servidor python manage.py runserver 0.0.0.0 --settings=curso.settings.local
Volvemos a indicar la ruta de nuestro archivo settings y arrancamos el servidor de forma que podamos hacer pruebas con la ip del equpipo.

_Ejemplo 3 _
Realizar operaciones con la base de datos:
python manage.py makemigrations --settings=curso.settings.local
python manage.py migrate --settings=curso.settings.local
python manage.py createsuperuser  --settings=curso.settings.local



