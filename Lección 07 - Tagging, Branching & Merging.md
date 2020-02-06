## Tagging, Branching & Merging

En esta lección veremos como:

 - Vistazo general
 - Crear Tag's
 - Crear Branches
 - Cambiar entre Branches
 - Realizar un Merge entre Branches
 - Tratar posibles problemas al hacer Merge

## Vistazo general
En esta lección veremos los siguientes comandos:
 - `git tag` para agregar etiquetas a commits específicos; un tag es una etiqueta que nos permite identificar un punto del desarrollo, por ejemplo, una versión beta. 
 - `git branch` para generar ramas las cuales pueden estar asociadas a diferentes características de un proyecto que se desarrollan en paralelo.
 - `git checkout` el cual nos permite movernos entre los diferentes  branches y tag's
 - `git merge` para combinar los cambios realizados en diferentes branches de forma automática

**Video >>> (dar clic)**

[![Git Tag](http://img.youtube.com/vi/D4VdXT72ASE/0.jpg)](http://www.youtube.com/watch?v=D4VdXT72ASE "Git Tag")

## Cear un Tag

Continuando con nuestro repositorio `new-git-project` crearemos un tag con el siguiente comando:

```bash
$ git tag -a v1.0
```
Esto abrirá el editor por defecto para poder generar un mensaje para el tag, en este caso ingresaremos el mensaje `Ready for content`.

![img_git__02](images/img_06_git_status_02.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA0MzU5OTU2NCwtMTY2MDgzMDkyNSwtMT
kzMDUwMjQ4LC0xODExMjE4NTk5LDE4MjU1MDMxNzVdfQ==
-->