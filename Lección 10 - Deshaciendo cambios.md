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


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTkxODE4MDg5NCwtMTYxODQ4NjQzNywzMj
I5MDk5MTFdfQ==
-->