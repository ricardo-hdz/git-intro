
Básicos de Git y Github
========

Crear un Repositorio
--------
Primero creamos un repositorio en Github haciendo click en donde el botón New en la página de repositorios de nuestro perfil en [Github](https://github.com/ricardo-hdz?tab=repositories).

Ahí se indicará el nombre del proyecto/repositorio (Project Name) y opcionalmente una descripción del mismo (Description) y un link a la web del proyecto (Homepage Url). También se puede indicar si el repositorio será público, siendo visible para todo el mundo, o bien privado, que solo será accesible para el usuario que lo crea y el o los contribuidores. 

Una vez creado el repositorio en Github se deberán realizar los siguientes pasos en nuestra computadora:

1. Crear el directorio (carpeta) en donde se alojará el repo. Para ello recomiendo crear una carpeta en nuestra carpeta de usuario (mac) / disco local c (windows) y alojar ahí todos los repos.

2. En línea de comandos (terminal/cmd) navegar hasta el repo. Deberemos llegar hasta el repositorio mediante la línea de comandos, usando el comando *cd*. Ej: 

3. Inicializar el repo de git. Una vez se llega al que será el directorio del repo se debe introducir lo siguiente para iniciar el repositorio en **git**.

`<git init>`

4. Añadir la dirección remota del repositorio de github. Se deberá indicar dónde estará alojado el repo. 

`<git remote add origin git@github.com:nombreusuario/nombrerepo.git>`


Clonar un Repositorio
--------

TBD

Comandos básicos de Git
========

1. Añadir uno o varios archivos a un commit.
2. Realizar un commit
3. Subir los cambios al repositorio mediante `push`
4. Revertir los cambios realizados por dicho commit.