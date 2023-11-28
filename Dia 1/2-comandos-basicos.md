# Comandos Básicos de GIT

## git config

`git config` es un comando que define valores de configuración de Git a nivel de un proyecto global o local

```
git config --global user.name "Juan Kuga”
git config --global user.email juankp3@gmail.com
```

## git init
`git init` es un comando que se utiliza una sola vez durante la configuración inicial de un repositorio nuevo. Al ejecutar este comando, se crea un directorio `.git/` en tu directorio de trabajo actual. 

```
git init
```

## git remote
`git remote` muestra el nombre del repositorio remoto al que estamos conectado.

```
git remote
git remote -v
```
## git add
`git add` añade un cambio del directorio de trabajo en el entorno de ensayo. De este modo, indica a Git que quieres incluir actualizaciones en un archivo concreto en la próxima confirmación.
```
git add .
git add --all
```
## git commit
`git commit` captura una instantánea de los cambios preparados en ese momento del proyecto. Las instantáneas confirmadas pueden considerarse como versiones "seguras" de un proyecto: Git no las cambiará nunca a no ser que se lo pidas expresamente.

```
git commit -m "mensaje de confirmación de los cambios realizados"
```

## git push
El comando git push se usa para cargar contenido del repositorio local a un repositorio remoto. El envío es la forma de transferir confirmaciones desde tu repositorio local a un repositorio remoto.

```
git push origin <branch-name>
```

## git pull
El comando git pull se emplea para extraer y descargar contenido desde un repositorio remoto y actualizar al instante el repositorio local para reflejar ese contenido. La fusión de cambios remotos de nivel superior en tu repositorio local es una tarea habitual de los flujos de trabajo de colaboración basados en Git.

```
git pull origin <branch-name>
```

## git branch
El comando git branch te permite crear, enumerar y eliminar ramas, así como cambiar su nombre. No te permite cambiar entre ramas o volver a unir un historial bifurcado. Por este motivo, git branch está estrechamente integrado con los comandos git checkout y git merge .

```
git branch <branch-name>
```

Elimina una rama sin cambios nuevos. (Rama ya fusionada)
```
git branch -d <branch-name>
```

Elimina una rama de forma definitiva con o sin cambios nuevos
```
git branch -D <branch-name>
```

## git checkout
El comando git checkout te permite desplazarte entre las ramas creadas por git branch . Al extraer una rama, se actualizan los archivos en el directorio de trabajo para reflejar la versión almacenada en esa rama y se indica a Git que registre todas las confirmaciones nuevas en dicha rama.
```
git checkout <branch-name>
```

## git merge
El comando git merge permite tomar las líneas independientes de desarrollo creadas por git branch e integrarlas en una sola rama. Ten en cuenta que todos los comandos presentados a continuación se fusionan en la rama actual

```
git merge <branch-name>
```

## git log
El comando git log es una herramienta básica de Git para explorar el historial del repositorio. Este comando se usa cuando necesitas buscar una versión concreta de un proyecto o saber los cambios que se introducirán mediante la fusión en una rama de función.

```
git log <branch-name>
```

## git ignore
gitignore , es un archivo de texto que le dice a Git qué archivos o carpetas ignorar en un proyecto. Un archivo local . gitignore generalmente se coloca en el directorio raíz de un proyecto. También puedes crear un archivo global

```
.gitignore
```

## git clone
git clone es una utilidad de línea de comandos de Git que se utiliza para fijar como objetivo un repositorio existente con el fin de clonarlo o copiarlo.

```
git clone
```
## git ammend
git clone es una utilidad de línea de comandos de Git que se utiliza para fijar como objetivo un repositorio existente con el fin de clonarlo o copiarlo.

```
git ammend
```