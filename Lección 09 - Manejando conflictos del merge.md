# Manejando conflictos durante un merge

 - Un conflicto durante un merge puede ocurrir cuando una misma línea en un archivo es modificada en dos o más branches por separado. Por ejemplo, si dos personas realizan un cambio sobre el texto del título de la página web en diferentes branches.
 - En estos casos Git no puede determinar de forma automática cual línea conservar y cual eliminar.

## Forzar a un conflicto en merge

### Práctica 09 - Conflictos Merge
Para simular un conflicto durante un merge y aprender como manejar este tipo de conflicto realizaremos los siguientes pasos:

> Recuerda realizar commit despues de cada paso.

 1. En el archivo `index.html`, cambiar el encabezado `"Adventure"` por `"Quest"`en el branch `master`.

 2. Crear el branch `heading-update` apuntado al penúltimo commit (el pénultimo commit debe estar asociado al mensaje `"Merge branch 'sidebar'"`). Este cambio debe ser hecho sobre el branch `heading-update`.

 3. En el archivo `index.html`, cambiar el encabezado `"Adventure"` por `"Quest"`en el branch `master`.

<!--stackedit_data:
eyJoaXN0b3J5IjpbODgxOTUyNzE5LDE3Nzg3NDI5OTEsLTM4MD
A1MzQzNV19
-->