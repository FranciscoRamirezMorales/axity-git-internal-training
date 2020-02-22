# Merging

En esta lección veremos los dos principales tipos de **Merge**:

 - ¿Qué es merge?
 - Fast-forward merge
 - Regular merge

## ¿Qué es merge?
Recordemos que el propósito de un branch (por ejemplo `sidebar`) es que nos permite realizar cambios que no afectan al branch `master`. Una vez que realizamos cambios en el branch `sidebar` podemos decidir que esos cambios no aplicarán, eliminarlos o mantenerlos y posteriormente combinarlos con otra rama.

**A la acción de combinar dos branches se le denomina `merge`.**
ara entender como funciona el comando merge, podemos ver el siguiente video:

**Video >>> (dar clic)**

[![Git merge](http://img.youtube.com/vi/gQiWicrreJg/0.jpg)](http://www.youtube.com/watch?v=gQiWicrreJg "Git merge")

## Fast-forward merge
Este es el mas simple de los merge, ya que como se puede observar en el video, el apuntador `HEAD` del branch `master` es movido al commit más `adelantado`.

> Recordemos en en la práctica anterior creamos un branch llamado `footer` basado en el branch `master`. Sobre `footer` (el cual en ese momento es una copia de `master`) se agregaron los enlaces de redes sociales. Por lo que footer tiene el commit más `adelantado`.

Tomando como base el resultado de la práctica anterior, para realizar un fast-forward merge ejecutamos el siguiente comando:

```bash
$ git merge footer
```

## Regular merge
Este tipo de merge es el más común ya que implica combinar dos branches cuyas rutas son diferentes. 

> Esta acción implica realizar un `commit`, ya que la propia acción de este tipo de merge implica cambios sobre los archivos.

Para realizar un regular merge ejecutamos el siguiente comando:

```bash
$ git merge sidebar
```

> Recordemos en en la práctica anterior creamos un branch llamado `sidebar` basado en el branch `master`. Tanto en master como en sidebar 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU5MjYyOTQ0MCwyMTI5MDU4NjQxLC0zOD
Q2NDIyMzEsNDc0MTQ3OTUyXX0=
-->