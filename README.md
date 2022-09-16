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

Descarga los archivos que hay en https://github.com/miguelramosga/daclaes_chatbot.

Algunos de estos archivos son secundarios y, como tal, no aportan a la arquitectura del modelo. Los realmente importantes son ".rasa/cache", "actions", "data", "models", "tests", "config.yml", "credentials.yml", "domain.yml" y "endpoints.yml". 
Para descargarlo todo, 
