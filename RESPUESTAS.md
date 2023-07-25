# Respuestas

Indica tu nombre a continuación: 

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 1

¿Cuál es la diferencia entre los archivos con el verbo `Create` con los archivos con el verbo `Add`?
R.- El verbo Create se ocupa para crear tablas.
    el verbo add se ocupa para agregar registros a las tablas ya creadas.

¿Cómo se llama el servicio que se declara en el archivo `docker-compose.yml`?
R.- flyway

¿Cuál es el comando que se ejecuta en el servicio declarado?
R.- -locations=filesystem:/flyway/sql -connectRetries=60 migrate

## ETAPA 2

¿Qué pasa si cambias el nombre del servicio de `postgres` a `db`? ¿Qué otros cambios tendrías que hacer?
R.- Se debe cambiar el .env la variable POSTGRES_SERVER ==> db
    En el docker-compose.yml se debe modificar la dependencia del servicio flyway  postgres ==> db

## ETAPA 3
¿Qué te llama la atención?

¿Cómo se relacionan el archivo `docker-compose.yml` y el archivo `movies-api/Dockerfile`?
R.- que el docker-compose.yml levanta un contenedor utilizando el Dockerfile dentro de la carpeta movies-api

¿Qué crees que hace el atributo `context` debajo de `build` (está en la linea 6 del archivo `docker-compose.yml`)?
R.- Agrega otra raiz o path a donde debe existir un dockerfile para generar una contenedor.

...