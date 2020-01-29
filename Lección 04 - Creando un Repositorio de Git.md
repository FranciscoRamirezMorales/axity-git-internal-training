# Creando un Repositorio de Git

Antes de empezar a utilizar Git, es necesario que exista un repositorio.

Si recordamos:

> Un **repositorio** - es un directorio que contiene un proyecto, así como algunos archivos internos para la gestión y administración del propio proyecto de Git.

## Crear directorio

El primer paso es crear un directorio de archivos. Para esto se deben ejecutar las siguientes líneas:

    # cd ~
    # mkdir axity-git-course
    # cd axity-git-course
    # mkdir new-git-project
    # cd new-git-project

Otra forma de hacerlo es ejecutando la siguiente línea:

    # cd ~
    # mkdir -p axity-git-course/new-git-project && cd $_

## Inicializando un Repositorio

Inicializar un proyecto es una de las actividades más simples, basta con ejecutar la siguiente línea:

    # git ini

Al ejecutar el comando git init se generan todos los directorios y archivos necesarios que Git usará para mantener el control de versiones de todo.

![img_git_repo](images/img_git_repo.png)

Aquí hay una breve sinopsis de cada uno de los archivos/directorios en el directorio **.git**:
  

 - **config**: donde se guardan todos los ajustes de configuración específicos del proyecto, incluida la configuración inicial (nombre, e-mail). Ver la siguiente documentación para mayor detalle: [Git Book](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)
  
 - **description**: este archivo solo lo usa el programa GitWeb, por lo que puede ser ignorado
  
 - **hooks**: aquí es donde se pueden colocar scripts ya sea del lado del cliente o del servidor y que se pueden usar para conectar los diferentes eventos del ciclo de vida de Git
  
 - **info**: contiene el archivo de exclusión global
  
 - **objects**: almacena todos los commits realizados
  
 - **refs**: este directorio contiene punteros para confirmar (básicamente las "ramas" y las "etiquetas")

Enviar comentarios

Historial

Guardadas

[](https://translate.google.com/community?source=mfooter)

Comunidad
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcyNDkwMTc5NiwxNzg2NDY5ODAxLDE2ND
Y4NzE0MzYsNDE3MzE2ODFdfQ==
-->