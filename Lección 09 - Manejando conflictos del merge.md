# Manejando conflictos durante un merge

 - Un conflicto durante un merge puede ocurrir cuando una misma línea en un archivo es modificada en dos o más branches por separado. Por ejemplo, si dos personas realizan un cambio sobre el texto del título de la página web en diferentes branches.
 - En estos casos Git no puede determinar de forma automática cual línea conservar y cual eliminar.

## Forzar a un conflicto en merge

### Práctica 09 - Simular un conflicto en merge

Para simular un conflicto durante un merge y aprender como manejar este tipo de conflicto realizaremos los siguientes pasos:

> Recuerda realizar commit despues de cada paso.

 1. En el archivo `index.html`, cambiar el encabezado `"Adventure"` por `"Quest"`en el branch `master`. Mensaje: `"Set page heading to Quest"`.

 2. Crear el branch `heading-update` apuntado al penúltimo commit (el penúltimo commit debe estar asociado al mensaje `"Merge branch 'sidebar'"`). Este cambio debe ser hecho sobre el branch `heading-update`. 

 3. En el archivo `index.html`, cambiar el encabezado `"Adventure"` por `"Crusade"`en el branch `heading-update`. Mensaje: `"Set page heading to Crusade"`.

 4. Establecer `master` como el branch activo.
 5. Ejecutar el comando de merge:

```bash
$ git merge heading-update
```
El resultado debería verse como sigue:

![img_09_git_merge_01](images/img_08_git_merge_01.png)

Este mesaje indica que GIt no pudo realizar 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM0NzQ3ODU5LC02ODE2NDQ5NzIsMTc3OD
c0Mjk5MSwtMzgwMDUzNDM1XX0=
-->