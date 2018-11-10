Git & Github: Introducción
========
El objetivo de esta repositorio y guía es ofrecer una introducción básica al control de versiones de Git y la herramienta de Github para crear repositorios y compartir código. La guía está diseñada para principiantes, especialmente pensada para niños y adolescentes que comienzan a aprender ty desarrollar conceptos de programación.

GIT
--------
Git es un sistema de control de versiones para rastrear cambios en archivos de computadora y coordinar el trabajo en esos archivos entre varias personas. Se utiliza principalmente para la administración de código fuente en el desarrollo de software, pero se puede usar para realizar un seguimiento de los cambios en cualquier conjunto de archivos. (Wikipedia, 2018)

Git usa cadenas de 40 caracteres comúnmente llamadas `SHA` para identificar los cambios  realizados. Por ejemplo, la siguiente cadena representa un cambio realizado a un archivo o conjunto de archivos:

```
74be3c2b93c8267de64e6dfde8658d31d7d2fe6c
```

### Objetos de Git
Hay 4 tipos de objetos en git:

1. `blob`: es un conjunto de datos que generalmente se interpreta como un archivo.

2. `tree`: es un directoro que como su nombre en español lo indica es un árbol de archivos y directprios. 

3. `commit`: de forma práctica, un commit es un cambio o modificación a un archivo o conjunto de archivos que se guarda como referencia de cambio a un árbol (`tree`)

4. `tag`: es un identificador que puede ser utilizado para identificar un cambio, como su nombre en español lo indicada (etiqueta)


[Github](http://github.com/)
--------
Github es una plataforma de desarrollo colaborativo de software para almacenar proyectos en línea utilizando el sistema de control de versiones Git. El código se puede almacena en repositorios (proyectos) públicos o privados.

Github también ofrece funcionalidades extendidas como `forks`, `issues`, `pull requests`, `diffs`. Estos conceptos se veran más adelante en el curso.

Actividad 1 - Tutorial de Introducción a Github

La primera actividad para conocer Github es completar el siguiente ejercicio en la página de Github. El ejercicio te introducirá a los conceptos básicos de la herramienta, así como a su interfase y funcionalidades más utilizadas.

El ejercicio comienza en el paso "Introducción a Github" y termina en "Has completado el GitHub Flow".

El tutorial se puede acceder a través de la siguiente liga: https://services.github.com/on-demand/intro-to-github/es/

Una vez terminado el tutorial podemos pasar a la siguiente sección para instalar git y github en nuestras máquinas.

Instalar Git y Github
========
### Instalar Git

Instalar Git utilizando los siguientes enlaces dependendiendo del sistema operativo:

Mac OS X -> [Git](http://sourceforge.net/projects/git-osx-installer/)

Windows -> [Git](https://git-scm.com/download/win)

Para instalar Git basta con descargar el software de instalación y seguir las instrucciones.

Nota: Git es un programa que se instala en la computadora y que utilzaremos mayormente a través de la línea de comandos o terminal.

### Instalar Github

Para instalar Github utilizaremos las cuenta que creamos en el tutorial.

Después de instalar Git de acuerdo a las instrucciones mencionadas arriba debemos proceder a configurar Git y Github para que puedan comunicarse entre sí, es decir, poder realizar cambios en nuestras computadoras y enviarlos a repositorios (proyectos) en Github.

Crear Clave SSH 
--------
>Las claves SSH se usan para establecer una conexión segura entre nuestra computadora y Github.

Para crear la clave SSH se siguen los siguientes pasos en la terminal o consola de comandos (cada paso se debe ejecutar en la consola):

`ssh-keygen -t rsa -C "your_email@youremail.com"`
(sustituir "your_email@youremail.com" por el email que utilizaste para crear tu cuenta de Github).

Después de ejecutar este comando, la terminal devolverá lo siguiente: 

`Generating public/private rsa key pair. Enter file in which to save the key. C/Users/your_user_directory/.ssh/id_rsa)`

Aquí debemos presionar `Enter` en Windoes o `return` en Mac. Después de esto la computadora guardará la clave ssh en el directorio .ssh dentro de nuestra carpeta de usuario.

A continuación la terminal desplegará: `Enter passphrase (empty for no passphrase)`. Aquí no hay por qué indicar nada, solo presionar `Enter` o `return`, y volverá a pedir una fras pero solo volvemos a presionar `Enter` una vez más.

Al final, la terminal desplegará algo similar a lo siguiente:

```
Your identification has been saved in /Users/your_user_directory/.ssh/id_rsa. 
Your public key has been saved in /Users/your_user_directory/.ssh/id_rsa.pub
```

Aquí debemos copiar la clave ssh. Para ello debemos realizar lo siguiente dependiento del sistema operativo:

Mac: `pbcopy < ~/.ssh/id_rsa.pub`

Windows: abrir el programa `Git Extensions` que se instalo cuando instalamos Git, ir a Help (Ayuda), Show Key (Mostrar Clave) y entonces presionar Copy to Clipboard (Copiar al portapales) para copiar la clave ssh al portapeles.

Configurar Github con la clave SSH 
--------

Ir a [Github](https://github.com/account/ssh) y hacer click en el botón "New SSH key". Agregar lo siguiente:

Title: un título que identifque a la clave SSH, puede ser cualquier nombre, por ejemplo "Mi Clave".
Key: aquí hay que pegar la clave que copiamos en el paso anterior, para ello basta con hacer Control+V (o Cmd+V en Mac).

Comprobar la configuración
--------

Para comprobar la configuaración ejecutamos el siguiente comando en la terminal:

`ssh -T git@github.com`

Después de esto la terminal desplegará algo similar a lo siguiente:

`The authenticity of host ´github.com (123.123.123.123) can't be established. RSa key fingerprint is....... Are you sure you want to continue connecting (yes/no)`

Aquí solamente hay que escribir `yes` en la terminal y presionar `Enter`.

A continuación la terminal mostrará el siguiente mensaje:

`Hi 'username'! You've succesfully authenticated, ....`

Después de esto nuestra computadora esta lista para comunicarse con Github.

Por último, hay que configurar alguna información Git que permitirá identificar nuestra cuenta y cambios.

Configuración de Git
--------
Para configurar nuestro nombre y email de Git basta con ejecutar los siguientes comandos en la terminal (recuerda sustituir "Firstname Lastname" con tu nombre y apellido y "your_email@youremail.com" con el email que utilizaste para crear tu cuenta de Github.

`git config --global user.name "Firstname Lastname"`

`git config --global user.email "your_email@youremail.com"`

Resumen
--------
En esta primerar sesión terminamos la introducción básica a Git y Github, realizamos nuetsro primer tutorial en línea para aprender Github y configuramos nuestras cuentas para que nuestra computadora se pueda comunicar con Github.

En la siguiente clase veremos cómo crear y clonar un repositorio (proyecto), así como realizar cambios a los archivos del repositorio, revertirlos y subirlos al repositorio remoto en Github.