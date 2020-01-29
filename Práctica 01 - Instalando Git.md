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
    

> Si se requiere, ingresar el password **Welcome1** y reponder "**Y**" en todas las opciones.

## Configurar Terminal de Linux

1. Agregar las siguientes líneas al archivo `.bashrc`

# Enable tab completion
source ~/.udacity-terminal-config/git-completion.bash

# Change command prompt
source ~/.udacity-terminal-config/git-prompt.sh

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

1. Guardar y Cerrar

## Configuración Inicial de Git

1. Agregar cosas
```
# sets up Git with your name
git config --global user.name "<Your-Full-Name>"

# sets up Git with your email
git config --global user.email "<your-email-address>"

# makes sure that Git output is colored
git config --global color.ui auto

# displays the original state in a conflict
git config --global merge.conflictstyle diff3

git config --list
```

## Configurar Editor por defecto

<!--stackedit_data:
eyJoaXN0b3J5IjpbOTQyNDY4MDgwLC0xMDA3MjgxMDQzLC0zOD
M5MzA0NSwtMjEwMTEyNjMwNyw3NzM5NDEzMDUsODA0MDYzODU3
LDE4MzYyMzcwMiw5MDMzMDI5OTgsLTcxNzIzNjcxMywtMzA0MT
I2MzE4LDE5NjgwNzE4MzQsLTE5Mzg3MjU2NzEsMzU5NjczNDYs
NzMwOTk4MTE2XX0=
-->