Este proyecto es una prueba de docker.

--------------------------------------

Como ejecutar: Introduce estos comandos:
````
docker build -t mi-app:1.0 .
docker run --rm -p 8000:8000 mi-app:1.0
````
--------------------------------------
Entorno de desarrollo: Ejemplo para comprobar la version de Python
````
docker compose build dev
docker compose run --rm -T dev python --version
````
--------------------------------------
Tests:
````
docker compose run --rm -T dev pytest
````
--------------------------------------
Formateo:
````
docker compose run --rm -T dev black .
````
--------------------------------------
Precommit: Comprueba que el codigo esta bien formateado y si no no te deja hacer el commit.