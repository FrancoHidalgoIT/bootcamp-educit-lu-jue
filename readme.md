# CLASE 15

## Configuración inicial

´´´sh
git config --global user.name "Franco Hidalgo"
git config --global user.email "francohidalgo2016@gmail.com"

´´´
## CREAR un repositorio (inicializar un repositorio)

´´´sh
git init
´´´

## Areas del repositorio de GIT

3 Áreas

* Working directory (WD): Directorio de trabajo donde se van agregando o quitando los archivos durante el desarrollo.

* Stating area (SA): También conocida como área de control de cambios. Área tenporal intermedia. 

* Local Repo (LR): Una caja donde voy a ir teniendo todas las fotos que voy tomando. Se guardan acá.

## El estado de los archivos

* Untracked: (Archivos que estan en el WD pero GIT no les esta dando seguimiento)

* Unmodified: (Archivos que GIT ya está siguiendo y con respecto al WD, no fueron modificados)

* Modified: (Archivos que se encuentran en el repositorio, seguidos por GIT, pero difieren con lo que se encuentra actualmente en el WD)

* Staged: (Archivos que están en el area temporal /intermedia)

## Saber el estado actual de los archivos (comando)

´´´
git status
´´´
## Voy a  poder mover los archivos del WD al SA

´´´sh
git add (nombre del archivo)
ej. git add index.html
git add . (con este comando agrego a todos los archivos que están untracked o unmodified)


## Para "tomar la foto" y pasar el archivo del area de transición al LR

´´´
git commit -m "Descripción de lo que subo, breve"
´´´

´´´
git log (para ver el local repo, "la caja de fotos")
´´´

´´´
git log --oneline (me da la foto pero de forma resumida)

## Para pasar el archivo del area de transición al WD

´´´
git restore --staged (nombre del archivo)

## Para eliminar los cambios guardados del WD 

´´´
git restore (nombre del archivo)

## Mientras tanto no podemos vovler del LR con los cambios del archivo