# Agregando commits al repositorio

En esta lección veremos como:

 - Empezar a utilizar nuestro repositorio
 - Aprovechar el poder del comando `git status`
 - Agregar commits
 - Agregar mensaje a un commit
 - Ver cambios realizados antes de un commit
 - Omitir archivos en Git

## Empezar a utilizar nuestro repositorio

Antes de empezar a trabajar en nuestro repositorio debemos movernos al directorio `new-git-project` y posteriormente ejecutar el comando:

    # git status

Salida:

    On branch master

    Initial commit

    nothing to commit (create/copy files and use "git add" to track)

### Crear un archivo HTML

Crear un archivo index.html con el siguiente código:

```
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

dadsa

```js
  import { Component } from '@angular/core';
  import { MovieService } from './services/movie.service';

  @Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css'],
    providers: [ MovieService ]
  })
  export class AppComponent {
    title = 'app works!';
  }
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0NjIzODM0ODAsLTE3NTg5ODQ3MjQsMT
MyNjk0Njc2NywxODE1MTIxNzgwLDQxNjM1ODA2M119
-->