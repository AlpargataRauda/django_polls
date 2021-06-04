# Bienvenido a la libreria de encuestas de django-polls
## Para trabajar con este repositorio

1. Descarga el codigo con el siguiente comando (usar la documentación https si no se tienen las claves ssh):
```
git clone git@github.com:AlpargataRauda/django_polls.git 
cd django_polls/ 
```
2. Deberemos entrar en la carpeta django-polls con el comando: 
```
 cd django_polls/
 ```
3. Y crear un entorno virtual con el comando: 
```
python3 -m venv .venv
```
4. Activar el entorno virtual con el comando: 
```
source .venv/bin/activate
```
5. Instalar las librerias necesarias que se encuentran en el fichero 'requirements.txt' con el comando:
```
pip install -r requirements.txt
```
6. Hacer las migraciones con el comando:
```
python manage.py migrate
```
7. Cargar los datos iniciales con:
```
python manage.py loaddata fixtures/polls_data.json
```
8. Configurar el localhost con una ip permitida para django. Para ello deberemos editar el fichero 'django_polls/settings.py'. Despues añadimos aqui la ip local a la variable 'ALLOWED_HOSTS' (en la linea 28), de forma que quede así:
```
ALLOWED_HOSTS = ['192.168.33.10', '127.0.0.1']
```
9. El ultimo paso es arrancar el servidor con:
```
python manage.py runserver
```

## Para subir cosas a github

1. Guarda los commits en la pestaña Source Control, debemos notificar lo que hemos hecho

2. Por último envía la carpeta de django_polls en el repositorio con:
```
git push (nombre del repositorio)
```