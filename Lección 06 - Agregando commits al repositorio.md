# Agregando commits al repositorio

En esta lección veremos como:

 - Empezar a utilizar nuestro repositorio
 - Agregar commits
 - Agregar mensaje a un commit
 - Ver cambios realizados antes de un commit
 - Omitir archivos en Git

## Empezar a utilizar nuestro repositorio

Antes de empezar a trabajar en nuestro repositorio debemos movernos al directorio `new-git-project` 

```bash
$ cd ~/axity-git-course/new-git-project/
``` 
Posteriormente ejecutar el comando:

```bash
$ git status
```
```bash
On branch master

Initial commit

nothing to commit (create/copy files and use "git add" to track)
```

### Crear un archivo HTML

Ahora creamos un archivo `index.html` 
```bash
    $ touch index.html
```
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

Adicional debemos:
 - crear el directorio `css` y dentro de él crear el archivo `app.css`
 - crear el directorio `js` y dentro de él crear el archivo `app.js`

```bash
$ mkdir css
$ mkdir js
$ touch css/app.css
$ touch js/app.js
```

Revisamos el estatus del repositorio después de crear directorios y archivos:

```bash
$ git status
```
![img_git_status_02](images/img_06_git_status_02.png)

#### ¿Qué significa esto?

![img_work_to_index](images/img_work_to_index.gif)

Para agregar el archivo `index.html` al Staging Index, debemos ejecutar el comando:
```bash
$ git add index.html
```
Revisamos nuevamente el estatus del repositorio:
```bash
$ git status
```
![img_git_status_03](images/img_06_git_status_03.png)

Para mover el resto de los archivos al Staging Index, ejecutamos el siguiente comando:

```bash
$ git add css/app.css js/app.js

# otra opción sería:
$ git add .
```

Volvemos a revisar el estatus del repositorio:

```bash
$ git status
```

![img_git_status_04](images/img_06_git_status_04.png)

Podemos observar que ahora todos los archivos se encuentran en el Staging Index.

### Aprovechar el poder del comando `git status`

> En este punto ya podemos identificar que git status es un comando bastante útil. Siempre debemos tenerlo en mente antes y después de cualquier otro comando de Git.

## Agregar commits

> Antes de avanzar, debemos estar seguros de haber configurado el editor por defecto de Git, ya que a partir de aquí lo usaremos para editar los mensajes de los commits.

Para hacer un commit debemos ejecutar el siguiente comando:
```bash
$ git commit
```
> Observemos el caracter `*` en el prompt `(master *)`. Esto indica que existen cambios que no hay sido enviados a un commit.

![img_git_status_04](images/img_06_git_status_04.png)

![img_git_status_04](images/img_06_git_status_04.png)


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzMzkxNDY1NTcsLTEwMDk5ODkyNzMsMT
c4MzEyMDU1OCwyMTAxODE0MDIxLC0xOTAyNzE3NDU2LC0xMDc1
MTExMDg2LDExMzA2MDEwMzcsMjM1OTMxNjE1LC0xMTMyODY3MD
k2LC00MTY2MDI2ODgsLTc0MTg0ODY4NSwtNzQxODQ4Njg1LC0x
MDc3OTg4MTE5LDEzNTEwNjY2NTMsLTE4MDQ2Mjc0NCwtMTgyMj
E4NDcyNCwtMTc4NDY2NTE0NywtMTg5ODk4NDcyMiwtNTgzMDgw
NjI0LDE3MTgyMzcyODFdfQ==
-->