# Plataforma educativa

Una plataforma robusta que te permite gestionar alumnos, sus grados y grupos, logros, crear clases y tener acciones en tiempo real, perfecto para cursos en linea en vivo o para escuelas, se compone de una api en laravel, un front en react y un servidor node para acciones en tiempo real y notificaciones.

##Instalacion

Para poder instalar es necesario tener conocimientos de laravel (usar composer install), tener conocimientos de react (usar npm run build) y tener conocimientos de node (usar node server.js).

**Api-laravel**, debes descomprimir el archivo api-laravel.php y dirigirte a la carpeta, como mencione es necesario tener conocimientos de laravel para crear las migraciones y los seeders, antes de todo asegurate de tener una base de datos postgree y configurala en tu archivo .env.

  - Dentro de api-laravel en terminal ejecutar "composer install"
  - Dentro de api-laravel en terminal ejecutar "php artisan migrate --seed"
  - Correr el servidor usando "php artisan serve" o meterlo en la carpeta de tu servidor.

**Front-react**, debes descomprimir el archivo front-react.zip y dirigirte a la carpeta, es necesario tener node y npm instalados.

- En el archivo public/index.html buscar socket.io/socket.io.js y cambiarlo por la ruta del servidor node (mas adelante explicare de donde sale).
- En el archivo public/index.html buscar window.api = y cambiar su valor por la ruta de api-laravel, si ya esta en un dominio hay que adjuntar "/api/" ejemplo: window.api = "http://api-laravel.mi-dominio.com/api/"
- En el archivo public/index.html buscar window.storage = y cambiar su valor por la ruta de api-laravel, si ya esta en un dominio hay que adjuntar "/storage/" ejemplo: window.storage = "http://api-laravel.mi-dominio.com/storage/"

**Servidor node**, dentro de api-laravel/require esta el archivo server.js y package.json puedes moverlo de carpeta o dejarlo ahi, debes ejecutar "npm install" dentro de esa carpeta.
- Tener redis instalado y ejecutandose (sirve para las acciones en tiempo real y notificaciones)

##Alumno
Inicio de sesion
![Inicio de sesion](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-1.PNG)

Bienvenida
![Bienvenida](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-2.PNG)

Logros
![Logros](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-3.PNG)

Cursos
![Cursos](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-4.PNG)

Lecciones
![Lecciones](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-5.PNG)

Leccion
![Leccion](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-6.PNG)

Logro
![Logro](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/Captura.PNG)

##Profesor
Dashboard
![Dashboard](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-10.PNG)

Cursos
![Cursos](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-11.PNG)
Añadir leccion
![Leccion](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-9.PNG)

Iniciar clase
![iniciar clase](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-12.PNG)
##Administrador
Cursos
![Cursos](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-7.PNG)

Alumnos
![Alumnos](https://raw.githubusercontent.com/le-vendetta/plataforma-educativa/master/imagenes/plataforma-8.PNG)


Sientete libre de usar el codigo como gustes, y si haces algo importante no olvides darme el credito :).