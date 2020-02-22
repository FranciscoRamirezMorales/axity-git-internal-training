# Deshaciendo cambios

Aunque es poco común deshacer los cambios de un commit es posible hacerlo. En esta lección solo mencionaremos los recursos disponibles para poder realizar este tipo de acciones.

En esta lección mencionaremos como:

 -  Cambiar el último commit
 - Agregar archivos omitidos al último commit
 - Revertir un commit
 - Reset


## Revertir un commit

```bash
$ git revert <SHA-del-commit-a-revertir>
```

Este comando:
 - Esta acción deshace los cambios realizados por el commit proporcionado
 - Crea un nuevo commit para registrar el cambio

## Revertir un commit

```bash
git reset <referencia-al-commit>
```

A diferencia de revert, un reset borra todos los commits indicados.

Opciones que se pueden usar en un `reset`:
-   `--mixed`
-   `--soft`
-   `--hard`

[![Git reset](http://img.youtube.com/vi/UN7ki2G2yKc/0.jpg)](http://www.youtube.com/watch?v=UN7ki2G2yKc "Git reset")



## Referencias relativas

Particularmente con reset podemos usar referencias relativas en lugar de especificar un commit en particular

Por ejemplo, si tenemos el siguiente log de commits:

```bash
* 9ec05ca (HEAD -> master) Revert "Set page heading to "Quests & Crusades""
* db7e87a Set page heading to "Quests & Crusades"
*   796ddb0 Merge branch 'heading-update'
|\  
| * 4c9749e (heading-update) Set page heading to "Crusade"
* | 0c5975a Set page heading to "Quest"
|/  
*   1a56a81 Merge branch 'sidebar'
|\  
| * f69811c (sidebar) Update sidebar with favorite movie
| * e6c65a6 Add new sidebar content
* | e014d91 (footer) Add links to social media
* | 209752a Improve site heading for SEO
* | 3772ab1 Set background color for page
|/  
* 5bfe5e7 Add starting HTML structure
* 6fa5f34 Add .gitignore file
* a879849 Add header to blog
* 94de470 Initial commit
```

En este caso `HEAD` apunta al commit `9ec05ca` y:

-   `HEAD^` correspon`db7e87a`
-   `HEAD~1` is also the `db7e87a` commit
-   `HEAD^^` is the `796ddb0` commit
-   `HEAD~2` is also the `796ddb0` commit
-   `HEAD^^^` is the `0c5975a` commit
-   `HEAD~3` is also the `0c5975a` commit
-   `HEAD^^^2` is the `4c9749e` commit (this is the grandparent's (`HEAD^^`) _second parent_ (`^2`))
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM2Mjk4NTkxMiwtMTk4NjQ3MzI0NSwtOT
E4MTgwODk0LC0xNjE4NDg2NDM3LDMyMjkwOTkxMV19
-->