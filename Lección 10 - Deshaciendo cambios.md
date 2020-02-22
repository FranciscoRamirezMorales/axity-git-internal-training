# Deshaciendo cambios

Aunque es poco común deshacer los cambios de un commit es posible hacerlo. En esta lección solo mencionaremos los recursos disponibles para poder realizar este tipo de acciones.

En esta lección mencionaremos como:

 -  Cambiar el último commit
 - Agregar archivos omitidos al último commit
 - Revertir un commit
 - Reset

## Cambiar el último commit

```bash
$ git commit --amend
```
Para poder usar este comando se deben realizar los siguientes pasos
-   edit the file(s)
-   save the file(s)
-   stage the file(s)
-   and run `git commit --amend`

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

-   `HEAD^` corresponde al commit `db7e87a`
-   `HEAD~1`corresponde al commit `db7e87a`
-   `HEAD^^` corresponde al commit `796ddb0`
-   `HEAD~2` corresponde al commit `796ddb0`
-   `HEAD^^^` corresponde al commit `0c5975a`
-   `HEAD~3` corresponde al commit `0c5975a`
-   `HEAD^^^2` corresponde al commit `4c9749e` (este es el `HEAD^^` del segundo padre (`^2`))

<!--stackedit_data:
eyJoaXN0b3J5IjpbODQzNTc0NjU1LC03ODM4ODQyMDYsLTEwOD
MyNTQ3OTYsMTMyOTgzNTU2LC0xOTg2NDczMjQ1LC05MTgxODA4
OTQsLTE2MTg0ODY0MzcsMzIyOTA5OTExXX0=
-->