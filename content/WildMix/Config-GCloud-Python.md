# Configurando el entorno de desarrollo de Google Cloud - Python

1. Descargar el DSK de [AppEngine para Python](https://cloud.google.com/appengine/downloads)

2. Descomprimirlo

3. Abrir la consola, ir a la carpeta donde lo descomprimimos, ejecutar el comando ``./install.sh``

4. Reiniciar la consola (Abri�ndola nuevamente)

5. Generar una serie de archivos para que GCloud sepa c�mo correrlo

   _app.yml_ : Qu� ambiente vamos a necesitar, y a d�nde va a enviar el tr�fico.

   _appengine_config.py_: D�nde se encuentran las librer�as que instalamos con pip, google no corre ese comando, por lo que debemos subir las librer�as. Este archivo lleva por c�digo:

   ```py
    from google.appengine.ext import vendor
    vendor.add("lib") # Donde lib es la carpeta donde guardaremos las librer�as.
   ```

6. Crear un folder _/lib_ para guardar las librer�as (en el proyecto actual)

7. Abrir consola, movernos a nuestro folder del proyecto actual

8. Iniciar ambiente virtual: ``source venv/bin/activate``

9. Instalar requirements.txt en este folder ``pip install -r requirements.txt -t lib``

   ``-t lib`` significa que ese es el directorio destino donde las instalar�

10. Indicar en app.yaml

    ```yaml
      service: default
      runtime: python27 # Ambiente a utilizar (python 27 es Python 2.7)
      api_version: 1
      threadsafe: yes
    
          # Hacia d�nde tiene qu� mandar el tr�fico  
          handlers:
          - url: .*
            script: main.app # m�dulo main, variable app, en el main.py, en la variable app = Flask(name)
            secure: always
    ```

11. Correr el servidor local ``dev_appserver.py .``, poner un punto al final, significa que el archivo yaml est� en el mismo directorio

12. Subir el archivo a internet

    12.1. Entrar a console.cloud.google.com

    12.2. Crear un Proyecto

    12.3. Ir al men� App Engine (barra lateral izq)

    12.4. Escoger el lenguaje de nuestra aplicaci�n.

    12.5. Autenticarnos con Google desde la consola ``gcloud auth login``

13. Hacer deploy de la aplicaci�n ``gcloud app deploy --project <projectid>``

14. Despu�s de eso nos dir� la URL donde se deploy�

