# Instalando Git

Para habilitar un ambiente de Git es necesario realizar los siguientes pasos:

 - Instalar Git

 - Configurar Terminal de Linux

 - Configuración Inicial de Git

 - Configurar Editor por defecto

## Instalar Git
 1. Iniciar la máquina virtual "**VM - Internal Training - Git**"
 2. Iniciar sesión con el **usuario**: **axity** / **password**: **Welcome1**
 3. Abrir una Terminal
 4. Para instalar Git ejecutar:

        # sudo add-apt-repository ppa:git-core/ppa
        # sudo apt update
        # sudo apt install git

> También podemos usar `apt-get` para instalar Git.

> Si se requiere, ingresar la contraseña **Welcome1** y responder "**Y**" en todas las opciones.

## Configurar Terminal de Linux

Agregar las siguientes líneas al archivo `.bashrc` (Usar **vi** o algún otro editor):

```
# Enable tab completion
source ~/.axity-terminal-config/git-completion.bash

# Change command prompt
source ~/.axity-terminal-config/git-prompt.sh

# colors!
red="\[\033[38;5;203m\]"
green="\[\033[38;05;38m\]"
blue="\[\033[0;34m\]"
reset="\[\033[0m\]"

export GIT_PS1_SHOWDIRTYSTATE=1

# '\u' adds the name of the current user to the prompt
# '\$(__git_ps1)' adds git-related stuff
# '\W' adds the name of the current directory
export PS1="$red\u$green\$(__git_ps1)$blue \W
$ $reset"
```
Descargar el directorio `axity-terminal-config` que se encuentra en dentro del directorio `resources` del repositorio de curso y copiarla dentro de la ruta `/home/axity/` con el nombre `.axity-terminal-config` (nótese que debe incluirse un "."). 

La ruta debería verse así:

    /home/axity/.axity-terminal-config


## Configuración Inicial de Git

Ejecutar las siguientes líneas para realizar la configuración inicial de Git:

Configurar Git con tu nombre

    # git config --global user.name "<Tu nombre completo>"

Configurar Git con tu e-mail

    # git config --global user.email "<Tu e-mail>"

Configurar la configuración de colores del texto de salida

    # git config --global color.ui auto

Configurar la forma en que se despliegan los estatus en conflicto

    # git config --global merge.conflictstyle diff3
    # git config --list

## Configurar Editor por defecto

Para configurar el editor por defecto (**Atom**) de Git ejecutar el siguiente comando:

    # git config --global core.editor "atom --wait"



<!--stackedit_data:
eyJoaXN0b3J5IjpbNzQ4ODMzMjIwLDkyMzk3OTc5OCwtMTQ5ND
kwMTA2MCwtMjA5MzU3NTI1NCwxOTkwNzg1MzE4LDE3MjIzNDA3
NzgsMTk1MjgzMzMsMTMzMjI1NTQ1MiwxNzc4OTU1MDUwXX0=
-->