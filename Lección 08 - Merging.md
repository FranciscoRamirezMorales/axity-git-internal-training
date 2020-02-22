# Merging

En esta lección veremos los dos principales tipos de **Merge**:

 - ¿Qué es merge?
 - Fast-forward merge
 - Regular merge

## ¿Qué es merge?
Recordemos que el propósito de un branch (por ejemplo `sidebar`) es que nos permite realizar cambios que no afectan al branch `master`. Una vez que realizamos cambios en el branch `sidebar` podemos decidir que esos cambios no aplicarán, eliminarlos o mantenerlos y posteriormente combinarlos con otra rama.

**A la acción de combinar dos branches se le denomina `merge`.**
ara entender como funciona el comando merge, podemos ver el siguiente video:

**Video >>> (dar clic)**

[![Git merge](http://img.youtube.com/vi/gQiWicrreJg/0.jpg)](http://www.youtube.com/watch?v=gQiWicrreJg "Git merge")

## Fast-forward merge
Este es el mas simple de los merge, ya que como se puede observar en el video, el apuntador `HEAD` del branch `master` es movido al commit mas `reciente/adelantado`.

```bash
$ git merge footer
```

## Regular merge
Este tipo de merge es el más común ya que implica combinar dos branches cuyas 
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDgzNDMwMjYsMjEyOTA1ODY0MSwtMzg0Nj
QyMjMxLDQ3NDE0Nzk1Ml19
-->