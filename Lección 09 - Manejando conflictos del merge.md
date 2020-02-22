# Manejando conflictos durante un merge

 - Un conflicto durante un merge puede ocurrir cuando una misma línea en un archivo es modificada en dos o más branches por separado. Por ejemplo, si dos personas realizan un cambio sobre el texto del título de la página web en diferentes branches.
 - En estos casos Git no puede determinar de forma automática cual línea conservar y cual eliminar.

## Forzar a un conflicto en merge

Para simular un conflicto durante un merge y aprender como manejar este tipo de conflicto realizaremos los siguientes pasos:


 1. En el archivo `index.html`, cambiar el encabezado `"Adventure"` por `"Quest"`en el branch `master`.

 2. Crear el branch `heading-update` apuntado al commit 

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI0MDAxMzAxNSwxNzc4NzQyOTkxLC0zOD
AwNTM0MzVdfQ==
-->