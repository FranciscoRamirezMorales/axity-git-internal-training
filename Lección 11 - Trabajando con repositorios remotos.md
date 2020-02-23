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

```markdown
# Travel Destinations

A simple app to keep track of destinations I'd like to visit.
```

### Contenido de index.html

Add the following content to the index.html file:

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>Travels</title>
    <meta name="description" content="">
    <link rel="stylesheet" href="css/app.css">
</head>
<body>

    <div class="container">
        <div class="destination-container">
            <div class="destination" id="florida">
                <h2>Florida</h2>
            </div>

            <div class="destination" id="paris">
                <h2>Paris</h2>
            </div>
        </div>
    </div>

</body>
</html>

```


```bash
$ cd ~/axity-git-course
```
`my-travel-plans`
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MDYxODY3MjMsLTE1NDQwMzU3MDcsMT
cxMjQyMzk0MSwxMzY0ODc5MTg3LDcwNjgwMDk3MSwxMzc2ODQ4
MDk0LC01MjI3Nzk5MDYsNTM0MDk4MDE3XX0=
-->