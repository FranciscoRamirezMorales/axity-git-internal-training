# Agregando commits al repositorio

En esta lección veremos como:

 - Empezar a utilizar nuestro repositorio
 - Aprovechar el poder del comando `git status`
 - Agregar commits
 - Agregar mensaje a un commit
 - Ver cambios realizados antes de un commit
 - Omitir archivos en Git

## Empezar a utilizar nuestro repositorio

Antes de empezar a trabajar en nuestro repositorio debemos movernos al directorio `new-git-project` 

    # cd cd ~/axity-git-course/new-git-project/
    
Posteriormente ejecutar el comando:

    # git status

```json
    On branch master

    Initial commit

    nothing to commit (create/copy files and use "git add" to track)
```

### Crear un archivo HTML

Crear un archivo `index.html` 

    # touch index.html

Dentro del archivo `index.html` debemos incluir el siguiente código:

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>Blog Project</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <link rel="stylesheet" href="css/app.css">
</head>
<body>

    <script src="js/app.js"></script>
</body>
</html>
```

> Podemos ver que en código hace referencia a un archivo CSS  y otro  de JavaScript.

Crear el directorio `css` y dentro de él crear el archivo `app.css`
Crear el directorio `js` y dentro de él crear el archivo `app.js`

```batch
$ mkdir css
$ mkdir js
$ touch css/app.css
$ touch js/app.js
```

Revisar el estatus del repositorio:

```batch
$ git status
```
```
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	css/
	index.html
	js/

nothing added to commit but untracked files present (use "git add" to track)
```
#### ¿Qué significa esto?

![img_work_to_index](images/img_work_to_index.gif)

Para agregar el archivo `index.html` al Staging Index, debemos ejecutar el comando:

    # git add index.html

Revisamos nuevamente el estatus del repositorio:

    # git status

Para mover el resto de los archivos al Staging Index, ejecutamos el siguiente comando:

```bash
$ git add css/app.css js/app.js

# otra opción sería:
$ git add .
```

Volvemos a revisar el estatus del repositorio:

    # git status

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM0ODY3NTQzOSwtNzQxODQ4Njg1LC03ND
E4NDg2ODUsLTEwNzc5ODgxMTksMTM1MTA2NjY1MywtMTgwNDYy
NzQ0LC0xODIyMTg0NzI0LC0xNzg0NjY1MTQ3LC0xODk4OTg0Nz
IyLC01ODMwODA2MjQsMTcxODIzNzI4MSwxMzI1NzQ2Mzc0LDE1
NjI0MzUyNzksMTc1MDIwOTU0Niw0MjEwNDM2NiwyMDQwMjI4OT
Y5LC0xNzU4OTg0NzI0LDEzMjY5NDY3NjcsMTgxNTEyMTc4MCw0
MTYzNTgwNjNdfQ==
-->