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
    
y posteriormente ejecutar el comando:

    # git status

```json
    On branch master

    Initial commit

    nothing to commit (create/copy files and use "git add" to track)
```

### Crear un archivo HTML

Crear un archivo `index.html` 

    # touch index.html

Dentro del archivo `index.html` ingresar el siguiente código:

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

> Podemos ver que en código hace referencia a un archivo CSS  y JavaScript.

Crear el directorio `css` y dentro de él crear el archivo `app.css`
Crear el directorio `js` y dentro de él crear el archivo `app.js`

```bash
$ mkdir css
$ mkdir js
$ touch css/app.css
$ touch js/app.js
```




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4OTg5ODQ3MjIsLTU4MzA4MDYyNCwxNz
E4MjM3MjgxLDEzMjU3NDYzNzQsMTU2MjQzNTI3OSwxNzUwMjA5
NTQ2LDQyMTA0MzY2LDIwNDAyMjg5NjksLTE3NTg5ODQ3MjQsMT
MyNjk0Njc2NywxODE1MTIxNzgwLDQxNjM1ODA2M119
-->