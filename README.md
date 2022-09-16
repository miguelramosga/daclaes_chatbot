# DACLA-ES Toolbot
## Instrucciones para poder mantener conversaciones con el asistente conversacional
### Primer paso: 

Se debe instalar Rasa en el ordenador siguiendo las instrucciones que se proporcionan en el siguiente enlace: https://rasa.com/docs/rasa/installation/.

Desde el principio, se va a necesitar disponer de Python, por lo que lo mejor es tener Anaconda. Desde la línea de comandos de Anaconda, también se tendrá que crear un entorno, activarlo e instalar Rasa Open Source. Es decir, se trataría de seguir los mismos pasos explicados en el enlace, pero aplicados a Anaconda. Se tendrá que ir insertando esto: 
  - python --version 
  - conda create -n chatbot python=3.8
  - conda activate chatbot
  - python -m pip uninstall -U pip
  - python -m ensurepip
  - python -m pip install -U pip
  - pip install rasa
  - rasa -h
  - rasa init


### Segundo paso:

Se tienen que descargar los archivos que hay en https://github.com/miguelramosga/daclaes_chatbot.

Algunos de estos archivos son secundarios y, como tal, no aportan a la arquitectura del modelo. Los realmente importantes son ".rasa/cache", "actions", "data", "models", "tests", "config.yml", "credentials.yml", "domain.yml" y "endpoints.yml". 

Para descargarlo todo, es necesario tener Git instalado en el ordenador (Git Bash), por lo que, si no se tiene, se debe proceder a su descarga. Una vez hecho esto, lo mejor es crear una carpeta previamente en local para que, ahí, se haga clic derecho y se seleccione la opción "Git Bash here". Eso abrirá la terminal correspondiente, donde ya es posible descargar lo mencionado. 

Para ello, se debe escribir lo siguiente: "git clone https://github.com/miguelramosga/daclaes_chatbot.git", lo que permite que la descarga de los archivos comience directamente. Una vez se tenga descargado, ya se puede trabajar con el proyecto o, en este caso, visualizarlo en detalle e interactuar con el chatbot. 


### Tercer paso: 

Se debe abrir el proyecto con Rasa. 

Para conseguir ejecutar el proyecto con Python, es preciso volver a la terminal de Anaconda. Aquí pueden distinguirse dos fases distintas: en el caso de que la terminal mencionada se tenga abierta y se haya procedido de la manera que se ha descrito en el paso uno, se puede pasar directamente a la segunda fase. 

#### Fase 1: 
Si se tiene el proyecto descargado, pero se ha cerrado lo realizado en el paso uno, es necesario volver a activar el entorno que se ha creado en dicho paso. Para ello, hay que escribir "conda activate chatbot" en la línea de comando de Anaconda. 

#### Fase 2: 
Lo siguiente que se debe hacer es ir a la ubicación donde se ha puesto lo descargado desde GitHub, que será la carpeta que se ha creado en el paso dos para guardarlo ahí. La instrucción que se debe dar es esta: "cd" + la ruta de la carpeta en cuestión; por ejemplo, "cd C:\User\miguelramosga\Documentos\DACLAES". 

### Cuarto paso:

Ejecutar instrucciones de Rasa. 

Una vez se llega a este punto, ya pueden ejecutarse las instrucciones de Rasa. La primera que debe llevarse a cabo es "rasa train", pues eso permitirá que todo el modelo se entrene de acuerdo a cómo esta diseñado. La siguiente ya sería "rasa shell", lo que conduce a poder interactuar con el chatbot y, finalmente, llevar a cabo una conversación. 

En el caso de que esto dé problemas al usuario, una segunda opción para poder interactuar con DACLA-ES Toolbot es escribir la siguiente instrucción: "rasa run --model daclaes_chatbot".


