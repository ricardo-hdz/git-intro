
Básicos de Git y Github
========

Crear un Repositorio mediante Git Clone
--------
Primero creamos un repositorio en Github haciendo click en donde el botón New en la página de repositorios de nuestro perfil en [Github](https://github.com/ricardo-hdz?tab=repositories).

Ahí se indicará el nombre del proyecto/repositorio (Project Name) y opcionalmente una descripción del mismo (Description) y un link a la web del proyecto (Homepage Url). También se puede indicar si el repositorio será público, siendo visible para todo el mundo, o bien privado, que solo será accesible para el usuario que lo crea y el o los contribuidores. 

Una vez creado el repositorio en Github se deberán realizar los siguientes pasos en nuestra computadora:

1. En la terminal, ir a la carpeta en donde se alojara el repositorio

2. Ejecutar, `git clone <direccion_repositorio>` donde direccion_repositorio es las direccion del repositorio en Github.


Crear un Repositorio localmente
--------

1. Crear el directorio (carpeta) en donde se alojará el repositorio.

2. En la linea de comandos ir hasta el directprio creado. Por ejemplo, `cd /directorio/de/proyecto`

3. Inicializar el repositorio de git con el siguiente comando:

`<git init>`

4. Crear el repositorio en Github. Después añadir la dirección remota del repositorio utilizando el siguiente comandoÑ

`<git remote add origin git@github.com:nombreusuario/nombrerepo.git>`


Clonar un Repositorio
--------

```
git clone <repositorio>
```

Comandos básicos de Git
========

```
git commit - Sirve para guardar los cambios a un archivo en la historia de Git
```

1. Añadir uno o varios archivos a un commit.
2. Realizar un commit
3. Subir los cambios al repositorio mediante `push`
4. Revertir los cambios realizados por dicho commit.