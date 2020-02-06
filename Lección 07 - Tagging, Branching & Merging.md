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

![img_07_git_tag_atom](images/img_07_git_tag_atom.png)

> Se recomienda el uso de la opción -a ya que esta incluirá información adicional como:
> 
> - la persona que generó el tag
> - la fecha en que fue realizado
> -  
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwMjA4NjA4NjksLTE2NjA4MzA5MjUsLT
E5MzA1MDI0OCwtMTgxMTIxODU5OSwxODI1NTAzMTc1XX0=
-->