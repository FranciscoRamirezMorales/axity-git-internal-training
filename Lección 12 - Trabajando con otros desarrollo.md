# Trabajando con otros desarrollos

En esta lección veremos:

Usar la función fork

## Entendiendo la funcionalidad de `fork`

 - `fork` no es un comando de git
 - `fork` es una funcionalidad de Github

Para entender como funciona la funcionalidad de `fork` en GitHub realice los siguientes pasos:

1. Use `git clone` para clonar [Proyecto my-travel-plans de Lam](https://github.com/udacity/course-collaboration-travel-plans).

2. Hacer al menos un cambio en el repositorio (local).

3. Hacer `commit`.

4. Usar git push para enviar los cambios al repositorio de **Lam**

**¿Qués es lo que observa?**

> Podemos observar que al ejecutar git push nos devuelve el error "unable to access".

Ahora hagamos lo siguiente:

 1. Ingresemos en el [Proyecto my-travel-plans de Lam](https://github.com/udacity/course-collaboration-travel-plans).

 2. Damos clic en el botón **Fork**.

 3. Verificamos que ahora el repositorio de Lam se encuentra listado en nuestros repositorios.

 4. Volvemos a ejecutar `git push` para enviar los cambios al repositorio de **Lam**

**¿Qués es lo que observa ahora?**

> Podemos ver ahora los cambios son enviados al repositorio de Lam".

## Resumen

Fork es una acción hecha sobre el sevicio de GitHub:

Realiza una copia idéntica de otro repositorio
Se tiene control total sobre la copia del repositorio
Los cambios realizados en la copia no afectan al repositorio original

<!--stackedit_data:
eyJoaXN0b3J5IjpbNTIxMDEyNTMwLDkwODU4NzUwOF19
-->