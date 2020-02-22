# Pre-requisitos
Antes de comenzar, debemos asegurarnos de los siguiente:

 - Estar ubicado en el proyecto/directorio `new-git-project` y asegurar que existen los siguientes archivos:

    -   `index.html`
    -   `css/app.css` (vacío)
    -   `js/app.js` (vacío)

 - El archivo `index.html` contiene el siguiente código:

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

    <header>
        <h1>Expedition</h1>
    </header>

    <div class="container">
        <main>

        </main>
    </div>

    <footer>
        Made with ♥ @ Udacity
    </footer>
    <script src="js/app.js"></script>
</body>
</html>
```

 - Todos los archivos han sido agregados al Staging Index y se ha realizado un commit.
 - El único branch es master. Si existen otros branches, asegurar que han sido borrados.
 - Al ejecutar git status, la salida debe indicar que el directorio de trabajo esta limpio (`working directory clean`).

# Pasos a seguir

## 1. Agregar un color a la página

1. En el branch master agregar el siguiente contenido dentro del archivo `css/app.css`:

```css
body {
    background-color: #00cae4;
}
```

2. Guardar el archivo y cerrar.
1. Realizar `commit`  con el mensaje `"Add starting HTML structure"`.
1. Usar `git log --oneline` para ver el historial de commits.

## 2. Agregar barra lateral

1. Crear un `branch` llamado `sidebar` apuntando al **SHA** asociado al commit del mensaje `"Add starting HTML structure"`.
1. Realizar checkout para cambiar al branch `slidebar`.
1. Usar `git log --oneline` para ver el historial de commits.

> Podemos abrir el archivo   `css/app.css` en Atom y posteriormente cambiar entre el branch `master` y `slidebar` para poder observar como se actualiza el contenido en las diferentes versiones del archivo.

4. Crear una barra lateral. Para hacer esto se debe asegurar que el branch activo es `sidebar` y agregar el código del bloque `<aside>` al archivo HTML:

```html
<div class="container">
    <main>

    </main>
</div>

<!-- start of new content -->
<aside>
    <h2>About Me</h2>

    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos, debitis earum molestias veniam suscipit aliquam totam exercitationem tempore neque vitae. Minima, corporis pariatur facere at quo porro beatae similique! Odit.</p>
</aside>
<!-- end of new content -->

<footer>
    Made with ♥ @ Udacity
</footer>
```
5. Guardar y cerrar.
6. Realizar `commit`  con el mensaje `"Add new sidebar content"`.

## Cambiar el encabezado en `master`


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY0MTYxMzMyOCwxNDM4MDE3MDYxLDE4Mj
cxOTQzMzAsMTE2MTUyMzczOCwxODkzODI5OTIzXX0=
-->