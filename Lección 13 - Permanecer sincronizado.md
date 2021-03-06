# Permanecer sincronizado con un repositorio remoto

Un **pull request** es una petición o solicitud al administrador (Maintainer) del repositorio original para incluir cambios en su proyecto sobre el cual hemos hecho un `Fork`.

 - Hacer Fork sobre el proyecto de [Axity](https://github.com/achamizoch/axity-collaboration-travel-plans)

 - Crear un `branch` con el nombre `include-<usuario>-destinations`.

 - Hacer al menos un `commit` en el branch que ha creado.

 - Hacer `push` sobre su proyecto asociado al Fork.

 - Ingrese a su cuenta de GitHub en el repositorio sobre el que realizó el Fork (no el original, el que se creó en su cuenta).

![img_13_git_request_01](images/img_13_git_request_01.png)

 - Dar clic sobre el botón "**New pull request**".

 - Del lado izquierdo seleccione el repositorio original y el branch sobre el cual se solicita aplicar los cambios.

 - Del lado derecho seleccione su repositorio (Fork) y el branch que creó previamente y sobre el que hizo los commits.

 - Dar clic sobre el botón "`Create pull request`".

 - Ingresar un título y una descripción del mensaje.

![img_13_git_request_02](images/img_13_git_request_02.png)

 - Dar clic sobre el botón "`Create pull request`".

## Obtener los cambios del repositorio original

 - Crear la conexión al repositorio original
```bash
$ git remote add upstream https://github.com/achamizoch/axity-collaboration-travel-plans.git
$ git remote -v
```

> Podemos renombrar las conexiones de la siguiente forma:
> 
> `$ git remote rename mine origin`
> `$ git remote rename source-repo upstream`
>

 - Obtener los cambios

```bash
$ git fetch upstream master
$ git log --oneline --graph --decorate --all
```

 - Hacer merge

```bash
# Asegurar que nos encontramos en el branch correcto para hacer el merge
$ git checkout master

# Hacer merge del branch del proyecto original a nuestro branch
$ git merge upstream/master

# Enviar los cambios del repositorio remoto a nuestro repositorio remoto
$ git push origin master
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYyMzg3NTU5MCwxODQwNzc5MTQ0LDMzOT
YwMjI1MSwtMTY1NDE1Mjk5MywxODY2NDY1MzQ0LC0xNTExOTAw
NDA4LDE5MDMzNjU3MzEsMTk1MTAxOTA4MF19
-->