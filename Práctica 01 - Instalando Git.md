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

Agregar las siguientes líneas al archivo `.bashrc` (Usar **vi** o algun otro editor):

```
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
```

## Configuración Inicial de Git

Ejecutar las siguientes lineas en línea de comandos para realizar la configuración inicial de Git:

Configurar Git con tu nombre

    $ git config --global user.name "<Tu nombre completo>"

Configurar Git con tu email

    $ git config --global user.email "<Tu e-mail>"

Configurar la configuración de colores del texto de salida

    $ git config --global color.ui auto

Configurar la forma en que se despliegan los estatus en conflicto

    $ git config --global merge.conflictstyle diff3
    $ git config --list


## Configurar Editor por defecto

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkzMzU2OTMxMywtNTQ4Mjg0Mzg2LC04Nz
M4Mjg4OTgsLTExOTMxNTIyOSwtMTAwNzI4MTA0MywtMzgzOTMw
NDUsLTIxMDExMjYzMDcsNzczOTQxMzA1LDgwNDA2Mzg1NywxOD
M2MjM3MDIsOTAzMzAyOTk4LC03MTcyMzY3MTMsLTMwNDEyNjMx
OCwxOTY4MDcxODM0LC0xOTM4NzI1NjcxLDM1OTY3MzQ2LDczMD
k5ODExNl19
-->