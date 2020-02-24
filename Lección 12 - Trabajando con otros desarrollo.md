# Trabajando con otros desarrollos

 - En esta lección veremos:

 - Entendiendo la funcionalidad de `Fork`

 - Revisando el historial de cambios

 - Resumen

## Entendiendo la funcionalidad de `Fork`

 - `Fork` es una acción hecha sobre el servicio de **GitHub**:

 - Realiza una copia idéntica de otro repositorio.
 
 - Se tiene control total sobre la copia del repositorio.
 
 - Los cambios realizados en la copia no afectan al repositorio original.
 
 - `Fork` no es un comando de **Git**
 
 - `Fork` es una funcionalidad de **GitHub**

Para entender cómo funciona la funcionalidad de `fork` en **GitHub** realice los siguientes pasos:

1. Use `git clone` para clonar [Proyecto my-travel-plans de Lam](https://github.com/udacity/course-collaboration-travel-plans).

2. Hacer al menos un cambio en el repositorio (local).

3. Hacer `commit`.

4. Usar git push para enviar los cambios al repositorio de **Lam**

**¿Qué es lo que observa?**

> Podemos observar que al ejecutar git push nos devuelve el error "unable to access".

Ahora hagamos lo siguiente:

 1. Ingresemos en el [Proyecto my-travel-plans de Lam](https://github.com/udacity/course-collaboration-travel-plans).

 2. Damos clic en el botón **Fork**.

 3. Verificamos que ahora el repositorio de Lam se encuentra listado en nuestros repositorios.

 4. Volvemos a ejecutar `git push` para enviar los cambios al repositorio de **Lam**

**¿Qué es lo que observa ahora?**

> Podemos ver ahora los cambios son enviados al repositorio de Lam".

## Revisar el historial de cambios

 1. Clonar el [Proyecto Lighhouse](https://github.com/GoogleChrome/lighthouse).

 2. Moverse al directorio del repositorio recién clonado.

### Agrupado por autor

```bash
$ git shortlog
```

### Por el número de commits ordenado numéricamente 

```bash
$ git shortlog -s -n
```

## Filtrar por autor

```bash
$ git log --author=Surma
$ git log --author="Paul Lewis"
```

## Filtrar por commit especifico

```bash
$ git show 5966b66
```

## Filtrar por un palabra en el mensaje del commit

```bash
$ git log --grep=bug
$ git log --grep bug
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM5NDE5ODA4MSw1ODU4MjMwNDksLTIxND
Q2NzExNzksOTA4NTg3NTA4XX0=
-->