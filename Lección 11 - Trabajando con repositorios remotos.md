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

 1. Crear el directorio `~/axity-git-course/my-travel-plans`
 2. Inicializar el directorio usando el comando `git init`
 3. Crear el archivo `README.md`
 4. Crear el archivo `index.html`
 5. Crear el archivo `app.css`

#### Contenido de `README.md`

```markdown
# Travel Destinations

A simple app to keep track of destinations I'd like to visit.
```

### Contenido de `index.html`

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

### COntenido del archivo app.css

```css
html {
    box-sizing: border-box;
    height: 100%;
}

*,
*::before,
*::after {
    box-sizing: inherit;
}

body {
    display: flex;
    margin: 0;
    height: 100%;
}

.container {
    margin: auto;
    padding: 1em;
    width: 80%;
}

.destination-container {
    display: flex;
    flex-flow: wrap;
    justify-content: center;
}

.destination {
    background: #03a9f4;
    box-shadow: 0 1px 9px 0 rgba(0, 0, 0, 0.4);
    color: white;
    margin: 0.5em;
    min-height: 200px;
    flex: 0 1 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

h2 {
    margin: 0;
    transform: rotate(-45deg);
    text-shadow: 0 0 5px #01579b;
}

#florida {
    background-color: #03a9f4;
}

#paris {
    background-color: #d32f2f;
}
```
 6. Guardar y cerrar los archivos.
 7. Realizar `commit`  con el mensaje `"Improve site heading for SEO"`.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgzNzQzOTI4NywxMzE0NzM0NTU3LC0xNT
Q0MDM1NzA3LDE3MTI0MjM5NDEsMTM2NDg3OTE4Nyw3MDY4MDA5
NzEsMTM3Njg0ODA5NCwtNTIyNzc5OTA2LDUzNDA5ODAxN119
-->