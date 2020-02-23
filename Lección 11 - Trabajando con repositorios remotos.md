# Trabajando con repositorios remotos

En esta lección conoceremos como trabajar con repositorios remotos de GitHub y como obtener y enviar cambios a un repositorio remoto.

## ¿Qué es GitHub?

Git es un sistema de control de versiones distribuido, lo que significa que no hay un depósito principal de información. Cada desarrollador tiene una copia del repositorio. Por lo tanto, puede tener una copia del repositorio (que incluye los commits publicados y el historial de versiones) y otros usuarios también pueden tener una copia del mismo repositorio. Cada repositorio tiene exactamente la misma información que los otros, no hay un repositorio que sea el principal.

![img_11_git_remote_01](images/img_11_git_remote_01.png)

La forma en que podemos interactuar y controlar un repositorio remoto es a través del comando remoto de Git:

```bash
$ git remote
```

[![Git remote](http://img.youtube.com/vi/414f0ukhOTY/0.jpg)](http://www.youtube.com/watch?v=414f0ukhOTY "Git remote")

## El comando Git Remote

### Práctica 11 - Git Remote

Para crear un repositorio remoto debemos ejecutar los siguientes comandos:

 1. Crear el directorio `~/my-travel-plans`
 2. Inicializar el directorio usando el comando `git init`
 3. Crear el archivo `README.md`
 4. Crear el archivo `index.html`
 5. Crear el archivo `app.cs`

#### Contenido de README.md

```
# Travel Destinations

A simple app to keep track of destinations I'd like to visit.

```
```bash
$ cd ~/axity-git-course
```
`my-travel-plans`
<!--stackedit_data:
eyJoaXN0b3J5IjpbODU4MjI0NTgzLC0xNTQ0MDM1NzA3LDE3MT
I0MjM5NDEsMTM2NDg3OTE4Nyw3MDY4MDA5NzEsMTM3Njg0ODA5
NCwtNTIyNzc5OTA2LDUzNDA5ODAxN119
-->