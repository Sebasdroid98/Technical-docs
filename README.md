# Technical-docs
Repositorio para indicar todo el proceso de instalación del conjunto de api, cliente y bd.

## Recomendaciones
 - [ ] Debes tener docker instalado en tu computador.
 - [ ] Asegurate de que docker está en ejecución.
 - [ ] Asegurate de usar las ramas "main" de cada repositorio.

## Descarga de recursos
 - [ ] Descarga este repositorio.
 - [ ] Accede a la carpeta "Technical-docs".
 - [ ] Descarga el repositorio "CLIENTE" desde "https://github.com/Sebasdroid98/Technical-frontend.git".
 - [ ] Renombra la carpeta "Technical-frontend" con el nombre "laravel_client".
 - [ ] Descarga el repositorio "API" desde "https://github.com/Sebasdroid98/Technical-backend.git".
 - [ ] Renombra la carpeta "Technical-backend" con el nombre "laravel_api".

## Estructura del proyecto
 - [ ] Technical-docs
 - [ ] _____laravel_client
 - [ ] __________>Dockerfile
 - [ ] __________>.env
 - [ ] _____laravel_api
 - [ ] __________>Dockerfile
 - [ ] __________>.env
 - [ ] _____docker-compose.yml


## Configuración de "laravel_client"
 - [ ] Accede a la carpeta "laravel_client".
 - [ ] Extrae el archivo "storage.zip".
 - [ ] Haz una copia del archivo ".env.example" y renombralo como ".env".
 - [ ] Ahora configura las siguiente variables:
 - [ ] APP_NAME=LaravelClient
 - [ ] APP_ENV=local
 - [ ] APP_KEY=base64:k6bcjjS5OwNSwULVxvDJsGgB+54TNNrjjjyX6QjTtGM=
 - [ ] APP_URL=laravel_client
 - [ ] APIREST_URL=laravel_api

## Configuración de "laravel_api"
 - [ ] Accede a la carpeta "laravel_api".
 - [ ] Extrae el archivo "storage.zip".
 - [ ] Haz una copia del archivo ".env.example" y renombralo como ".env".
 - [ ] Ahora configura las siguiente variables:
 - [ ] APP_NAME=LaravelApi
 - [ ] APP_ENV=local
 - [ ] APP_KEY=base64:0YL7WlfvvKjKdp4UWje/csAo/LQp/8HkRYFddwBZn5c=
 - [ ] APP_URL=laravel_api
 - [ ] DB_HOST=mysql
 - [ ] DB_PORT=3306
 - [ ] DB_DATABASE=laravel
 - [ ] DB_USERNAME=laravel
 - [ ] DB_PASSWORD=laravel

## Despliegue de los proyectos
 - [ ] Regresa a la carpeta "technical-docs".
 - [ ] Abre una terminal y ejecuta el comando "docker-compose up -d --build".
 - [ ] Después de que terminen de configurarse los proyectos, los enlaces quedaran asignados asi:
 - [ ] CLIENTE = "http://localhost:8080/public/".
 - [ ] API     = "http://localhost:8081/public/".
 - [ ] Para ejecutar las migraciones accede a la la API (http://localhost:8081/public/) y accede a la ruta "run-migrations" o presiona en el enlace que dice "Ejecutar-migraciones".

# Funcionalidades

## En "laravel_client"
 - [ ] Registro de libros.
 - [ ] Visualización del listado de libros.
 - [ ] Edición de un libro por su id.
 - [ ] Eliminación de un libro por su id.

## En "laravel_api" endpoints
 - [ ] GET "api/v1/books"___________Para obtener todos los libros.
 - [ ] GET "api/v1/books/{id}"______Para obtener un libro por su id.
 - [ ] POST "api/v1/books"__________Para registrar un libro.
 - [ ] PUT "api/v1/books/{id}"______Para actualizar un libro.
 - [ ] DELETE "api/v1/books/{id}"___Para eliminar un libro por su id.